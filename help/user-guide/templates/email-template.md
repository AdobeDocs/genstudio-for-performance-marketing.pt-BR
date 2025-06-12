---
title: Diretrizes do modelo de email
description: Siga as práticas recomendadas ao usar modelos de email com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 4760da26d20e91489a74bb238e07f0d3b426c0a1
workflow-type: tm+mt
source-wordcount: '416'
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

Ao personalizar seu modelo de email, use espaços reservados para o conteúdo para os seguintes campos obrigatórios:

- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selecionado no JPEG de conteúdo, PNG ou GIF)

O GenStudio for Performance Marketing gera automaticamente os campos a seguir. Rich text não está habilitado. Não é necessário aplicar espaços reservados para conteúdo para:

- `pre_header`
- `subject`

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

Este é um exemplo básico de um template de email do HTML com uma seção. O `<head>` inclui CSS simples embutido para estilo, e o `<body>` usa espaços reservados para conteúdo como `pre_header`, `headline`, `sub_headline`, `body`, `cta` e `image` com link e. Esses espaços reservados permitem que o GenStudio for Performance Marketing insira conteúdo dinâmico durante a geração de email.

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Marketing Email</title>
        <style>
            .container {
                width: 100%;
                padding: 20px;
                font-family: Arial, sans-serif;
            }
            .cta-button {
                display: inline-block;
                background-color: #fff;
                color: #000;
                border: 2px solid #000;
                padding: 10px 20px;
                text-decoration: none;
                font-family: 'Source Sans Pro', Arial, sans-serif;
                font-weight: 600;
                font-size: 14px;
                margin-top: 20px;
                text-align: center;
            }
        </style>
    </head>
    <body>
        <div class="container">
            {{pre_header}}
            <h1>{{headline}}</h1>
            <p>
                <a href="{{link}}">
                    <img alt="banner headline" src="{{image}}" width="600" height="600">
                </a>
            </p>
            <h2>{{sub_headline}}</h2>
            <p>{{body}}</p>
            <a href="#" class="cta-button">{{cta}}</a>
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
            .cta-button {
            display: inline-block;
            background-color: #fff; /* Background color to white */
            color: #000; /* Text color to black */
            border: 2px solid #000; /* Border color to black */
            padding: 10px 20px;
            text-decoration: none;            
            font-family: 'Source Sans Pro', Arial, sans-serif;
            font-weight: 600; /* Semibold */
            font-size: 14px;
            margin-top: 20px;
            text-align: center;
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
                <p><img alt="pic1" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="pic2" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
            <a href="#" class="cta-button">{{cta}}</a>
        </div>
    </body>
</html>
```

+++
