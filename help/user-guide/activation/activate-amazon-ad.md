---
title: Ativar anúncios do Amazon
description: Saiba como ativar experiências de anúncios do Amazon.
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# Ativar anúncios do Amazon

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios para o Amazon Ads.

**Formatos com suporte**: exibição estática.

A ativação de uma experiência do Amazon Ads segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página abrange os pré-requisitos e campos de configuração específicos do Amazon Ads. Depois de ativar uma experiência no GenStudio for Performance Marketing, use o Amazon Ads para analisar a experiência e iniciar o anúncio.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Acesso à conta do Amazon Ads de destino.
* Acesso de administrador a essa conta para ler e gravar no Amazon Ads.

O Amazon Ads organiza campanhas e anúncios em diferentes contas, e cada conta inclui uma biblioteca criativa. A conta de destino já deve existir no Amazon Ads; o GenStudio for Performance Marketing publica experiências de anúncios na biblioteca criativa dessa conta, mas não cria contas.

## Conectar sua conta do Amazon Ads

Para que sua organização possa publicar ativos em uma biblioteca criativa, um gerente de sistema da GenStudio deve conectar sua conta do Amazon Ads à GenStudio for Performance Marketing. É necessário ter acesso de administrador a essa conta para ler e gravar no Amazon Ads. Consulte [Conectar contas de mídia paga](/help/user-guide/connectors/connect-channel.md).

Depois que a sincronização for concluída, você poderá visualizar as contas adicionadas.

## Campos de configuração do Amazon Ads

Os ativos aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: ID de rastreamento (usada como o nome criativo da plataforma)
* **Campos de configuração da plataforma**: conta

Sua experiência criativa é entregue à biblioteca criativa da conta selecionada no Amazon Ads quando a ativação é concluída.
