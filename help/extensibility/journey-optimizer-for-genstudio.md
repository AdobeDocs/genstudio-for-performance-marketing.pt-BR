---
title: Journey Optimizer para GenStudio
description: Instale e configure o aplicativo Journey Optimizer para GenStudio Adobe Exchange para que sua organização possa usar modelos do Adobe Journey Optimizer no GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: fbec4567d960a6e3607c5e5e43057e2f22e9f6ea
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Journey Optimizer para GenStudio

As organizações que usam o [!DNL Adobe Journey Optimizer] (AJO) e o [!DNL GenStudio for Performance Marketing] na mesma organização do [!DNL IMS] podem instalar o aplicativo **Journey Optimizer for GenStudio** do [!DNL Adobe Exchange]. Depois que um administrador do sistema aprovar o aplicativo e concluir a implantação, os autores poderão escolher modelos de conteúdo do AJO ao criar experiências de email no GenStudio, ao lado dos modelos carregados diretamente para [!DNL Content].

Este tópico é para **administradores e desenvolvedores** que instalam o aplicativo, criam credenciais OAuth no [!DNL Adobe Developer Console] e mapeiam permissões de conta técnica no [!DNL Adobe Experience Platform]. Para saber como a sintaxe de modelo do AJO e do Marketo funciona com o GenStudio, consulte [Modelos do AJO e do Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Pré-requisitos

* O AJO deve ser provisionado na organização em que você implanta a extensão.
* Os usuários que criam modelos no AJO precisam de permissão para **criar e editar** modelos de conteúdo no Journey Optimizer, conforme definido pela sua organização.
* Os modelos de email no AJO devem incluir espaços reservados em campo (barras de controle) onde o conteúdo gerado deve aparecer. Um modelo pode ser selecionado sem esses campos, mas **a geração de experiência falha** se os espaços reservados que [!DNL GenStudio for Performance Marketing] espera estiverem ausentes. Consulte [Personalizar um modelo](/help/user-guide/templates/customize-template.md) e [Nomes de campos reconhecidos](/help/user-guide/templates/customize-template.md#recognized-field-names).

## Instalar o aplicativo do Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483304?captions=por_br&learn=on)

1. Abra o [Adobe Exchange](https://exchange.adobe.com) e vá para o **[!UICONTROL Experience Cloud]**.
1. Abra a lista [Journey Optimizer para GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio).
   ![Listagem do Journey Optimizer for GenStudio no Adobe Exchange, incluindo requisitos e instalação gratuita](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. Selecione **[!UICONTROL Gratuito]** para solicitar o aplicativo para sua organização.
1. Depois que sua organização **revisar e aprovar** a solicitação, continue com [Criar credenciais OAuth no Adobe Developer Console](#create-oauth-credentials-in-adobe-developer-console) e [Implantar o aplicativo do Exchange](#deploy-the-application-from-exchange).

## Criar credenciais OAuth no Adobe Developer Console

Crie um **projeto** no [Adobe Developer Console](https://developer.adobe.com/console/) que forneça credenciais OAuth para a API do Journey Optimizer. Você precisará de valores como **ID do Cliente**, **Segredo do Cliente**, **ID da Organização** e **Escopo** ao configurar o aplicativo no Exchange.

1. Faça logon na Adobe Developer Console e crie um **novo projeto**.
1. Adicione a **API do Adobe Journey Optimizer (AJO)** ao projeto clicando em **[!UICONTROL Adicionar API]** e selecionando **[!UICONTROL Adobe Journey Optimizer]** na lista de APIs de produto **[!DNL Experience Cloud]**.
1. Gere credenciais no espaço de trabalho do projeto e copie a **ID do Cliente**, **Segredo do Cliente**, **ID da Organização**, **Escopo** e quaisquer outros valores solicitados pelo fluxo de implantação. Armazene-os com segurança na próxima seção.

>[!NOTE]
>
>Ao instalar a partir do Exchange, use a **ID do cliente OAuth** se uma ID do cliente OAuth e uma ID da conta técnica forem mostradas.

## Implantar o aplicativo do Exchange

### Abra o aplicativo em Gerenciar e adicione um ambiente

1. Retornar ao [Adobe Exchange](https://exchange.adobe.com).
1. Selecione **[!UICONTROL Gerenciar]** e abra os **[!UICONTROL aplicativos App Builder]** (ou o caminho da sua organização para aplicativos gerenciados).
1. Selecione **Journey Optimizer para GenStudio** e confirme se o aplicativo é **Aprovado**.
1. Em **[!UICONTROL Ambientes]**, escolha um ambiente existente na lista suspensa **Ambientes:** ou selecione **[!UICONTROL Adicionar ambiente]** para criar um.
   ![Detalhes do aplicativo com status Aprovado e Adicionar Ambiente](/help/extensibility/ajo-config-002.png){width="50%"}
1. No ambiente selecionado, selecione **[!UICONTROL Configuração]**.
1. Na guia **[!UICONTROL Configuração]**, encontre **[!UICONTROL Credenciais da AJO]**.
   ![Configuração com Credenciais do AJO antes da implantação (Rascunho)](/help/extensibility/ajo-config-004.png){width="80%"}
1. Insira as credenciais do projeto do Developer Console que tem a API do Journey Optimizer adicionada (por exemplo, **[!UICONTROL ID do Cliente do AJO]**, **[!UICONTROL Segredo do Cliente do AJO]** e **[!UICONTROL Ponto de Extremidade do Token do AJO]** e quaisquer outros campos obrigatórios).
1. Insira o nome da **sandbox totalmente em minúsculas** (por exemplo, `prod`).
1. Clique em **[!UICONTROL Implantar]**. Quando a implantação for concluída, o status será exibido como implantado. O texto do botão será alterado para **[!UICONTROL Desimplantar]**.
   ![Aplicativo implantado com Undeploy disponível na exibição de aplicativos do App Builder](/help/extensibility/ajo-config-005.png){width="80%"}

Após a implantação, a Adobe Developer Console inclui um novo projeto gerado automaticamente chamado **Journey Optimizer para o GenStudio &lt;Your_Environment_Name>** com APIs do AJO e Adobe Runtime. Este projeto é somente leitura e não pode ser editado ou excluído.
![Projeto Developer Console gerado automaticamente somente leitura após a implantação](/help/extensibility/ajo-auto-project.png){width="100%"}

### Atualizar configuração

Para alterar as variáveis de configuração de um ambiente, **[!UICONTROL Desimplantar]** primeiro, atualize os valores e **[!UICONTROL Implante]** novamente para que as alterações entrem em vigor.

Você pode criar **vários ambientes** no Exchange (por exemplo, um por sandbox). Cada implantação pode aparecer como uma experiência separada no GenStudio quando sua organização usa várias sandboxes.

## Mapear permissões para a conta técnica

Os usuários podem ver a extensão do AJO no GenStudio sem acesso total ao [!DNL Adobe Experience Platform]. Para chamadas de API (por exemplo, carregar modelos), a conta técnica vinculada às credenciais OAuth deve receber permissões do Journey Optimizer em **[!DNL Adobe Experience Platform]** > **[!UICONTROL Permissões]**. Os nomes de função e conjuntos de permissões exatos dependem da sua organização.

Exiba a extensão em **[!UICONTROL Administrador do Jornada]** em **[!UICONTROL Permissões]** > **[!UICONTROL Funções]** do AJO e adicione as **credenciais de API** do projeto do Developer Console, as mesmas credenciais usadas ao implantar do Exchange.

![Credenciais de API atribuídas à função do AJO Architect nas Permissões do Adobe Experience Platform](/help/extensibility/ajo-map-permissions.png){width="80%"}

**Consulte também** (controle de acesso do Journey Optimizer):

* [Controle de acesso](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Permissões no Journey Optimizer](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/access-control/permissions)
* [Introdução para administradores do sistema](https://experienceleague.adobe.com/pt-br/docs/journey-optimizer/using/get-started/quick-start/administrator)

## Acessar modelos do AJO no GenStudio

Após a implantação e o mapeamento de permissões:
1. Abra o **[!UICONTROL Criar]** no GenStudio for Performance Marketing e inicie uma experiência de **Email**.
1. Em **[!UICONTROL Selecionar modelo]**, abra a guia **[!UICONTROL Modelo do AJO]** ao lado de **[!UICONTROL Modelos carregados]** para procurar modelos no Journey Optimizer.

![Selecionar modelo com a guia Modelo do AJO e a galeria de modelos](/help/extensibility/ajo-template-tab.png){width="80%"}

## Solução de problemas

### A guia Modelos do AJO não está visível

* Confirme se os valores inseridos na **[!UICONTROL Configuração]** do Exchange estão corretos, incluindo **ID do Cliente**, **Segredo do Cliente**, **Escopo** e **Sandbox**.
* Verifique se o nome da **sandbox está em minúsculas** (por exemplo, `prod`).
* Ao instalar do Exchange, use a **ID do Cliente** conforme descrito em [Criar credenciais OAuth](#create-oauth-credentials-in-adobe-developer-console).

### A guia Modelos do AJO está visível, mas nenhum modelo é exibido

* Recarregue a página ou abra a guia **[!UICONTROL Modelo do AJO]** novamente.
* Nas ferramentas do navegador **[!UICONTROL Rede]**, inspecione a solicitação **`get-templates`**. Se retornar **403 Proibido**, a conta técnica não será atribuída a uma função ou grupo com as permissões necessárias do Journey Optimizer. Atualize os mapeamentos em [!DNL Adobe Experience Platform] **[!UICONTROL Permissões]** e em **[!UICONTROL Permissões]** da AJO conforme exigido pela sua organização.
