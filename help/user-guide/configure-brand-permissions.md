---
title: Atribuir  [!DNL Brand] permissões
description: Saiba mais sobre a atribuição de direitos para criadores e editores do GenStudio for Performance Marketing [!DNL Brand] .
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# Atribuir [!DNL Brand] permissões

Por padrão, os gerentes de sistema da GenStudio podem criar e editar [!DNL Brands]. As funções de editor de conteúdo e colaborador têm permissões de edição e criação, mas podem não exigir direitos de gerenciamento do sistema. Para conceder aos editores de conteúdo e colaboradores esses direitos relacionados ao [!DNL Brand], um administrador do sistema do Adobe deve executar algumas tarefas de configuração adicionais na Adobe Admin Console. Consulte [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) em _Guia de administração de empresas e equipes_.

Adicionar usuários e grupos de usuários é uma tarefa básica comum a todos os produtos da Adobe com direitos gerenciados pela Admin Console. Consulte [Usuários do Adobe Admin Console](https://helpx.adobe.com/br/enterprise/using/users.html) no _Guia de administração de empresas e equipes_ para obter uma visão geral do gerenciamento de usuários e dos procedimentos para adicionar usuários e grupos de usuários.

## Etapa 1: Criar um grupo de usuários

**Para criar um grupo de usuários**:

1. Faça logon na Admin Console e navegue até **[!UICONTROL Usuários]** > **[!UICONTROL Grupos de Usuários]**.

1. Clique em **[!UICONTROL Novo Grupo de Usuários]**. O pop-up _Criar um novo grupo de usuários_ é aberto.

1. Adicione um nome informativo do grupo de usuários ao campo **[!UICONTROL Nome do grupo de usuários]** para identificar a finalidade do novo grupo. Por exemplo, &quot;Gerentes de marca&quot;.

1. Opcionalmente, adicione uma descrição do grupo e sua finalidade.

1. Clique em **[!UICONTROL Salvar]**. O Admin Console abre o pop-up _Novo grupo_, com o nome do grupo recém-criado.

Consulte [Gerenciar grupos de usuários](https://helpx.adobe.com/br/enterprise/using/user-groups.html) no _Guia de administração de empresas e equipes_.

## Etapa 2: atribuir um perfil do GenStudio System Manager ao grupo de usuários

Depois de criar um novo grupo de usuários e adicionar usuários, você pode atribuir o perfil do **Adobe GenStudio system manager** a esse grupo. O direito associado ao perfil atribuído fornece a todos os usuários neste grupo permissões do GenStudio [!DNL Brands] (criar, atualizar e excluir marcas).

**Para atribuir um perfil ao grupo de usuários**:

1. Navegue até o grupo de usuários recém-criado e clique na guia _Perfis de produto atribuídos_.

1. Na guia _Perfis de produto atribuídos_, clique em **[!UICONTROL Atribuir perfil]**. A janela pop-up _Atribuir produtos e perfis_ é aberta.

1. Selecione `Adobe GenStudio` na lista _Selecionar produtos_.

1. Clique em **[!UICONTROL Aplicar]**. O pop-up _Selecionar perfis de produto_ é aberto, exibindo os perfis de produto associados ao Adobe GenStudio.

1. Selecione `Adobe GenStudio system manager`.

1. Clique em **[!UICONTROL Aplicar]**. O pop-up _Atribuir produtos e perfis_ é aberto, exibindo o perfil de produto do grupo de usuários recém-criado.

1. Clique em **[!UICONTROL Salvar]**.

Consulte [Atribuir perfis de produto a grupos de usuários](https://helpx.adobe.com/br/enterprise/using/user-groups.html) no _Guia de administração de empresas e equipes_.

## Etapa 3: adicionar usuários ao grupo de usuários

Para atribuir aos usuários a permissão para criar, editar e publicar [!DNL Brands], adicione-os ao grupo de usuários recém-criado.

>[!NOTE]
>
>Você deve adicionar pelo menos um usuário a este grupo de usuários antes de adicionar o grupo ao seu projeto.

**Para adicionar usuários ao grupo de usuários**:

1. No _Admin Console_, navegue até **[!UICONTROL Usuários]** > **[!UICONTROL Grupos de Usuários]**.

1. Selecione o nome do grupo de usuários criado anteriormente. A janela pop-up _Adicionar usuários a este grupo de usuários_ é aberta.

1. Adicione um usuário novo ou existente por nome de usuário ou endereço de email. Ao inserir um nome ou endereço de email para um usuário existente, esse campo é preenchido automaticamente com nomes correspondentes para usuários conhecidos que pertencem a esta Organização IMS. Saiba mais sobre como gerenciar grupos de usuários em [Gerenciar grupos de usuários](https://helpx.adobe.com/br/enterprise/using/user-groups.html) no _Guia de administração de empresas e equipes_.

Os usuários recebem as permissões de criação, edição e publicação do [!DNL Brand] dos gerenciadores de sistema do Adobe GenStudio quando adicionados ao grupo. Os usuários também recebem um convite automatizado por email para editar o projeto [!DNL Brands] do Adobe GenStudio for Performance Marketing.

## Etapa 4: Criar um projeto [!DNL Brands]

Um _projeto_ fornece um local de armazenamento onde usuários selecionados podem salvar ativos — neste caso, [!DNL Brands] ativos.

**Para criar um projeto [!DNL Brands] a partir da _guia Armazenamento_**:

1. Navegue até a guia _Armazenamento_ na Admin Console.

1. Clique em **[!UICONTROL Projetos]** na navegação lateral. A guia _Projetos_ é aberta.

1. Clique em **[!UICONTROL Criar projeto]**. O pop-up _Novo projeto_ é aberto.

1. Digite `Adobe GenStudio Brands` no campo de nome do projeto. Digite este nome de projeto exatamente como exibido aqui. Não inclua espaços extras nem altere a caixa da letra.

1. Clique em **[!UICONTROL Criar]**. A janela pop-up _Convidar para projeto_ é aberta.

Consulte [Gerenciar projetos](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) no _Guia de administração de empresas e equipes_.

## Etapa 5: Convidar grupo de usuários para projeto

Agora você está pronto para adicionar o grupo de usuários que acabou de criar ao projeto `Adobe GenStudio [!DNL Brands]`.

**Para convidar o grupo de usuários para o projeto recém-criado**:

1. No pop-up _Convidar para projeto_, adicione o grupo de usuários que você acabou de criar a este projeto.

1. Escolha a opção de permissões **Pode editar**.

1. Clique em **[!UICONTROL Convidar]**.
