---
title: Conectar mídia paga
description: Conecte uma conta de canal para ativar e monitorar seus anúncios e mídia com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: cf4be61925761c9630cb8ea5c995d017b3938a31
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Conectar contas de mídia paga

O _[!DNL Data connectors]_&#x200B;habilita a integração perfeita entre o GenStudio for Performance Marketing e suas contas de rede de mídia paga. Conectando-se a contas de canal de terceiros, você pode trocar dados críticos, como métricas de desempenho de campanha no [[!DNL Insights]](/help/user-guide/insights/overview.md), e pode fornecer novos posicionamentos de anúncios com o [[!DNL Activate]](/help/user-guide/activation/overview.md). Essa integração permite que o GenStudio for Performance Marketing gerencie suas mídias e anúncios enquanto recebe insights valiosos, incluindo impressões, cliques e conversões, de suas campanhas ativas.

**Para se conectar a uma conta de mídia paga**:

1. Clique nas reticências **[!UICONTROL ... Mais]** na navegação inferior esquerda.

1. Selecione **[!UICONTROL Configurações]** com o ícone cog.

1. Em _[!UICONTROL Configurações]_, escolha um tipo de conector na seção _[!UICONTROL Conectores de dados]_ e clique em **[!UICONTROL Conectar]**.

   Opcionalmente, se houver contas conectadas, você pode clicar em _contas conectadas_ para exibir uma lista de nomes de contas, detalhes e status.

1. Veja o [tipo de conector](#connector-types) selecionado, revise os pré-requisitos e continue com as etapas de conexão.

## Conexões de mídia paga

O GenStudio for Performance Marketing oferece suporte a vários tipos de conectores para integração com suas plataformas de marketing preferidas. Cada tipo de conector tem pré-requisitos específicos e etapas de configuração a serem concluídas para uma conexão bem-sucedida.

### Conexão com o Google Campaign Manager 360

>[!BEGINSHADEBOX]

**Pré-requisitos**:

- Conta do Google Campaign Manager 360
- Remova os bloqueadores de pop-up do navegador

>[!ENDSHADEBOX]

**Para conectar uma conta do Google Campaign Manager 360**:

1. Na seção _Data connectors_, clique em **[!UICONTROL Connect]** no cartão _Google Campaign Manager 360_.

1. Faça logon na sua conta do Google Campaign Manager 360.

   Talvez seja necessário remover os bloqueadores de pop-ups e usar **[!UICONTROL Atualizar]** para tentar novamente.

1. Leia os termos e condições e clique em **[!UICONTROL Permitir]** para conceder acesso.

1. Na exibição _[!UICONTROL Google Campaign Manager 360]_, selecione um ou mais anunciantes e clique em **[!UICONTROL Selecionar]**.

A exibição _[!UICONTROL contas do Google Campaign Manager 360]_ lista o `Account name`, `Added by`, `Date added` e `Status`. Use **[!UICONTROL Adicionar conta]** para adicionar mais contas à lista.

### Metadados conectados

Quando você conecta seu perfil do _Meta Business_ à GenStudio for Performance Marketing, ele garante um acesso perfeito aos dados de publicidade de suas páginas de negócios, contas de Meta Ads e outros ativos do Meta.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

- Logon no Facebook/Meta que pode acessar todos os serviços Meta, como a conta Meta Ads e o Perfil comercial do Facebook
- Acesso à conta de Metadados com nível de permissão `View performance` para acessar relatórios e exibir anúncios, incluindo os seguintes
   - Permissões necessárias para uso com [!DNL Insights]:

      - `pages_show_list`
      - `ads_read`
      - `ads_management`
      - `pages_read_engagement`

   - Permissões necessárias para uso com [!DNL Activate]:

      - `ads_management`
      - `ads_read`
      - `business_management`
      - `instagram_basic`
      - `instagram_content_publish`
      - `pages_manage_ads`
      - `pages_manage_posts`
      - `pages_show_list`

- Remova os bloqueadores de pop-up do navegador

>[!ENDSHADEBOX]

**Para conectar uma conta de Metadados**:

1. Na seção _Data connectors_, clique em **[!UICONTROL Connect]** no cartão _Meta Ads_.

1. Faça logon em sua conta do Facebook.

   Talvez seja necessário remover os bloqueadores de pop-ups e usar **[!UICONTROL Atualizar]** para tentar novamente.

1. Siga as instruções de autenticação do Facebook, verifique as informações da conta e clique em **[!UICONTROL Continuar como...]**

1. Em _[!UICONTROL Logon do Facebook para Empresas]_ (símbolo de Meta para Adobe), passe pelas seguintes seleções para conceder acesso ao GenStudio for Performance Marketing:

   - Selecione um ou mais perfis da Meta Business e clique em **[!UICONTROL Continuar]**
   - Selecione uma ou mais metapáginas e clique em **[!UICONTROL Continuar]**
   - Selecione uma ou mais contas do Instagram e clique em **[!UICONTROL Continuar]**
   - Revise as seleções e clique em **[!UICONTROL Salvar]**

1. Depois de receber a verificação de que sua conta está conectada, clique em **[!UICONTROL Obteve]**.

   Essa etapa garante que o GenStudio for Performance Marketing tenha acesso a todos os anúncios, metadados e métricas para obter o desempenho ideal.

1. Em _[!UICONTROL Meta Ads]_, selecione uma ou mais contas a serem incluídas em [!DNL Insights] e clique em **[!UICONTROL Selecionar]**.

1. Depois de receber uma confirmação de _Plataforma conectada_, clique em **[!UICONTROL Exibir contas]**.

   A exibição das _[!UICONTROL Contas de meta anúncios]_ lista as `Account name`, `Added by`, `Date added` e `Status`.

Use **[!UICONTROL Adicionar conta]** para adicionar mais contas à lista. O fluxo de autorização pode ser um pouco diferente quando você adiciona contas vinculadas ao mesmo perfil de Meta Business. Você seleciona somente as novas contas de Meta Ads durante o processo de conexão.

## Assimilação de dados

Inicialmente, o GenStudio for Performance Marketing importa os seis meses mais recentes de dados históricos. Essa prática garante acesso imediato a insights relevantes para analisar tendências, avaliar desempenho e tomar decisões informadas. O processo de assimilação pode levar de um a cinco dias, dependendo do volume de dados na sua conta.

>[!BEGINSHADEBOX]

**Política de assimilação e retenção de dados**

O GenStudio for Performance Marketing retém os dados do canal por 13 meses. Essa política de retenção inclui os seis meses de dados assimilados durante a conexão inicial, garantindo uma análise e relatórios abrangentes de dados históricos.

>[!ENDSHADEBOX]
