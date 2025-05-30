---
title: Diretrizes do modelo de metadados
description: Siga as práticas recomendadas ao usar modelos de meta anúncios com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Diretrizes do modelo de metadados

Os modelos de meta anúncios ajudam você a criar anúncios visualmente consistentes e eficazes nas plataformas Meta. Seguindo as práticas de design recomendadas e usando campos compatíveis, é possível garantir que seus modelos sejam otimizados para o GenStudio for Performance Marketing. Este guia explica como estruturar, personalizar e preparar modelos de metadados para integração perfeita e resultados de alto impacto.

Siga estas práticas recomendadas de design ao personalizar modelos de metadados para funcionar com o GenStudio for Performance Marketing:

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

Ao personalizar o modelo de Metadados, aplique espaços reservados para o conteúdo dos seguintes campos obrigatórios:

- `image` (obrigatório, selecionado no JPEG de conteúdo, PNG ou GIF)
- `on_image_text` (texto que aparece sobre a imagem)

O GenStudio for Performance Marketing gera automaticamente os campos a seguir. Não é necessário aplicar espaços reservados para conteúdo para:

- `headline`
- `body`
- `cta`

Consulte [Espaços reservados para conteúdo](/help/user-guide/content/customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

## Taxas de proporção suportadas

| Taxa de proporção | Dimensões (pixels) | Notas |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Quadrado 1:1 | 1080 x 1080 | Padrão para a maioria dos posicionamentos de meta; recomendado para maior compatibilidade. |
| Retrato 4:5 | 1080 x 1350 | Otimizado para feeds para dispositivos móveis; fornece mais espaço vertical. |
| História 9:16 | 1080 x 1920 | Ideal para histórias e bobinas; preenche toda a tela móvel. |
| Paisagem 1.91:1 | 1080 x 566 | Melhor para anúncios em links e posicionamentos de Feed de notícias; formato amplo. |
| Personalizado | Mínimo 50 x 50 (largura) | Use somente se necessário; pode resultar em corte ou dimensionamento. |

Se o anúncio não for projetado em uma dessas taxas de aspecto, a GenStudio for Performance Marketing corta automaticamente a imagem no tamanho apropriado.

## Exemplo de modelo

+++Exemplo: modelo de metadados

<!-- Does this need to be a precise size? -->

Este é um exemplo básico de um modelo de Meta-anúncio. O cabeçalho contém CSS em linha para estilo. O corpo usa [espaços reservados para conteúdo](#content-placeholders), como `image` e `on_image_text`, para indicar onde o GenStudio for Performance Marketing pode gerar conteúdo.

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
