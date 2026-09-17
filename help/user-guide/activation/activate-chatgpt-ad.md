---
title: Ativar um anúncio de ChatGPT
description: Saiba como ativar uma experiência de anúncio no ChatGPT.
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
source-wordcount: '272'
ht-degree: 0%
---
# Ativar um anúncio de ChatGPT

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios ChatGPT.

**Formatos com suporte**: Cartões de Chat.

Você pode [criar uma experiência de ChatGPT](/help/user-guide/create/create-chatgpt-ad.md) no GenStudio for Performance Marketing e depois selecioná-la para ativação.

A ativação de um anúncio ChatGPT segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página aborda os pré-requisitos e campos de configuração específicos do ChatGPT. Depois de ativar uma experiência de ChatGPT no GenStudio for Performance Marketing, use o OpenAI Ads Manager para executar as verificações finais e iniciar o anúncio.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Uma conta do OpenAI Ads e uma chave de API dessa conta.
* A campanha e o grupo de publicidade de destino do ChatGPT já devem existir no Gerenciador de anúncios OpenAI. A GenStudio for Performance Marketing não cria novas campanhas ou grupos de anúncios.

## Conectar sua conta do ChatGPT

Antes que sua organização possa ativar experiências, um gerente de sistema da GenStudio deve conectar sua conta do OpenAI Ads à GenStudio for Performance Marketing:

1. No OpenAI Ads Manager, vá para **[!UICONTROL Configurações]** > **[!UICONTROL Chaves de API]** > **[!UICONTROL Criar nova chave]**.
1. No GenStudio for Performance Marketing, vá para **[!UICONTROL Mais]** > **[!UICONTROL Configurações]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Conectar]** > **[!UICONTROL Adicionar Conta]**.
1. Insira o nome da sua conta do OpenAI Ads, cole sua chave de API e clique em **[!UICONTROL Adicionar conta]**.

## Campos de configuração do ChatGPT

Os ativos, títulos (Título) e cópia do corpo aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: URL de Destino, ID de Rastreamento (usado como nome de anúncio da plataforma)
* **Campos de configuração de plataforma**: conta de anúncios OpenAI, campanha OpenAI, grupo de anúncios OpenAI

A URL de destino deve usar um formato `https://` válido, por exemplo `https://www.example.com`.
