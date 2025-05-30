---
title: Diretrizes do modelo de email
description: Siga as práticas recomendadas ao usar modelos de email com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Diretrizes do modelo de email

Um template de email de marketing serve como base para campanhas de email visualmente envolventes e responsivas. Em geral, os templates do HTML permitem controlar o layout, a tipografia, as cores e as imagens para alinhar-se às diretrizes da marca. Ao preparar seu modelo para uso no GenStudio for Performance Marketing, use o HTML semântico e o CSS em linha para estilizar e evite scripts ou dependências externas. Modelos bem estruturados do HTML podem aprimorar a experiência do recipient e melhorar a capacidade de entrega e as taxas de engajamento.

Siga estas práticas recomendadas de design ao personalizar modelos de email para funcionar com o GenStudio for Performance Marketing:

- Usar fontes do Adobe ou Google
- Usar HTML limpo e responsivo e CSS em linha
- **não** usar o JavaScript
- **não** usar largura fixa no corpo ou contêiner
- **não** usar a codificação base64 para imagens porque ela pode aumentar significativamente o tamanho do modelo
- O tamanho máximo do arquivo do HTML é 102 KB

## Nomes de campo reconhecidos

O GenStudio for Performance Marketing gera automaticamente o campo `subject` para emails. Ao personalizar o modelo, use espaços reservados para o conteúdo para os seguintes campos obrigatórios:

- `pre_header` (rich text não habilitado)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selecionado no JPEG de conteúdo, PNG ou GIF)

Os campos máximos permitidos em um modelo são 20. Consulte [Espaços reservados para conteúdo](/help/user-guide/content/customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

## Email de várias seções

_Seções_ permitem que você organize o conteúdo em grupos distintos, que oferecem suporte a layouts mais complexos. No Genstudio para Marketing de desempenho, é possível definir cada seção usando uma convenção de nomenclatura de grupo. Consulte [Personalizar seções de modelo](/help/user-guide/content/customize-template.md#sections-or-groups).

Os modelos de várias seções podem ter 0, 2 ou 3 seções:

- Um modelo básico (seções zero) pode gerar um único conjunto de elementos de modelo, o que não requer a convenção de nomenclatura de grupo.
- Um modelo complexo (várias seções) pode gerar até três conjuntos de elementos de modelo, o que requer que você siga a convenção de nomenclatura de grupo: (`groupname_fieldname`)

Exemplo de nomes de campo para duas seções:

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

## Exemplos de modelo

+++Exemplo: modelo de email com uma seção

Este é um exemplo básico de um modelo HTML para um email que contém uma seção. O cabeçalho contém CSS simples e em linha para estilo. O corpo contém um `pre_header`, `headline`, e `image` [espaço reservado](#content-placeholders) para uso do GenStudio for Performance Marketing para inserir conteúdo durante o processo de geração de email.

```html {line-numbers="true" highlight="13"}
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Exemplo: modelo de email com várias seções

O modelo a seguir é o mesmo modelo de HTML no exemplo acima, mas com mais duas seções. O cabeçalho contém CSS em linha para estilizar um grupo. O corpo usa dois grupos com [espaços reservados para o conteúdo](#content-placeholders) usando um prefixo.

```html
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++
