---
title: Ativar um anúncio innovid
description: Saiba como ativar uma experiência Innovid.
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# Ativar um anúncio innovid

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios para o Innovid.

**Formatos com suporte**: Exibição Estática, Exibição com Zip HTML5.

A ativação de uma experiência Innovid segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página aborda os pré-requisitos e campos de configuração específicos do Innovid. Depois de ativar uma experiência no GenStudio for Performance Marketing, use o Innovid para revisar a experiência e iniciar o anúncio.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Acesso à conta do Target Innovid.
* Acesso de administrador a essa conta para ler e gravar no Innovid.

O Innovid organiza campanhas e anúncios em diferentes contas, e cada conta tem uma biblioteca criativa. A biblioteca criativa de destino já deve existir no Innovid; o GenStudio for Performance Marketing publica experiências de anúncio nessa biblioteca criativa, mas não cria contas ou bibliotecas criativas.

## Conectar sua conta do Innovid

Para que sua organização possa publicar ativos em uma biblioteca criativa, um gerente de sistema da GenStudio deve conectar sua conta da Innovid à GenStudio for Performance Marketing. Você deve ter acesso de administrador a essa conta para ler e gravar no Innovid. Consulte [Conectar contas de mídia paga](/help/user-guide/connectors/connect-channel.md).

Depois que a sincronização for concluída, você poderá visualizar as contas adicionadas.

## Campos de configuração innovid

Os ativos aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: ID de rastreamento (usada como o nome criativo da plataforma)
* **Campos de configuração da plataforma**: conta, biblioteca Creative, nome do conceito

Sua experiência criativa é entregue à biblioteca criativa selecionada no Innovid quando a ativação é concluída.
