---
title: Diretrizes para modelos de anúncio do Meta
description: Siga as práticas recomendadas ao usar modelos de anúncios do Meta com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
TQID: https://experienceleague.adobe.com/-WHH1xjWFaizXTKjuF-K9UtaR12V3QpMezSqRfwbMIU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 1%

---

# Diretrizes do modelo de anúncio do Meta

Os modelos de anúncios do Meta ajudam você a criar anúncios visualmente consistentes e eficazes nas plataformas do Meta. Seguindo as práticas de design recomendadas e usando campos compatíveis, é possível garantir que seus modelos sejam otimizados para o GenStudio for Performance Marketing. Este guia explica como estruturar, personalizar e preparar modelos de anúncios do Meta para integração perfeita e resultados de alto impacto.

Siga estas práticas recomendadas de design ao personalizar modelos de anúncios do Meta para funcionar com o GenStudio for Performance Marketing:

- Usar largura de 360 pixels para layouts de coluna
- Use uma resolução mínima de 1080 x 1080 pixels para imagens
- É necessário exatamente um campo de imagem
- **não** usar tamanho de fonte relativo
- Fazer **não** definir viewport
- **não** usar o JavaScript
- **não** substitua um elemento HTML no CSS
- Usar a marca `<img>` em vez de `background-image`
- Usar o mascaramento para melhorar a legibilidade do texto em imagens de plano de fundo
- Somente uma seção pode ser usada, gerando um único conjunto de elementos de modelo

## Nomes de campo reconhecidos

Ao personalizar o modelo de anúncios do Meta, aplique espaços reservados para o conteúdo dos seguintes campos obrigatórios:

- `image` (obrigatório, selecionado no JPEG de conteúdo, PNG ou GIF)
- `on_image_text` (texto que aparece sobre a imagem)

O GenStudio for Performance Marketing gera automaticamente os campos a seguir. Não é necessário aplicar espaços reservados para conteúdo para:

- `headline`
- `body`
- `cta`

Consulte [Espaços reservados para conteúdo](/help/user-guide/templates/customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

## Taxas de proporção suportadas

| Taxa de proporção | Dimensões (pixels) | Notas |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Quadrado 1:1 | 1080 x 1080 | Padrão para a maioria das disposições do Meta; recomendado para maior compatibilidade. |
| Retrato 4:5 | 1080 x 1350 | Otimizado para feeds para dispositivos móveis; fornece mais espaço vertical. |
| História 9:16 | 1080 x 1920 | Ideal para histórias e bobinas; preenche toda a tela móvel. |
| Paisagem 1.91:1 | 1080 x 566 | Melhor para anúncios em links e posicionamentos de Feed de notícias; formato amplo. |
| Personalizado | Mínimo 50 x 50 (largura) | Use somente se necessário; pode resultar em corte ou dimensionamento. |

Se o anúncio não for projetado em uma dessas taxas de aspecto, a GenStudio for Performance Marketing corta automaticamente a imagem no tamanho apropriado.

## Exemplo de modelo

+++Exemplo: Meta ad template

<!-- Does this need to be a precise size? -->

Este é um exemplo básico de um modelo de anúncio do Meta. O cabeçalho contém CSS em linha para estilo. O corpo usa [espaços reservados para conteúdo](#content-placeholders), como `image` e `on_image_text`, para indicar onde o GenStudio for Performance Marketing pode gerar conteúdo.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
