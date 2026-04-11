---
title: Marketo para GenStudio
description: Instale e configure o aplicativo Marketo para GenStudio Adobe Exchange para que sua organização possa usar modelos do Marketo Engage no GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: 4118624b479905cd2f2193d542c000678daaf4b8
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Marketo para GenStudio

As organizações que usam o [!DNL Marketo Engage] e o [!DNL GenStudio for Performance Marketing] na mesma organização do [!DNL IMS] podem instalar o aplicativo **Marketo for GenStudio** do [!DNL Adobe Exchange]. Depois que um administrador do sistema aprovar o aplicativo e concluir a implantação, os autores poderão escolher modelos do Marketo ao criar experiências de email no GenStudio, ao lado de modelos carregados diretamente para [!DNL Content].

Este tópico é para **administradores** que instalam o aplicativo, coletam credenciais do Marketo e implantam o aplicativo no Exchange. Para saber como a sintaxe de modelo do AJO e do Marketo funciona com o GenStudio, consulte [Modelos do AJO e do Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Pré-requisitos

* [!DNL Marketo Engage] deve ser provisionado na organização em que você implanta a extensão.
* Os usuários que implantam o aplicativo precisam de **credenciais do Marketo**. Para criar e recuperar essas credenciais, você deve ter acesso ao **Administrador do produto Marketo** (a área **[!UICONTROL Administrador]** deve estar disponível ao abrir o Marketo).

## Instalar o aplicativo do Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483316?captions=por_br&learn=on)

1. Abra o [Adobe Exchange](https://exchange.adobe.com) e vá para o **[!UICONTROL Experience Cloud]**.
1. Abra a lista [Marketo para GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio).
   ![Marketo para listagem do GenStudio no Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Selecione **[!UICONTROL Gratuito]** para solicitar o aplicativo para sua organização.
1. Depois que sua organização **revisar e aprovar** a solicitação, continue com [Obter credenciais do Marketo](#get-marketo-credentials) e [Implantar o aplicativo do Exchange](#deploy-the-application-from-exchange).

## Obter credenciais do Marketo

Você usa credenciais da instância do **Marketo** (não do Adobe Developer Console). Colete os itens a seguir antes de implantar no Exchange.

### Criar um usuário somente API (opcional se você reutilizar um usuário API existente)

1. No Marketo, vá para **[!UICONTROL Admin]**.
1. Em **[!UICONTROL Segurança]**, abra **[!UICONTROL Usuários e Funções]**.
1. Para um novo usuário da API, clique em **[!UICONTROL Criar somente usuário da API]** (use um email exclusivo para cada usuário da API). Atribua a função **[!UICONTROL Funções de API (todos os Espaços de Trabalho)]** (ou as funções exigidas por sua organização). Se você já tiver um usuário de API que deseja usar, pule para [Criar ou selecione um serviço do LaunchPoint](#create-or-select-a-launchpoint-service).

![Usuários e funções com API somente e funções de usuário e API](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### Criar ou selecionar um serviço LaunchPoint

1. Em **[!UICONTROL Admin]**, em **[!UICONTROL Integração]**, abra o **[!UICONTROL LaunchPoint]**.
1. Clique em **[!UICONTROL Criar]** para criar um novo Serviço (ou usar um serviço personalizado existente).
   ![Serviço personalizado do LaunchPoint](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. Para o seu serviço, clique em **[!UICONTROL Exibir Detalhes]** e copie a **[!UICONTROL ID do Cliente]** e o **[!UICONTROL Segredo do Cliente]**. Você os inserirá na **[!UICONTROL Configuração]** do Adobe Exchange.

### Observe o URL de base da API REST do Marketo

1. Em **[!UICONTROL Admin]**, em **[!UICONTROL Integração]**, abra os **[!UICONTROL Serviços Web]**.
1. Localize o ponto de extremidade da **[!UICONTROL API REST]**. Copie somente a **URL base** (host), no formato `https://###-XXX-###.mktorest.com`. **não** inclua segmentos de caminho como `/rest` ou `/identity`. Esse valor é exclusivo por instância do Marketo.

![URL base do ponto de extremidade da API REST de Serviços da Web](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

Você também precisará da **[!UICONTROL URL da Identidade da Marketo Engage]** que sua tela de implantação do Exchange solicita, juntamente com a URL de base REST e a ID do Cliente e o Segredo do Cliente do LaunchPoint.

## Implantar o aplicativo do Exchange

Para disponibilizar a extensão no GenStudio, implante o aplicativo do Adobe Exchange.

1. Retornar ao [Adobe Exchange](https://exchange.adobe.com).
1. Selecione **[!UICONTROL Gerenciar]** e abra o aplicativo **Marketo para GenStudio** (por exemplo, em **[!UICONTROL aplicativos App Builder]** ou em aplicativos gerenciados de sua organização).
1. Em **[!UICONTROL Ambientes]**, escolha um ambiente existente na lista suspensa ou selecione **[!UICONTROL Adicionar ambiente]** para criar um.
1. Abrir **[!UICONTROL Configuração]** para o ambiente selecionado.
1. Insira a **[!UICONTROL ID do Cliente]** e o **[!UICONTROL Segredo do Cliente]** do [LaunchPoint](#create-or-select-a-launchpoint-service), a **[!UICONTROL URL da Identidade do Marketo Engage]** e a **[!UICONTROL URL Base da API REST do Marketo Engage]** (o host base dos [Serviços da Web](#note-your-marketo-rest-api-base-url)).
1. Clique em **[!UICONTROL Implantar]**. Quando a implantação for bem-sucedida, a ação será alterada para **[!UICONTROL Desimplantar]**.

### Atualizar configuração

Para alterar os valores de configuração de um ambiente, **[!UICONTROL Desimplantar]** primeiro, atualize os campos e **[!UICONTROL Implante]** novamente.

## Acessar modelos do Marketo no GenStudio

Depois que o Marketo for GenStudio for instalado e configurado, uma guia **[!UICONTROL Modelos do Marketo]** será exibida quando você criar uma experiência de **Email** no GenStudio. Use essa guia para procurar modelos na Marketo Engage.

>[!IMPORTANT]
>
>Crie emails no fluxo de experiência do **email padrão** no GenStudio for Performance Marketing. Essa integração NÃO é compatível com emails criados com a nova experiência do editor de email.

![Configuração do Exchange com credenciais da Marketo](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## Solução de problemas

### A guia Modelos do Marketo não está visível

* Confirme se o aplicativo está **Aprovado** no Exchange e se o ambiente está **implantado** com a ID do Cliente, o Segredo do Cliente e as URLs de base da Marketo válidos.
* Peça ao administrador para verificar se o acesso de **Administrador de Produto do Marketo** foi usado ao criar credenciais.

### Os modelos não são carregados

* Recarregue a página ou saia e entre novamente na GenStudio.
* No painel de ferramentas do desenvolvedor do navegador **[!UICONTROL Rede]**, procure chamadas de API com falha para sua instância do Marketo e verifique se a URL base REST corresponde a **[!UICONTROL Serviços da Web]** no Marketo (nenhum caminho extra após o host).
