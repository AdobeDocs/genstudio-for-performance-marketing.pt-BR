---
title: Conectar um assistente do AI
description: Saiba como conectar um assistente de IA com suporte ao [!DNL GenStudio for Performance Marketing] e verificar o acesso às ferramentas disponíveis.
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# Conectar um assistente de IA

Conecte um assistente de IA com suporte ao [!DNL GenStudio for Performance Marketing] antes de consultar dados de desempenho, reunir rascunhos ou publicar anúncios aprovados. As opções de conexão variam de acordo com o assistente de IA e a organização.

## Pré-requisitos

Antes de se conectar, confirme se você tem:

- Uma conta ativa do Adobe com acesso a [!DNL GenStudio for Performance Marketing].
- Um plano suportado que permite conexões MCP remotas quando você usa Claude, ChatGPT ou Microsoft Copilot. Consulte a documentação do assistente de IA para obter instruções específicas sobre como configurar manualmente conexões MCP.

## Conectar o Adobe CX Enterprise Coworker

[!DNL GenStudio for Performance Marketing] ferramentas são gerenciadas como uma conexão nativa no Adobe CX Enterprise Coworker. Sua organização controla a disponibilidade, de modo que você não insira o URL do servidor MCP direto.

Inicie uma nova conversa e [verifique a conexão](#verify-the-connection). Se as ferramentas não forem exibidas, entre em contato com o administrador da organização ou representante da Adobe.

## Conectar Claude

Claude exige um plano Pro, Max, Team ou Enterprise. O mesmo conector remoto funciona no Claude na web e no aplicativo de desktop.

1. Em Claude, selecione **[!UICONTROL Personalizar]** na barra lateral esquerda.
1. Selecione **[!UICONTROL Conectores]** e, em seguida, o ícone adicionar.
1. Selecione **[!UICONTROL Adicionar conector personalizado]**.
1. Digite `https://genstudio-services.adobe.io/mcp` como a URL do servidor MCP.
1. Faça logon com sua Adobe ID.
1. Selecione a organização IMS que tem acesso a [!DNL GenStudio for Performance Marketing].

&#x200B;> [!NOTE]
&#x200B;> Em um plano Team ou Enterprise, o proprietário de uma organização pode precisar adicionar o conector primeiro. Se o conector já estiver disponível, selecione **[!UICONTROL Conectar]**.

## Conectar o ChatGPT

O ChatGPT requer uma conta Plus, Pro, Business, Enterprise ou Education. As conexões MCP personalizadas estão disponíveis na Web por meio do modo de desenvolvedor.

1. Entre no [ChatGPT](https://chatgpt.com) em um navegador da Web.
1. Abra **[!UICONTROL Configurações]** e habilite o **[!UICONTROL Modo de desenvolvedor]**.
1. Em **[!UICONTROL Configurações]**, abra a área para aplicativos ou conectores.
1. Adicione uma conexão MCP personalizada denominada `GenStudio`.
1. Digite `https://genstudio-services.adobe.io/mcp` como a URL do servidor MCP.
1. Mantenha **[!UICONTROL OAuth]** como o método de autenticação.
1. Faça logon com sua Adobe ID.
1. Selecione a organização IMS que tem acesso a [!DNL GenStudio for Performance Marketing].

&#x200B;> [!NOTE]
> O ChatGPT pode alterar o local das configurações do desenvolvedor e do conector. Se esses rótulos forem diferentes em sua conta, siga as instruções atuais do OpenAI para adicionar um conector MCP remoto.

## Conectar códex

O Codex requer a interface de linha de comando do Codex e uma conta do Codex autenticada.

1. Abra `~/.codex/config.toml` para todos os projetos ou `.codex/config.toml` para um projeto.
1. Adicionar esta configuração:

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. Executar `codex mcp login genstudio`.
1. Faça logon com sua Adobe ID na janela do navegador que é aberta.
1. Selecione a organização IMS que tem acesso a [!DNL GenStudio for Performance Marketing].

## Conectar Gravador

O Writer requer acesso ao AI Studio.

1. No Writer, abra **[!UICONTROL AI Studio]**.
1. Selecione **[!UICONTROL Conectores e ferramentas]**.
1. Selecione **[!UICONTROL Criar conector personalizado]**.
1. Selecione **[!UICONTROL Servidor MCP]** como o tipo de conector.
1. Insira um nome e uma descrição para o conector.
1. Digite `https://genstudio-services.adobe.io/mcp` como a URL do servidor MCP.
1. Defina o acesso do grupo ao conector.
1. Selecione **[!UICONTROL OAuth 2.0 (nível de usuário)]** como o método de autenticação.
1. Faça logon com sua Adobe ID.
1. Selecione **[!UICONTROL Salvar]**.

[!DNL GenStudio for Performance Marketing] ferramentas aparecem na biblioteca de ferramentas do AI Studio. Cada usuário do Writer faz logon com uma Adobe ID individual.

## Conectar o Microsoft Copilot

O Microsoft controla o fluxo de configuração para conexões MCP personalizadas no Copilot. Siga a [documentação do Microsoft Copilot](https://learn.microsoft.com/en-us/copilot/) atual para adicionar um servidor MCP remoto e, em seguida, use `https://genstudio-services.adobe.io/mcp` como URL do servidor.

Quando solicitado, entre com sua Adobe ID e selecione a organização IMS que tem acesso a [!DNL GenStudio for Performance Marketing].

## Verifique a conexão

Após a configuração, confirme se as ferramentas estão disponíveis.

1. Inicie uma nova conversa no assistente de IA.
1. Pergunte ao assistente quais [!DNL GenStudio for Performance Marketing] ferramentas ele pode acessar.
1. Confirme se a resposta lista ferramentas nos Insights, Criar e Ativar.
1. Solicite um resumo do desempenho de um canal de mídia paga conectado.

O assistente retorna os dados de desempenho disponíveis ou explica por que nenhum dado corresponde à solicitação.

&#x200B;> [!TIP]
&#x200B;> Se a autenticação falhar, reconecte e confirme se você selecionou a organização IMS correta. Se nenhuma ferramenta for exibida, confirme se sua conta tem acesso ao [!DNL GenStudio for Performance Marketing].

## Recursos relacionados

- [Visão geral dos assistentes de IA](overview.md)
- [Usar assistentes de IA](use-ai-assistants.md)
- [Referência das ferramentas do assistente de IA](tools-reference.md)
