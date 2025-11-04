---
title: Diretrizes para modelos de anúncio de exibição
description: Siga as práticas recomendadas ao usar modelos de anúncio de exibição e banner com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: 85cc8ee51bd6b934811583dc0a8460d6d7083a70
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

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

Consulte [Espaços reservados para conteúdo](/help/user-guide/content/customize-template.md#content-placeholders) para entender mais sobre o uso de nomes de campo em modelos.

## Dimensões suportadas

A Largura x Altura (pixels) deve ser definida.

| Orientação | Dimensões (pixels) | Notas |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical | 300 x 600<br>160 x 600 | Comum a banners de meia página e arranha-céus. |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Quadro de classificação padrão, retângulo médio e tamanhos de banner. |
| Personalizado | 50 x 50 a 2000 x 2000 | Use para disposições não padrão ou exclusivas; verifique os limites da plataforma. |

