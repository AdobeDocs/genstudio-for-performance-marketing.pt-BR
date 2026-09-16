---
title: Ativar um anúncio do Meta
description: Saiba como ativar uma experiência de anúncio do Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
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
source-wordcount: '382'
ht-degree: 0%
---
# Ativar um anúncio do Meta

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios do Meta para o Instagram e o Facebook.

**Formatos com suporte**: Imagem, Vídeo, Carrossel.

[Crie uma experiência do Meta](/help/user-guide/create/create-meta-ad.md) no GenStudio for Performance Marketing e selecione-a para ativação.

A ativação de um anúncio Meta segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página abrange os pré-requisitos e campos de configuração específicos do Meta. Depois de ativar uma experiência do Meta no GenStudio for Performance Marketing, use o [Meta Ads Manager](https://adsmanager.facebook.com/) para revisar a experiência e iniciar o anúncio.

Diferente de alguns outros canais, um anúncio de Meta pode incluir várias taxas de aspecto em um único anúncio. Se a sua experiência tiver várias taxas de proporção, [!DNL Activate] ainda gerará apenas uma linha para ela, não uma linha por taxa de proporção.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

Confirme se suas contas de anúncio conectadas do Meta têm permissão total para gerenciar anúncios nestes componentes da plataforma de publicidade da Meta:

* Conta de anúncio do Meta
* Página do Facebook
* Campanha do Meta
* Conjunto de anúncios do Meta
* Perfil do Instagram (opcional)

A campanha e o conjunto de anúncios do Meta de destino já devem existir no Meta Ads Manager. Atualmente, a GenStudio for Performance Marketing não cria campanhas ou conjuntos de anúncios.

## Conectar suas contas do Meta

Antes que sua organização possa ativar experiências, um gerente de sistema da GenStudio deve conectar suas contas da Meta à GenStudio for Performance Marketing. Essa conexão permite que os dados fluam entre o GenStudio for Performance Marketing e o Meta, habilitando o processo de ativação. Consulte [Conectar-se ao Meta Ads](/help/user-guide/connectors/meta-ads.md).

Para selecionar uma conta do Instagram, verifique no Meta Business Manager se [a conta do Instagram que deseja usar está conectada à mesma conta de anúncio](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account) selecionada durante a integração. Se essa conexão estiver ausente, a conta do Instagram pode não aparecer no menu suspenso **[!UICONTROL Perfil do Instagram]** durante a ativação.

Depois que a sincronização for concluída, você poderá visualizar as contas adicionadas. Grandes quantidades de dados levam mais tempo para sincronizar.

## campos de configuração do Meta

Os ativos, títulos e cópia do corpo aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: Descrição, Call-to-action, URL de destino, Parâmetros de URL, ID de rastreamento (usado como o nome do anúncio do Meta)
* **Campos de configuração da plataforma**: conta de anúncio, página do Facebook, perfil do Instagram, campanha do Meta, conjunto de anúncios do Meta
