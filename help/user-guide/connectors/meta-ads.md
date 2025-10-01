---
title: Conectar-se ao Meta Ads
description: Conecte uma conta do Meta Ads para ativar e monitorar seus anúncios e mídia com o Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: fb5fe4885340639f8179c8de6944ac21bfe009ec
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Conectar-se ao Meta Ads

Esta página explica como conectar e gerenciar a conta de perfil do Meta Ads com o GenStudio for Performance Marketing para gerenciar campanhas, exportar conteúdo e acessar dados de publicidade de suas campanhas ativas.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

- Logon do Facebook/Meta que pode acessar todos os serviços da Meta

- _Controle total_ sobre o Meta Business Portfolio e contas de anúncios, incluindo:

   - Gerenciar campanhas
   - Exibir desempenho
   - Gerenciar modelos de hub do Creative
   - Análises avançadas

- Desative qualquer bloqueador de pop-up no navegador

>[!ENDSHADEBOX]

## Conectar uma conta do Meta ads

1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Configurações]**.

1. Na seção _Data connectors_, clique em **[!UICONTROL Connect]** no cartão _Meta Ads_.

1. Faça logon em sua conta do Facebook.

   Talvez seja necessário remover os bloqueadores de pop-ups e usar **[!UICONTROL Atualizar]** para tentar novamente.

1. Siga as instruções de autenticação do Facebook, verifique as informações da conta e clique em **[!UICONTROL Continuar como...]**

1. Em _[!UICONTROL Logon do Facebook para Empresas]_ (símbolo do Meta para Adobe), passe pelas seguintes seleções para conceder acesso ao GenStudio for Performance Marketing:

   - Selecione um ou mais perfis do Meta Business e clique em **[!UICONTROL Continuar]**
   - Selecione uma ou mais páginas do Meta e clique em **[!UICONTROL Continuar]**
   - Selecione uma ou mais contas do Instagram e clique em **[!UICONTROL Continuar]**
   - Revise as seleções e clique em **[!UICONTROL Salvar]**

     ![Revisar seleções](/help/assets/meta/meta-review-selections.png "Revisar seleções"){width="400" zoomable="yes"}

1. Depois de receber a verificação de que sua conta está conectada, clique em **[!UICONTROL Obteve]**.

   Essa etapa garante que o GenStudio for Performance Marketing tenha acesso a todos os anúncios, metadados e métricas para obter o desempenho ideal.

1. Em _[!UICONTROL Meta Ads]_, selecione uma ou mais contas a serem incluídas em [!DNL Insights] e clique em **[!UICONTROL Selecionar]**.

1. Depois de receber uma confirmação de _Plataforma conectada_, clique em **[!UICONTROL Exibir contas]**.

   A exibição das _[!UICONTROL contas do Meta Ads]_ lista as `Account name`, `Added by`, `Date added` e `Status`.

   ![Lista de contas do Meta](/help/assets/meta/meta-accounts-list.png "Lista de contas conectadas do Meta"){zoomable="yes"}

Use **[!UICONTROL Adicionar conta]** para adicionar mais contas à lista. O fluxo de autorização pode ser um pouco diferente quando você adiciona contas vinculadas ao mesmo perfil do Meta Business. Você seleciona somente as novas contas do Meta Ads durante o processo de conexão.

## Desconectar e solucionar problemas de uma integração do Meta Ads

Às vezes, uma instância do GenStudio for Performance Marketing é conectada incorretamente a uma conta do Meta Ads. As configurações comuns que podem causar problemas incluem:

- Uma conta do Instagram é selecionada sem selecionar sua página associada do Facebook
- Permissões revogadas para um usuário que executou a conexão inicial

Nessas situações, é melhor reconectar a conta de anúncio do Meta à instância do GenStudio for Performance Marketing. Primeiro, o usuário deve remover a integração do aplicativo diretamente do Meta Business Manager, criando uma tabulação limpa para redefinir as permissões. Isso requer acesso de administrador ao Meta Business Manager.

Essas etapas limpam as permissões em cache e redefinem o fluxo de integração:

1. Acesse o [Meta Business Manager](https://business.facebook.com) visitando o site do Facebook.
1. Faça logon com sua conta da. A conta deve ter acesso de administrador ao Business Manager.
1. Clique no ícone de engrenagem **[!UICONTROL Configurações]** no canto inferior esquerdo para navegar até as configurações do Business Portfolio.
1. No menu à esquerda, clique em **[!UICONTROL Integrações]**.
1. Selecione **[!UICONTROL Aplicativos Conectados]**. Você verá o Adobe GenStudio na lista de aplicativos conectados.
   ![Aplicativos Conectados do Meta Business Manager](./meta-connected-apps.png "Painel Aplicativos Conectados do Meta Business Manager")
1. Clique no nome do aplicativo.
1. Clique em **[!UICONTROL Remover]**.
1. Confirme a remoção quando solicitado.

Agora você pode reconectar suas contas de anúncio do Meta, perfis do Instagram e páginas do Facebook.
