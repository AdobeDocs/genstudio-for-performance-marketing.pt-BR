---
title: Personalizar um modelo
description: Saiba como personalizar seu modelo do HTML usando espaços reservados para conteúdo reconhecidos pela IA gerativa do Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
TQID: https://experienceleague.adobe.com/6gHxPvfz-30X3w2MYIc2Aj5SiGZokzOqSvOHYTQ-u7I
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2: id: be495d08-ecd1-455f-951e-c22de504e667id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: e8e0898054576454bad9ecdbd1a48b17f955e138
workflow-type: tm+mt
source-wordcount: 1646
ht-degree: 0%

---

# Personalizar um modelo

Você pode personalizar um modelo para usar no GenStudio for Performance Marketing inserindo espaços reservados para conteúdo, ou campos, que a IA geradora usa para inserir conteúdo.

As próximas seções explicam como adaptar seus modelos do HTML para o GenStudio for Performance Marketing usando a linguagem de modelo _[!DNL Handlebars]_. A sintaxe [!DNL Handlebars] usa texto regular com chaves duplas como espaços reservados para conteúdo. Consulte [O que é [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) no_ Guia de linguagem do Handlebars _para saber como preparar seu modelo.

Quando o modelo estiver pronto, você poderá [carregá-lo no GenStudio for Performance Marketing](use-templates.md#upload-a-template) e começar a gerar emails personalizados com base no modelo personalizado.

Siga as [diretrizes de acessibilidade](accessibility-for-templates.md) e as [práticas recomendadas](/help/user-guide/templates/best-practices-for-templates.md) para que você possa alcançar mais de seu público-alvo e fornecer uma experiência ideal.

## Espaços reservados de conteúdo

>[!TIP]
>
>Os espaços reservados para o conteúdo são **não** o mesmo que o texto de espaço reservado no conteúdo a ser preenchido posteriormente por um usuário. Veja mais sobre [o uso de texto de espaço reservado em modelos](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates).

O GenStudio for Performance Marketing reconhece determinados tipos de conteúdo ou [elementos](use-templates.md#template-elements) em um modelo, mas somente se você identificá-los com um [nome de campo reconhecido](#recognized-field-names).

No cabeçalho ou no corpo de um modelo do HTML, é possível usar a sintaxe [!DNL Handlebars] para inserir um espaço reservado para conteúdo, em que você precisa que o GenStudio for Performance Marketing preencha o modelo com conteúdo real. A GenStudio for Performance Marketing reconhece e interpreta esses espaços reservados com base no [nome do _campo_ reconhecido](#recognized-field-names). Cada nome de campo está associado a regras e comportamentos específicos que determinam como o conteúdo é gerado e inserido no modelo.

Por exemplo, você pode usar `{{headline}}` com a sintaxe [!DNL Handlebars] para indicar onde o título do email deve ser colocado. O GenStudio reconhece esse campo, gera um título relevante com base nas diretrizes e critérios de prompt e insere o título neste local:

```handlebars
<div>{{headline}}</div>
```

### Nomes de campo reconhecidos

A tabela a seguir lista os nomes de campo reconhecidos pelo GenStudio for Performance Marketing para adicionar um espaço reservado em um modelo. Cada campo segue diretrizes de canal específicas, instruções LLM e regras baseadas em função. Adicione esses nomes de campos usando a sintaxe [!DNL Handlebars] ao modelo em que você precisa do GenStudio for Performance Marketing para gerar um determinado tipo de conteúdo.

| Campo | Função | Modelo de canal |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Pré-cabeçalho | email |
| `{{headline}}` | Título | email <br>Anúncio do Meta <br>Banner e anúncio de exibição <br>Anúncio do LinkedIn |
| `{{sub_headline}}` | Subtítulo | email<br>Banner e Anúncio de exibição |
| `{{introductory_text}}` | Texto introdutório | Anúncio do LinkedIn |
| `{{body}}` | Corpo do texto | email <br>Anúncio do Meta <br>Banner e Anúncio de exibição |
| `{{cta}}` | Call to action<br>Consulte [Chamadas para ação](#calls-to-action) | email <br>Anúncio do Meta <br>Banner e anúncio de exibição <br>Anúncio do LinkedIn |
| `{{image}}` | Imagem — selecione de [!DNL Content] | email <br>Anúncio do Meta <br>Banner e anúncio de exibição <br>Anúncio do LinkedIn |
| `{{on_image_text}}` | No texto da imagem<br>Consulte [No texto da imagem](#on-image-text). | Anúncio do Meta <br>LinkedIn |
| `{{link}}` | Call to action na imagem<br>Consulte [Link na imagem](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

O GenStudio for Performance Marketing gera determinados campos automaticamente nos seguintes modelos:

- **O modelo de email** não exige que você identifique o campo `subject`
- **O modelo de anúncio do Meta** não exige que você identifique os campos `headline`, `body` e `CTA`
- **Modelo de banner e anúncio de exibição** não requer que você identifique o campo `CTA`
- **O modelo de anúncio do LinkedIn** não requer que você identifique os campos `headline`, `introductory_text` e `CTA`

>[!WARNING]
>
>Para anúncios do Instagram, o título gerado não aparece na experiência final.

Há um limite de 20 campos ao fazer upload de um modelo para o GenStudio for Performance Marketing. Como o campo `subject` é gerado automaticamente em um email, ele conta como um campo. Isso significa que há 19 campos permitidos em um template de email.

>[!TIP]
>
>Você pode verificar seu modelo usando a [visualização do modelo](#template-preview) no GenStudio for Performance Marketing.

### Planos de ação

Um Call to action (CTA) inclui uma frase e um link. Para que os recursos _[!UICONTROL Rephrase]_ e _[!UICONTROL Adicionar link]_ funcionem corretamente durante o processo de geração de variante, você deve incluir espaços reservados para o link e a frase no modelo.

Use a orientação a seguir para configurar espaços reservados para o CTA:

- A refrase do CTA está disponível e o link é editável

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- A refrase do CTA está disponível, mas o link **não** é editável porque o link real é fornecido no modelo

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- O link do CTA é editável, mas a refrase está **não** disponível porque a frase é fornecida no modelo

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

O GenStudio for Performance Marketing também pode fornecer frases de chamada para ação de variante. Consulte [Revise o Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Link na imagem

Você pode personalizar seu modelo de email para permitir que os criadores adicionem um link a uma imagem. Semelhante ao link do CTA, use a seguinte orientação para aplicar um espaço reservado `link` a uma marca de imagem:

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

Neste exemplo:

- `{{link}}` é um espaço reservado para a URL real.
- `src="image-source.jpg"` deve ser substituído pela URL de origem da imagem real.
- `{{imageDescription}}` é um nome de campo definido pelo usuário que fornece um espaço reservado para o texto alternativo da imagem, útil para acessibilidade e SEO.

### Texto alternativo

Use um nome de campo definido pelo usuário como um espaço reservado para gerar uma descrição de texto alternativo (atributo HTML `alt="text"`) para uma imagem. O espaço reservado `{{imageDescription}}` a seguir é usado com o campo `{{image}}` dentro da mesma marca `<img>`, garantindo que a relação entre a imagem e sua descrição persista.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

Neste exemplo:

- `{{image}}` é o espaço reservado para a URL de origem da imagem.
- `{{imageDescription}}` é o espaço reservado para o texto alternativo, que fornece uma descrição da imagem para fins de acessibilidade e SEO.

### Rótulo de acessibilidade

O atributo `aria-label` é usado para definir um nome acessível para elementos que não têm rótulos visíveis. Esse atributo é especialmente útil em modelos nos quais é importante fornecer contexto para elementos interativos, como um botão do CTA.

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

### No texto da imagem

O espaço reservado `{{on_image_text}}` é usado para especificar uma sobreposição de texto de mensagens de impacto curto, colocadas diretamente na imagem em uma experiência.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- 
this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Nomes de campo manuais

Todos os outros nomes de campo são definidos pelo usuário e tratados como campos preenchidos manualmente. Por exemplo, talvez você queira reservar uma seção para conteúdo de rodapé.

Para criar uma seção editável, adicione colchetes duplos ao redor do nome da seção:

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

### Edição de rich text

Aprimore seu conteúdo criativo durante o processo do [!DNL Create] com a edição de rich text. A tela determina a capacidade de rich text com base no local do espaço reservado para conteúdo. A capacidade de Rich Text está disponível somente quando você usa espaços reservados de conteúdo como elementos autônomos ou em marcas HTML de nível de bloco, como `<p>`, `<div>` ou `<span>`.

A edição de rich text está disponível para conteúdo independente em um parágrafo:

```html
<p>{{body}}</p>
```

Se você usar um espaço reservado para conteúdo dentro de um atributo do HTML (como `alt`, `href` ou `src`), a edição de rich text não será suportada para esse campo.

A edição de rich text **não** está disponível para o conteúdo `alt`:

```html
<img src="image.jpg" alt="{{image_description}}">
```

Se um campo for exibido mais de uma vez, a capacidade de rich text será determinada com base no fato de ser usado como um atributo do HTML em qualquer uma das instâncias. Por exemplo, quando o título é usado como um título e como texto alternativo para uma imagem, a marca `alt` tem prioridade.

A edição de rich text **não** está disponível para `headline`, pois é usada como conteúdo `alt`:

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

A edição de rich text pode estar disponível para determinados campos em canais específicos, como `on_image_text` em canais sociais (Meta, LinkedIn).

## Seções ou grupos

Se o seu modelo de email exigir várias áreas de conteúdo, como várias ofertas ou histórias, você poderá organizá-las usando seções ou grupos. _As seções_ informam à GenStudio for Performance Marketing que os campos desta seção exigem um alto grau de coerência. O estabelecimento dessa relação ajuda a IA a gerar conteúdo que corresponde aos elementos criativos na seção.

Use um nome de grupo de sua escolha como um prefixo para indicar que um campo faz parte de uma seção ou grupo. Use um nome de campo (como `headline`, `body`, `image` ou `cta`) após o sublinhado (`_`).

Sintaxe: `groupname_fieldname`

- _Correção_ (👍): `pod1_body`
- _Incorreto_ (❌): `pod1body`

Cada seção pode usar apenas um de cada tipo de campo. Por exemplo, os seguintes campos pertencem à seção `pod1`:

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Por causa dessa regra, as seções não podem ser aninhadas.

Cada tipo de modelo, como email ou anúncio do Meta, tem restrições específicas de canal no uso de seções. Consulte as [diretrizes específicas do canal](/help/user-guide/templates/best-practices-for-templates.md) no tópico _Práticas recomendadas para usar modelos_.

Por exemplo, um template de email pode incluir até três seções; portanto, você pode ter três seções de título e corpo:

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

A GenStudio for Performance Marketing entende que `pod1_headline` está mais intimamente relacionado a `pod1_body` do que a `pod2_body`.

>[!TIP]
>
>Consulte [Prompts estruturados](/help/user-guide/effective-prompts.md#structured-prompts) para saber como criar um prompt que gera conteúdo variável para cada seção em um email de várias seções.

## Visualização do modelo

Quando você [carrega um modelo](use-templates.md#upload-a-template), o GenStudio for Performance Marketing verifica o arquivo HTML em busca de campos reconhecidos. Use a visualização para revisar seus [elementos do modelo](use-templates.md#template-elements) e confirmar se você os identificou corretamente com os [nomes de campo reconhecidos](#recognized-field-names).

Exemplo de visualização para um modelo de email:

![Campos de visualização detectados](/help/assets/template-detected-fields.png "Verificar campos detectados"){zoomable="yes"}

Consulte [Editor de código de modelo](/help/user-guide/templates/code-editor.md).

### Visualização do controle

Você pode controlar a visibilidade de conteúdo especial usando Auxiliares Internos (expressões especiais na linguagem de modelo [!DNL Handlebars] que executam determinadas ações). Por exemplo, é possível adicionar uma declaração condicional que adicione parâmetros de rastreamento aos links no modelo exportado, mantendo os links de visualização limpos.

O valor `_genStudio.canvas` é definido ao renderizar um modelo, e o valor `genStudio.export` é definido ao exportar um modelo. Você pode decidir incluir determinado conteúdo na parte superior de um email usando um invólucro condicional, por exemplo, quando o modelo for usado para exportação:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Outro exemplo pode ser impedir o uso de códigos de rastreamento ao visualizar um modelo no GenStudio for Performance Marketing. O exemplo a seguir mostra como adicionar parâmetros de rastreamento a links no modelo exportado, mantendo os links de visualização limpos:

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Conteúdo estático

Os modelos de email e Meta geralmente vinculam-se a imagens e arquivos CSS hospedados em outros domínios. Quando o GenStudio for Performance Marketing gera miniaturas para visualizações de modelo ou as experiências derivadas delas, ele valida a fonte de conteúdo e incorpora uma cópia para fins de visualização.

Os arquivos externos são temporariamente incorporados apenas para criar a pré-visualização do modelo, o que garante que a pré-visualização reflita com precisão o conteúdo conforme ele aparece no momento da criação. Estes arquivos externos **não** são armazenados permanentemente no GenStudio for Performance Marketing. Após a criação da pré-visualização do modelo, o GenStudio for Performance Marketing continua fazendo referência ao link de origem original fornecido no modelo.

### Atualizar conteúdo

Se a origem for alterada após a criação da visualização inicial, use a função [atualizar](/help/user-guide/templates/use-templates.md#refresh-template) para atualizar a visualização do modelo com a versão mais recente do conteúdo das fontes externas.
