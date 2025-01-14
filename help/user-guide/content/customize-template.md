---
title: Personalizar um modelo
description: Saiba como personalizar e otimizar seu modelo para o Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 8930d3284f9dd1223067239c0077e481ea98335a
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 0%

---

# Personalizar um modelo

Você pode personalizar um modelo para usar no GenStudio for Performance Marketing inserindo espaços reservados para conteúdo, ou campos, que a IA geradora usa para inserir conteúdo.

As próximas seções explicam como adaptar seus modelos de HTML para o GenStudio for Performance Marketing usando a linguagem de modelo _Handlebars_. A sintaxe [!DNL Handlebars] usa texto regular com chaves duplas como espaços reservados para conteúdo. Consulte [O que é [!DNL Handlebars]?](https://handlebarsjs.com/guide/#what-is-handlebars) no _guia de idioma do Handlebars_ para saber como preparar seu modelo.


Quando o modelo estiver pronto, você poderá [carregá-lo no GenStudio for Performance Marketing](use-templates.md#upload-a-template) e começar a gerar emails personalizados com base no modelo personalizado.

>[!TIP]
>
>Siga as [diretrizes de acessibilidade](accessibility-for-templates.md) e as [práticas recomendadas](/help/user-guide/content/best-practices-for-templates.md) para que você possa alcançar mais de seu público-alvo e fornecer uma experiência ideal.

## Espaços reservados de conteúdo

A GenStudio for Performance Marketing reconhece determinados [elementos](use-templates.md#template-elements) em um modelo, mas somente se você identificá-los com um nome de campo reconhecido.

Dentro do cabeçalho ou do corpo de um modelo, você pode usar a sintaxe [!DNL Handlebars] como um espaço reservado de conteúdo, em que você requer que o GenStudio for Performance Marketing preencha o modelo com conteúdo real. A GenStudio for Performance Marketing reconhece e interpreta os espaços reservados de conteúdo com base no [nome do _campo_ reconhecido](#recognized-field-names).

Por exemplo, você pode usar `{{ headline }}` com a sintaxe [!DNL Handlebars] para indicar onde o título do email deve ser colocado:

```handlebars
<div>{{headline}}</div>
```

### Nomes de campo reconhecidos

A tabela a seguir lista os nomes de campo reconhecidos pelo GenStudio for Performance Marketing para preenchimento em modelos. Adicione esses nomes de campos usando a sintaxe [!DNL Handlebars] ao modelo em que você precisa do GenStudio for Performance Marketing para gerar conteúdo.

| Texto | Função | Modelo de canal |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | Pré-cabeçalho | email |
| `{{headline}}` | Título | email <br>Meta-anúncio <br>Exibir anúncio |
| `{{body}}` | Corpo do texto | email <br>Meta-anúncio <br>Exibir anúncio |
| `{{cta}}` | Chamada para ação | email <br>Meta-anúncio <br>Exibir anúncio |
| `{{on_image_text}}` | No texto da imagem | Meta-anúncio |
| `{{image}}` | Imagem — selecione a partir do conteúdo | email <br>Meta-anúncio <br>Exibir anúncio |
| `{{brand_logo}}` | Logotipo da marca selecionada<br>Consulte [Nome do campo do logotipo da marca](#brand-logo-field-name) para obter o uso recomendado. | email<br>Meta-anúncio |

O GenStudio for Performance Marketing preenche determinados campos automaticamente nos seguintes modelos:

- **O modelo de email** não requer que você identifique o campo `subject`
- **O modelo de metadados** não requer que você identifique os campos `headline`, `body` e `CTA`
- **O modelo Exibir Anúncios** não requer que você identifique o campo `CTA`

>[!WARNING]
>
>Para anúncios do Instagram, o título gerado não aparece na experiência final.

Há um limite de 20 campos ao fazer upload de um modelo para o GenStudio for Performance Marketing. Como o campo `subject` é gerado automaticamente em um email, ele conta como um campo. Isso significa que há 19 campos permitidos em um template de email.

>[!TIP]
>
>Você pode verificar seu modelo usando a [visualização do modelo](#template-preview) no GenStudio for Performance Marketing.

#### Nome do campo de logotipo da marca

No momento, não é possível selecionar o logotipo da marca para o upload do modelo. Os exemplos a seguir demonstram dois métodos que renderizam condicionalmente o logotipo da marca. Cada método verifica a origem, fornece uma imagem padrão ou alternativa caso o logotipo da marca não esteja disponível e aplica um estilo:

**Exemplo 1**: usando a condição [!DNL Handlebars] Built-in Helpers diretamente no atributo HTML `img src`:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Exemplo 2**: usando a instrução de condição interna [!DNL Handlebars] para envolver a marca HTML `img`:

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Nomes de campo manuais

Todos os outros nomes de campo são tratados como campos preenchidos manualmente.

Para criar uma seção editável, adicione colchetes duplos ao redor do nome da seção:

```handlebars
{{customVariable}}
```

### Seções ou grupos

_As seções_ informam à GenStudio for Performance Marketing que os campos desta seção exigem um alto grau de coerência. O estabelecimento dessa relação ajuda a IA a gerar conteúdo que corresponde aos elementos criativos na seção.

Use um prefixo de sua escolha no nome do campo para indicar que um campo faz parte de uma seção ou grupo. Use um nome de campo (`headline`, `body`, `image` ou `cta`) após o sublinhado (`_`). Por exemplo, o título e o corpo a seguir pertencem à seção `pod1`:

- `pod1_headline`
- `pod1_body`

Cada seção pode usar apenas um de cada tipo de campo. No exemplo acima, a seção `pod1` só pode usar um campo `pod1_headline`. Por causa dessa regra, as seções não podem ser aninhadas.

Cada tipo de modelo, como email ou Meta ad, tem restrições específicas de canal no uso de seções. Consulte as [diretrizes específicas do canal](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) no tópico _Práticas recomendadas para usar modelos_.

Por exemplo, um template de email pode incluir até três seções; portanto, você pode ter três seções de título e corpo:

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

A GenStudio for Performance Marketing entende que `pod1_headline` está mais intimamente relacionado a `pod1_body` do que a `pod2_body`.

Consulte [Prompts estruturados](/help/user-guide/effective-prompts.md#structured-prompts) para saber como criar um prompt que gera conteúdo variável para cada seção de um email.

## Visualização do modelo

Quando você [carrega um modelo](use-templates.md#upload-a-template), o GenStudio for Performance Marketing verifica o arquivo HTML em busca de campos reconhecidos. Use a visualização para revisar seus [elementos do modelo](use-templates.md#template-elements) e confirmar se você os identificou corretamente com os [nomes de campo reconhecidos](#recognized-field-names).

Exemplo de visualização para um modelo de email:

![Campos de visualização detectados](/help/assets/template-detected-fields.png){width="650"}

### Visualização do controle

Você pode controlar a visibilidade de conteúdo especial usando Auxiliares Internos (expressões especiais na linguagem de modelo [!DNL Handlebars] que executam determinadas ações). Por exemplo, é possível adicionar uma declaração condicional que adicione parâmetros de rastreamento aos links no modelo exportado, mantendo os links de visualização limpos.

O valor `_genStudio.browser` é definido ao renderizar um modelo, e o valor `genStudio.export` é definido ao exportar um modelo. Você pode decidir incluir determinado conteúdo na parte superior de um email usando um invólucro condicional, por exemplo, quando o modelo for usado para exportação:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Outro exemplo pode ser impedir o uso de códigos de rastreamento ao visualizar um modelo no GenStudio for Performance Marketing. O exemplo a seguir mostra como adicionar parâmetros de rastreamento a links no modelo exportado, mantendo os links de visualização limpos:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Conteúdo estático

Os modelos de email e meta geralmente vinculam a imagens e arquivos CSS hospedados fora do GenStudio for Performance Marketing. Quando o GenStudio for Performance Marketing gera miniaturas para esses modelos ou as experiências derivadas deles, ele pode ignorar esses recursos externos se eles não tiverem os cabeçalhos corretos do CORS (Cross-Origin Resource Sharing, Compartilhamento de recursos entre origens).

Para garantir que esses recursos estejam disponíveis durante o processo de geração de miniaturas, considere duas opções:

1. **Usar cabeçalhos CORS**: o servidor host deve enviar respostas com um cabeçalho `Access-Control-Allow-Origin` definido como valor `https://experience.adobe.com` para ambientes de produção. Esse método permite que o GenStudio for Performance Marketing acesse e inclua os recursos.

1. **Usar URLs de Dados**: Incorpore os recursos externos diretamente no modelo usando URLs de Dados. Esse método ignora as restrições do CORS e garante que os recursos estejam disponíveis durante a geração de miniaturas.

>[!TIP]
>
>Use [atualizar](/help/user-guide/content/use-templates.md#refresh-template) para atualizar a visualização do modelo com o conteúdo estático mais recente.

## Exemplos de modelo

+++Exemplo: modelo de email com uma seção

Este é um exemplo básico de um modelo de HTML para um email que contém uma seção. O cabeçalho contém CSS simples e em linha para estilo. O corpo contém um `pre-header`, `headline`, e `image` [espaço reservado](#content-placeholders) para uso do GenStudio for Performance Marketing para inserir conteúdo durante o processo de geração de email.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Exemplo: modelo de email com várias seções

O modelo a seguir é o mesmo modelo de HTML no exemplo acima, mas com mais duas seções. O cabeçalho contém CSS em linha para estilizar um grupo. O corpo usa dois grupos com [espaços reservados para o conteúdo](#content-placeholders) usando um prefixo.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Exemplo: modelo de metadados

Este é um exemplo básico de um modelo de Meta-anúncio. O cabeçalho contém CSS em linha para estilo. O corpo usa [espaços reservados para o conteúdo](#content-placeholders) usando um prefixo.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
