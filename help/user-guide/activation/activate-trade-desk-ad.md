---
title: Ativar um anúncio para a Trade Desk
description: Saiba como ativar uma experiência de anúncio de exibição estática para a Trade Desk.
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
source-wordcount: '461'
ht-degree: 0%
---
# Ativar um anúncio para a Trade Desk

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios para a Trade Desk.

**Formatos com suporte**: exibição estática (somente ativo único).

A ativação de um anúncio para a Trade Desk segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação para outros canais de anúncios pagos, com uma diferença. A Trade Desk é um serviço corporativo gerenciado, não uma plataforma de anúncios de autoatendimento, portanto, o acesso à conta funciona de forma diferente dos outros canais. Essa página aborda essas diferenças, juntamente com os pré-requisitos e campos de configuração específicos da Trade Desk.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Pré-requisitos

* Uma conta existente do Trade Desk em tempo real. Configure diretamente com a Trade Desk antes de conectá-la ao GenStudio for Performance Marketing.
* Acesso à API habilitado pela equipe de conta da Trade Desk. Para a Trade Desk, a equipe de conta ativa esse acesso em seu nome usando um token de API, em vez do logon OAuth usado por outros canais de anúncios pagos.
* O anunciante, a vaga e as permissões corretas habilitadas pela Trade Desk para a integração com o GenStudio for Performance Marketing.
* Um token de API ou credenciais da equipe de conta da Trade Desk, com permissões para publicar criações na conta de anunciante de destino.
* Uma campanha de destino que já existe na Trade Desk. O GenStudio for Performance Marketing ativa anúncios nessa campanha existente.

## Conectar sua conta da Trade Desk

Antes que sua organização possa ativar experiências, trabalhe com sua equipe de conta da Trade Desk para habilitar o acesso à API e, em seguida, um gerente de sistema da GenStudio conectará a conta à GenStudio for Performance Marketing:

1. Entre em contato com a equipe de conta da Trade Desk e solicite acesso para publicar criações do GenStudio for Performance Marketing na conta da Trade Desk. Confirme a ID do anunciante, a vaga ou os detalhes do parceiro que serão usados para ativação.
1. Obtenha o token da API ou as credenciais da equipe de conta da Trade Desk e confirme se o token oferece suporte a permissões de publicação criativa para a conta de anunciante de destino.
1. No GenStudio for Performance Marketing, vá para **[!UICONTROL Configurações]** > **[!UICONTROL Canais]** e clique em **[!UICONTROL Conectar]** no bloco **[!UICONTROL Trade Desk]**. Insira o Nome da conta, a ID do anunciante e o token ou as credenciais da API e salve a conexão.

Se a conexão falhar, confirme com sua equipe de conta da The Trade Desk se o acesso à API foi ativado e se o token tem o anunciante correto e as permissões de assento.

## Os campos de configuração da Trade Desk

Os ativos aprovados estão bloqueados e não podem ser editados durante a ativação, pois já passaram por revisão e aprovação em [!DNL Content]. É possível editar:

* **Campos de texto**: ID de rastreamento (usada como o nome criativo da plataforma)
* **Campos de configuração da plataforma**: Conta, Campanha

No momento, a ativação para a Trade Desk suporta apenas anúncios de exibição estáticos de ativo único.
