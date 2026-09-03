---
title: Diretrizes para modelos de anúncio de exibição
description: Siga as práticas recomendadas ao usar modelos de anúncio de exibição e banner com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
TQID: https://experienceleague.adobe.com/HjkLWiyqK1quHoZB5lEE-qyB3zci12KlRAZC8ME-9Ao
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 1%

---

# Exibir diretrizes do modelo de anúncio

Os modelos de exibição são layouts pré-projetados usados para criar banners e anúncios de exibição visualmente envolventes. Elas fornecem uma estrutura flexível para incorporar imagens, texto e call to action, garantindo consistência e eficiência ao produzir várias variações de anúncios. Ao preparar seu modelo para uso no GenStudio for Performance Marketing, verifique se todos os ativos estão otimizados para exibição na Web e atendem aos formatos e tamanhos de arquivo necessários.

Siga estas práticas recomendadas de design ao personalizar modelos de Banner e Anúncio de exibição para funcionar com o GenStudio for Performance Marketing:

- Usar fontes do Adobe ou Google
- Prepare ativos que sejam bem exibidos em dimensões finas
- É necessário exatamente um campo de imagem
- **não** usar imagens de fundo inseridas ou codificadas
- Use imagens de plano de fundo (campo `image`) carregadas no repositório de conteúdo do GenStudio for Performance Marketing. Siga as diretrizes em [Carregando imagens para anúncios de exibição](#uploading-images-for-display-ads) para obter melhores resultados
- **não** usar o JavaScript
- Somente uma seção pode ser usada, gerando um único conjunto de elementos de modelo

## Nomes de campo reconhecidos

Ao personalizar seu banner ou modelo de anúncio de exibição, use espaços reservados para conteúdo para os seguintes campos obrigatórios:

- `headline`
- `sub_headline`
- `body`
- `image` (obrigatório, selecionado no JPEG de conteúdo, PNG ou GIF)

O GenStudio for Performance Marketing gera automaticamente os campos a seguir. Não é necessário aplicar espaços reservados para conteúdo para:

- `cta`

Consulte [Espaços reservados para conteúdo](/help/user-guide/templates/customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

## Dimensões suportadas

A Largura x Altura (pixels) deve ser definida.

| Orientação | Dimensões (pixels) | Notas |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical | 300 x 600<br>160 x 600 | Comum a banners de meia página e arranha-céus. |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Quadro de classificação padrão, retângulo médio e tamanhos de banner. |
| Personalizado | 50 x 50 a 2000 x 2000 | Use para disposições não padrão ou exclusivas; verifique os limites da plataforma. |

