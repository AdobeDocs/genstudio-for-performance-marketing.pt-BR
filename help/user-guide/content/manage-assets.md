---
title: Gerenciar ativos e experiências
description: Simplifique e aprimore o gerenciamento de ativos aprovados pela marca para uso e reutilização em sua jornada de marketing digital.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: d5efabbaf3dd0817bd3158acb59d997a727e5f62
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gerenciar ativos e experiências

O Adobe GenStudio for Performance Marketing [!DNL Content] simplifica e aprimora o gerenciamento de ativos aprovados pela marca para uso e reutilização em sua jornada de marketing digital.

## Galeria [!DNL Content]

A galeria mostra um inventário de ativos, experiências ou modelos aprovados, dependendo da exibição selecionada. O ícone de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar entre várias categorias para filtrar o conteúdo mostrado na galeria. No modo de exibição _[!UICONTROL Assets]_, clique no ícone de pesquisa (lupa) para usar uma palavra-chave para localizar um ativo.

A seguir, uma pesquisa sobre o termo `dog` na galeria [!UICONTROL Assets]:

![exibição do Assets com pesquisa no cachorro](/help/assets/content-assets.png)

### Pesquisar conteúdo

O filtro e a interface de pesquisa são rápidos e responsivos e fornecem uma experiência produtiva de pesquisa. Cada exibição do [!DNL Content] fornece opções de filtro para restringir sua pesquisa pelo ativo, experiência ou modelo ideal. Para ativos e experiências, você pode selecionar uma campanha e diretrizes específicas, como o conteúdo criado para um produto específico.

Há filtros baseados em [palavras-chave](asset-details.md#user-defined-metadata) e [categorias de atributo](/help/user-guide/insights/attribute-category.md) para restringir os resultados da pesquisa. Por exemplo, talvez você queira encontrar um ativo de um tipo de arquivo ou assunto específico para ajudá-lo a criar uma nova experiência para sua campanha. Ou você pode filtrar o conteúdo com base no seu nome de usuário ou no nome de um membro da equipe:

- O filtro **[!UICONTROL Carregado por]** limita a lista _[!UICONTROL Assets]_ para mostrar apenas os ativos carregados por você ou por uma pessoa específica.
- O filtro **[!UICONTROL Criado por]** limita a lista _[!UICONTROL Experiências]_ para mostrar apenas as experiências criadas por você ou por uma pessoa específica.

**Para pesquisar conteúdo a ser reutilizado**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Assets]**.

1. Selecione um repositório de ativos na lista **[!UICONTROL Local]** ou verifique se você está observando o repositório de ativos correto. `GenStudio assets` é o repositório padrão.

   >[!IMPORTANT]
   >
   >A lista _Local_ está disponível somente quando você [se conecta a um repositório AEM](connect-aem-repo.md).

1. Clique em **[!UICONTROL Pesquisar]** (lupa) para inserir uma palavra-chave ou descrição.

1. Restrinja sua pesquisa selecionando uma categoria na lista _[!UICONTROL Filtro]_. Por exemplo, se você estiver procurando um arquivo PNG, clique em **[!UICONTROL Formato de arquivo]** e escolha **PNG**.

   Quanto mais você limitar sua pesquisa, menos opções de filtro estarão disponíveis. Clique em **[!UICONTROL Limpar tudo]** para remover todos os filtros.

1. Selecione um ativo para obter uma visualização completa e uma lista de detalhes.

   Clique em **[!UICONTROL Baixar]** (seta para baixo) para usar o ativo na sua estação de trabalho local.

### Local

Por padrão, os ativos adicionados a [!DNL Content] por meio do processo [!DNL Create] ou através de upload são armazenados no repositório `GenStudio assets`. O repositório `GenStudio assets` é um repositório leitura-gravação no GenStudio for Performance Marketing. Isso significa que você pode salvar, editar e excluir ativos no repositório `GenStudio assets`.

A lista **[!UICONTROL Local]** acima da galeria _[!UICONTROL Assets]_ à direita permite selecionar entre repositórios do Adobe Experience Manager (AEM) [!DNL Assets Content Hub] conectados.

![Lista de locais de repositórios](../../assets/content-location-selection.png){width="350"}

Quando você seleciona um repositório AEM, a galeria mostra um inventário de ativos desse repositório, permitindo que você aproveite os ativos aprovados desses repositórios como entradas para a criação de conteúdo. As opções de filtro são alteradas para refletir as categorias configuradas em [!DNL AEM Assets Content Hub].

Consulte [Conectar um repositório AEM](connect-aem-repo.md) para obter orientação sobre como adicionar seu repositório [!DNL AEM Assets Content Hub] ao GenStudio for Performance Marketing.

O repositório AEM é somente leitura, o que significa que você pode acessar o conteúdo, mas não pode salvar rascunhos, novos ativos ou metadados no repositório AEM. Todos os rascunhos e atualizações finais para ativos, experiências e modelos são salvos no repositório do `GenStudio assets` com os novos [metadados do sistema](asset-details.md#system-metadata).

{{note-aem-assets}}

Um repositório AEM pode aplicar determinados requisitos de licenciamento, como a expiração de ativos. Esses ativos podem não estar disponíveis para uso nos fluxos de trabalho do [!DNL Create]. Os ativos expirados podem precisar ser renovados ou substituídos para manter a continuidade dos projetos. Consulte o administrador do [!DNL AEM Assets Content Hub] para obter assistência com esses ativos.

## Gerenciamento do Assets

No [!UICONTROL Conteúdo], você pode armazenar, recuperar e gerenciar facilmente seus ativos digitais. Ao utilizar os repositórios `GenStudio assets` e AEM, é possível garantir que seus ativos estejam bem organizados e acessíveis para várias campanhas de marketing. Essa abordagem de vários repositórios oferece flexibilidade e controle sobre o uso de ativos em todos os ambientes, garantindo que somente ativos aprovados e atualizados sejam usados em esforços de marketing.

A tabela a seguir lista as tarefas de gerenciamento disponíveis para ativos, experiências e modelos:

| Tarefas | Ativos | Experiências | Modelos |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [Exibir detalhes](/help/user-guide/content/asset-details.md) | ✓ µ | ✓ | ✓ |
| [Criar experiência](/help/user-guide/create/overview.md) |        |             | ✓ |
| [Editar no Adobe Express](#edit-in-express) | ✓ |             |           |
| [Exportar para Ativação](#export-for-activation) |        | ✓ |           |
| [Atualizar](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [Download](#download-assets) | ✓ |             | ✓ |
| [Excluir](#delete-assets) | ✓ | ✓ | ✓ |

### Adicionar ativos

Ao adicionar ativos ao [!DNL Content], eles são armazenados por padrão no repositório `GenStudio assets`. O botão _[!UICONTROL Adicionar ativos]_ está disponível somente quando o _[!UICONTROL Local]_ é o repositório `GenStudio assets`.

![Campo de localização](../../assets/content-location.png){width="350"}

**Para adicionar um ou mais ativos**:

1. Em _[!DNL Content]_, clique em **[!UICONTROL Adicionar ativos]**.

1. No modo de exibição _Adicionar ativos aprovados_, solte um ou mais arquivos no espaço. Como opção, você pode selecionar arquivos locais usando o **[!UICONTROL Procurar]** ou importar arquivos do Dropbox ou do Microsoft OneDrive.

1. Na seção _Adicionar detalhes_, selecione um **[!UICONTROL nome da campanha]** ou insira um novo nome.

1. Para melhorar a descoberta, adicione detalhes opcionais, como _Marca_, _Personas_, _Região_ e _Palavras-chave_, na seção **Mais detalhes**.

   Quanto mais detalhes você fornecer, mais conhecerá os recursos avançados do GenStudio for Performance Marketing. Selecione um ou mais detalhes na lista ou insira um novo, onde aplicável, como com palavras-chave. Cada detalhe adicionado aparece abaixo da lista. Clique em **`x`** para remover um detalhe.

   Todos os detalhes adicionados se aplicam a todos os ativos adicionados nesta ação.

   Consulte [detalhes de metadados](/help/user-guide/content/asset-details.md#system-metadata).

1. Clique em **[!UICONTROL Adicionar ativos]**.

1. Quando o carregamento do ativo for concluído, clique em **Concluído**.

1. Para exibir os novos ativos carregados, clique em **[!UICONTROL Atualizar]** na notificação _Novos ativos disponíveis_, na parte inferior da Tela.

### Baixar ativos

**Para baixar um ativo**:

1. Em _[!DNL Content]_, selecione um ativo ou modelo. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição de ativos, clique no ícone **[!UICONTROL Download]** (seta para baixo) no canto superior direito.

1. O download começa colocando uma cópia do ativo no local de download padrão.

### Excluir ativos

**Para excluir um ativo**:

1. Em _[!DNL Content]_, selecione um ativo, experiência ou modelo. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição do ativo, clique em **[!UICONTROL Excluir]** (lixeira) no canto superior direito.

1. No pop-up _Excluir ativo_, verifique o ativo e clique em **[!UICONTROL Excluir]**.

## Exportar para ativação

É possível exportar uma experiência aprovada para ativação em um formato compatível com o canal de destino.

**Para exportar uma experiência**:

1. Em _[!DNL Content]_, selecione uma experiência. Clicar em uma experiência abre a exibição de detalhes ou clique no menu de atalho (`...`).

1. Clique em **[!UICONTROL Exportar para ativação]** (caixa com a seta apontando para fora).

1. No pop-up _Exportar para ativação_, selecione um dos formatos disponíveis:

   - Email: `HTML`, `CSV`
   - Anúncios de meta e exibição: `HTML`, `JPEG`, `PNG`

Consulte [Ativação](/help/user-guide/activation/overview.md).

## Editar no Express

Você pode editar ativos de imagem (JPG ou PNG) diretamente no GenStudio for Performance Marketing usando o Adobe Express. A Tela _[!UICONTROL Powered by Adobe Express]_ fornece recursos convenientes para aprimorar suas imagens sem sair do aplicativo do GenStudio. É possível remover facilmente planos de fundo, aplicar preenchimentos gerativos, ajustar efeitos e recortar imagens.

>[!BEGINSHADEBOX]

Critérios para aprimorar imagens com o recurso [!DNL Edit in Adobe Express]:

- Os tipos MIME suportados incluem `image/png` e `image/jpeg`
- As dimensões mínimas da imagem são 50x50 pixels
- As dimensões máximas da imagem são 8000x8000 pixels
- O tamanho máximo é 40MB (40.000.000 bytes)

>[!ENDSHADEBOX]

**Para editar um ativo com o Express**:

1. Em _[!DNL Content]_, selecione um ativo de imagem. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição de ativos, clique no ícone **[!UICONTROL Editar no Adobe Express]** no canto superior direito.

1. Na Tela _[!UICONTROL Powered by Adobe Express]_, use os controles Expressos no painel esquerdo para aprimorar sua imagem.

1. Quando estiver satisfeito com a imagem atualizada, clique em **[!UICONTROL Salvar uma cópia]** no canto superior direito.

1. Selecione o formato de arquivo - JPG ou PNG - e clique em **[!UICONTROL Salvar uma cópia]**.

1. No pop-up _[!UICONTROL Salvar uma cópia do ativo]_, atualize o **[!UICONTROL Nome do ativo]**.

   - Selecione **[!UICONTROL Mesmos detalhes que o ativo original]** para transferir os detalhes do ativo para a nova imagem.

   - Expanda a seção **[!UICONTROL Mais detalhes]** para atualizar as diretrizes e outros metadados.

   >[!TIP]
   >
   >Quanto mais detalhes você fornecer, mais conhecerá os recursos avançados do GenStudio for Performance Marketing. Selecione um ou mais detalhes na lista ou insira um novo, onde aplicável, como com palavras-chave. Cada detalhe adicionado aparece abaixo da lista. Clique em **`x`** para remover um detalhe.

1. Clique em **[!UICONTROL Salvar]**.
