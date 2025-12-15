---
title: Diretrizes do modelo do LinkedIn
description: Siga as práticas recomendadas ao usar modelos do LinkedIn com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: ff694925dea4741d13ae71a68e23a5e604134521
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 1%

---

# Diretrizes de modelo do LinkedIn

Os templates do LinkedIn fornecem uma maneira estruturada de criar e personalizar anúncios criativos para campanhas do LinkedIn. Essas diretrizes garantem que seus anúncios atendam às especificações do LinkedIn e, ao mesmo tempo, simplifiquem o processo criativo no GenStudio for Performance Marketing. Este guia ajuda você a se preparar para uma promoção de marca consistente e um desempenho eficiente nas plataformas móveis e de desktop do LinkedIn.

Siga estas práticas recomendadas de design ao personalizar modelos de anúncios do LinkedIn para funcionar com o GenStudio for Performance Marketing:

- É necessário exatamente um campo de imagem
- Tamanho máximo de imagem de 5 MB
- Máximo de 70 caracteres no título
- Texto introdutório com no máximo 150 caracteres
- Somente uma seção pode ser usada, gerando um único conjunto de elementos de modelo

## Nomes de campo reconhecidos

Ao personalizar seu modelo do LinkedIn, aplique espaços reservados para o conteúdo para estes campos obrigatórios:

- `image` (obrigatório, selecionado no JPEG de conteúdo, PNG ou GIF)
- `on_image_text` (texto que aparece sobre a imagem)

O GenStudio for Performance Marketing gera automaticamente os campos a seguir. Não é necessário aplicar espaços reservados para conteúdo para:

- `headline`
- `introductory_text`
- `cta` (Call to action)

Consulte [Espaços reservados para conteúdo](/help/user-guide/templates/customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

## Taxas de proporção suportadas

Todas as larguras dos modelos do LinkedIn são codificadas em 1200 pixels.

| Taxa de proporção | Platform | Dimensões (px) | Notas |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| Quadrado 1:1 | Desktop, móvel | 1200 x 1200 | Mais versátil. Ideal para aparência consistente em dispositivos e inserções. |
| Horizontal 1.91:1 | Desktop | 1200 x 628 | Formato paisagem padrão. Geralmente usado para conteúdo patrocinado e anúncios de feed de notícias. |
| Vertical 1:1.91 | Dispositivos móveis | 1200 x 2292 | Formato vertical alto. Otimizado para visualização móvel, oferecendo mais presença na tela. |
| Vertical 2:3 | Dispositivos móveis | 1200 x 1800 | Um pouco menos alto que 1:1.91. Bom para campanhas iniciadas por dispositivos móveis. |
| Vertical 4:5 | Dispositivos móveis | 1200 x 1500 | Recomendado para dispositivos móveis. Equilibra visibilidade e conteúdo, o que geralmente resulta em maior impacto. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
