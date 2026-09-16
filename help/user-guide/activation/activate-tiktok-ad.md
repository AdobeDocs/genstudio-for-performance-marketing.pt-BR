---
title: Ativar um anúncio do TikTok
description: Saiba como ativar uma experiência de anúncio de vídeo no feed do TikTok.
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%
---
# Ativar um anúncio do TikTok

O Adobe GenStudio for Performance Marketing é compatível com a ativação de experiências de anúncios do TikTok.

**Formatos com suporte**: anúncios de vídeo no feed.

Você pode [criar uma experiência do TikTok](/help/user-guide/create/tiktok-experiences.md) no GenStudio for Performance Marketing e depois selecioná-la para ativação.

A ativação de um anúncio TikTok segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página abrange os pré-requisitos e campos de configuração específicos do TikTok. Depois de ativar uma experiência do TikTok no GenStudio for Performance Marketing, use o TikTok Ads Manager para executar as verificações finais e iniciar o anúncio.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Uma conta do TikTok Ads com acesso de Operador ou Administrador.
* Pelo menos uma conta de anúncio do TikTok habilitada para uso, conectada por um gerente de sistema ou editor do GenStudio.
* A campanha do TikTok de destino já deve existir no TikTok Ads Manager. O TikTok Ads Manager, não o GenStudio for Performance Marketing, define o orçamento, a oferta, a otimização e o direcionamento do grupo de anúncios.

## Conectar sua conta do TikTok

Antes que sua organização possa ativar experiências, um gerente de sistema da GenStudio deve conectar sua conta do TikTok Ads à GenStudio for Performance Marketing:

1. Vá para **[!UICONTROL Configurações]** > **[!UICONTROL TikTok]** > **[!UICONTROL Conectar]**.
1. Faça logon na conta do TikTok Ads Manager na janela que é aberta e conclua o logon no OAuth. Sua conta deve ter acesso de Operador ou Administrador à conta do anúncio.

Depois que a conexão for concluída, confirme se pelo menos uma conta de anúncio do TikTok está ativada para uso.

## campos de configuração do TikTok

Os ativos aprovados e o texto principal estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: Call-to-action, URL de destino, ID de rastreamento (usado como nome de anúncio da plataforma)
* **Campos de configuração da plataforma**: conta, campanha e grupo de anúncios do TikTok Ads
