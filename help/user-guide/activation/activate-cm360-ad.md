---
title: Ativar um anúncio do Google Campaign Manager 360
description: Saiba como ativar uma experiência do Google Campaign Manager 360.
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# Ativar um anúncio do Google Campaign Manager 360

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios para o Google Campaign Manager 360.

**Formatos com suporte**: Exibição Estática, Exibição de Vídeo, Exibição de Zip HTML5.

A ativação de um anúncio do Google Campaign Manager 360 segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página abrange os pré-requisitos e campos de configuração específicos do Google Campaign Manager 360. Depois de ativar uma experiência no GenStudio for Performance Marketing, use o Google Campaign Manager 360 para analisar a experiência e iniciar o anúncio.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Uma conta do Google Campaign Manager 360 com acesso ao anunciante do target.
* Acesso de administrador ao anunciante, para ler e gravar no Campaign Manager 360.

O Campaign Manager 360 organiza campanhas e anúncios em anunciantes diferentes e cada anunciante inclui uma biblioteca criativa. O anunciante do target já deve existir no Campaign Manager 360; o GenStudio for Performance Marketing publica experiências de anúncios na biblioteca criativa desse anunciante, mas não cria anúncios.

## Conectar sua conta do Google Campaign Manager 360

Para que sua organização possa publicar ativos em uma biblioteca criativa, um gerente de sistema ou editor do GenStudio deve conectar sua conta do Google Campaign Manager 360 à GenStudio for Performance Marketing. Você deve ter acesso de administrador ao anunciante para ler e gravar no Campaign Manager 360. Consulte [Conectar contas de mídia paga](/help/user-guide/connectors/connect-channel.md).

Depois que a sincronização for concluída, você poderá visualizar as contas adicionadas.

## Campos de configuração do Google Campaign Manager 360

Os ativos aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: ID de rastreamento (usada como o nome criativo da plataforma)
* **Campos de configuração da plataforma**: anunciante

Sua experiência criativa é entregue à biblioteca criativa do anunciante selecionado no Google Campaign Manager 360 quando a ativação é concluída.
