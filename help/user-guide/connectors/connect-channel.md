---
title: Conectar mídia paga
description: Conecte uma conta de canal para ativar e monitorar seus anúncios e mídia com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: 2844914d25d9bc3a2be7f47d0cd7f26f7c921555
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# Conectar contas de mídia paga

O _[!DNL Data connectors]_habilita a integração perfeita entre o GenStudio for Performance Marketing e suas contas de rede de mídia paga. Conectando-se a contas de canal de terceiros, você pode trocar dados críticos, como métricas de desempenho de campanha no [[!DNL Insights]](/help/user-guide/insights/overview.md), e pode fornecer novos posicionamentos de anúncios com o [[!DNL Activate]](/help/user-guide/activation/overview.md). Essa integração permite que o GenStudio for Performance Marketing gerencie suas mídias e anúncios enquanto recebe insights valiosos, incluindo impressões, cliques e conversões, de suas campanhas ativas.

**Para se conectar a uma conta de mídia paga**:

1. Clique nas reticências **[!UICONTROL ... Mais]** na navegação inferior esquerda.

1. Selecione **[!UICONTROL Configurações]** com o ícone cog.

1. Em _[!UICONTROL Configurações]_, escolha um tipo de conector na seção _[!UICONTROL Conectores de dados]_ e clique em **[!UICONTROL Conectar]**.

   Opcionalmente, se houver contas conectadas, você pode clicar em _contas conectadas_ para exibir uma lista de nomes de contas, detalhes e status.

1. Veja o [tipo de conector](#connector-types) selecionado, revise os pré-requisitos e continue com as etapas de conexão.

## Conexões de mídia paga

O GenStudio for Performance Marketing oferece suporte a vários tipos de conectores para integração com suas plataformas de marketing preferidas. Cada tipo de conector tem pré-requisitos específicos e etapas de configuração a serem concluídas para uma conexão bem-sucedida.

### Metadados conectados

>[!BEGINSHADEBOX]

**Pré-requisitos**:

- Conta do Facebook/Meta ads
- Acesso à conta de Metadados com nível de permissão `View performance` para acessar relatórios e exibir anúncios
- Remova os bloqueadores de pop-up do navegador

>[!ENDSHADEBOX]

**Para conectar uma conta de Metadados**:

1. Na seção _Data connectors_, clique em **[!UICONTROL Connect]** no cartão _Meta Ads_.

1. Faça logon em sua conta do Facebook.

   Talvez seja necessário remover os bloqueadores de pop-ups e usar **[!UICONTROL Atualizar]** para tentar novamente.

1. Siga as instruções de autenticação do Facebook.

1. No pop-up _[!UICONTROL Logon do Facebook para Empresas]_ (Símbolo de meta para Adobe), passe pelas seleções a seguir.

   - Verifique as informações da conta e clique em **[!UICONTROL Continuar como]**
   - Conceda acesso a páginas selecionadas e clique em **[!UICONTROL Continuar]**
   - Conceda acesso a empresas selecionadas e clique em **[!UICONTROL Continuar]**
   - Aceite uma ou mais contas do Instagram e clique em **[!UICONTROL Continuar]**
   - Revise as seleções e clique em **[!UICONTROL Salvar]**

1. No modo de exibição _[!UICONTROL Meta Ads]_, selecione uma ou mais contas e clique em **[!UICONTROL Selecionar]**.

A exibição das _[!UICONTROL Contas de meta anúncios]_ lista as `Account name`, `Added by`, `Date added` e `Status`. Use **[!UICONTROL Adicionar conta]** para adicionar mais contas à lista.

## Assimilação de dados

Inicialmente, o GenStudio for Performance Marketing importa os seis meses mais recentes de dados históricos. Essa prática garante acesso imediato a insights relevantes para analisar tendências, avaliar desempenho e tomar decisões informadas. O processo de assimilação pode levar de um a cinco dias, dependendo do volume de dados na sua conta.

>[!BEGINSHADEBOX]

**Política de assimilação e retenção de dados**

O GenStudio for Performance Marketing retém os dados do canal por 13 meses. Essa política de retenção inclui os seis meses de dados assimilados durante a conexão inicial, garantindo uma análise e relatórios abrangentes de dados históricos.

>[!ENDSHADEBOX]
