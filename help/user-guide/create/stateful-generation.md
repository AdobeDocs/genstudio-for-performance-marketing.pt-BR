---
title: Gerar e refinar conteúdo com geração com monitoração de estado
description: Saiba como gerar conteúdo sobre a marca e refiná-lo alternadamente em uma conversa com impressão de voz e dicas visuais em [!DNL GenStudio for Performance Marketing].
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# Gerar e refinar conteúdo com a geração stateful

O [!DNL GenStudio for Performance Marketing] usa a Geração de estado para ajudá-lo a criar conteúdo sobre a marca e, em seguida, refiná-lo girando em uma conversa, em vez de começar novamente com um novo prompt a cada vez. À medida que você refina, a geração se lembra das instruções anteriores e das variantes mantidas e aplica somente a alteração solicitada.

A geração de estado adiciona três tipos de contexto às suas gerações: a impressão de voz mantém a cópia na voz da sua marca, dicas visuais em uma imagem ou vídeo e um URL de página da Web adiciona o contexto de referência de uma página escolhida.

## Gerar e refinar conteúdo

1. No [!DNL GenStudio for Performance Marketing], inicie uma geração para seu canal e formato. Consulte a [[!DNL Create] visão geral](/help/user-guide/create/overview.md) para iniciar uma geração para cada canal.
1. _Opcional_: para aterrar a cópia em seu próprio criativo, selecione **[!UICONTROL Selecionar do Conteúdo]** e escolha uma imagem ou vídeo para usar como uma [dica visual](#ground-content-in-an-image-or-video).
1. Selecione **[!UICONTROL Gerar]**. O [!DNL GenStudio for Performance Marketing] cria um conjunto de variantes e aplica a [voz da marca](#keep-copy-in-your-brand-voice) automaticamente nos canais com suporte.
1. Refine os resultados na gaveta do prompt. Digite a alteração desejada, como `shorten the headline`, `make variant 2 punchier` ou `change the headline`. A geração aplica somente essa alteração e mantém as instruções anteriores.
1. Para manter uma variante enquanto continua refinando, digite uma instrução na gaveta do prompt, como `keep variant 2`.
1. Quando o conteúdo estiver pronto, exporte-o ou envie-o para revisão.

## Aterrar conteúdo em uma imagem ou vídeo

As dicas visuais permitem que a geração leia uma imagem ou vídeo que você anexa e, em seguida, escreva uma cópia que reflita esse criativo. A opção **[!UICONTROL Creative]** controla dicas visuais e está ativada por padrão.

Para usar uma dica visual, selecione **[!UICONTROL Selecionar do conteúdo]** e escolha uma imagem ou vídeo antes de gerar. Para gerar sem uma dica visual, desative as **[!UICONTROL opções do Creative]**.

>[!NOTE]
>As dicas visuais não estão disponíveis para anúncios de exibição de vários quadros ou anúncios no carrossel.

## Manter cópia na voz da sua marca

A impressão de voz aplica a voz aprendida de sua marca à cópia gerada, para que soe na marca sem solicitação extra. Está ativada por padrão para canais que têm [Insights](/help/user-guide/insights/overview.md), como LinkedIn e Meta.

## Usar uma página da Web como contexto

Você pode apontar a geração para uma página da Web e usar seu conteúdo como contexto. Na gaveta do prompt, digite uma instrução que inclua a URL, como `Use this URL to generate an ad for this channel: https://www.example.com`.

>[!NOTE]
>Digite o URL no prompt. Não o adicione através de _Parâmetros_.

## Recursos relacionados

- [Gerenciar variantes](/help/user-guide/create/manage-variants.md): edite e ajuste as variantes geradas diretamente na Tela.
- [Gravar prompts efetivos](/help/user-guide/effective-prompts.md): prompts de artesanato que produzem melhores resultados.
