---
title: Ativar um anúncio do LinkedIn
description: Saiba como ativar uma experiência de anúncio do LinkedIn.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# Ativar um anúncio do LinkedIn

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios do LinkedIn para o [Gerenciador de Campanhas do LinkedIn](https://business.linkedin.com/marketing-solutions).

**Formatos com suporte**: Imagem única, Vídeo único.

Você pode [criar uma experiência do LinkedIn](/help/user-guide/create/create-linkedin.md) no GenStudio for Performance Marketing e depois selecioná-la para ativação.

A ativação de um anúncio do LinkedIn segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais de anúncios pagos. Esta página abrange os pré-requisitos e campos de configuração específicos do LinkedIn. Depois de ativar uma experiência do LinkedIn no GenStudio for Performance Marketing, use o Gerenciador de campanhas do LinkedIn para analisar a experiência e iniciar o anúncio.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Uma conta do gerente de campanha do LinkedIn com permissão total para gerenciar campanhas e anúncios. Essa conta deve conter campanhas existentes.
* Contas de anúncio do LinkedIn com permissão total para criar anúncios e publicar conteúdo nas páginas do LinkedIn.

A campanha e o conjunto de anúncios do LinkedIn de destino já devem existir no Gerenciador de campanhas do LinkedIn. A GenStudio for Performance Marketing não cria campanhas ou conjuntos de anúncios.

>[!NOTE]
>
>O LinkedIn renomeou sua hierarquia de campanha: o que o LinkedIn Campaign Manager anteriormente chamava de **grupo de campanha** agora é chamado de **campanha**, e o que anteriormente chamava de **campanha** agora é chamado de **conjunto de anúncios**. Os campos de configuração **[!UICONTROL Campanha do LinkedIn]** e **[!UICONTROL Conjunto de anúncios do LinkedIn]** em [!DNL Activate] usam esta terminologia atual.

Atualmente, o GenStudio for Performance Marketing é compatível com anúncios do LinkedIn de Imagem única e Vídeo único, cada um com apenas uma imagem ou vídeo por publicação. Se a sua experiência incluir várias taxas de proporção, o [!DNL Activate] gerará uma linha separada por proporção na tabela de ativação para que cada uma possa ser executada como seu próprio anúncio. Exclua todas as linhas desnecessárias.

## Conectar suas contas do LinkedIn

Antes que sua organização possa ativar experiências, um gerente ou editor de sistema da GenStudio deve conectar suas contas de anúncios do LinkedIn à GenStudio for Performance Marketing. Você deve ter acesso de administrador total à conta de anúncio e à página de perfil do LinkedIn para se conectar com sucesso. Você só precisa conectar uma conta publicitária em **[!UICONTROL Configurações]** uma vez. Depois disso, ele estará disponível para qualquer pessoa que possa acessar essa instância.

Essa conexão permite que os dados fluam entre o GenStudio for Performance Marketing e o LinkedIn, habilitando o processo de ativação.

Depois que a sincronização for concluída, você poderá visualizar as contas adicionadas. Grandes quantidades de dados levam mais tempo para sincronizar.

## Campos de configuração do LinkedIn

Os ativos, as manchetes e o texto de introdução aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram pela revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: Descrição, Call-to-action, URL de destino, Parâmetros de URL, ID de rastreamento (usado como nome de anúncio da plataforma)
* **Campos de configuração da plataforma**: conta de anúncio do LinkedIn, campanha do LinkedIn, conjunto de anúncios do LinkedIn
