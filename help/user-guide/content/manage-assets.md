---
title: Gerenciar ativos e experiências
description: Simplifique e aprimore o gerenciamento de ativos aprovados pela marca para uso e reutilização em sua jornada de marketing digital.
feature: Content Management, Content Attributes
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: 1df977edbca284e67a5d28a6835bf5fc5608aa33
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 1%

---

# Gerenciar ativos e experiências

O Adobe GenStudio for Performance Marketing [!DNL Content] simplifica e aprimora o gerenciamento de ativos aprovados pela marca para uso e reutilização em sua jornada de marketing digital.

## Galeria [!DNL Content]

A galeria mostra um inventário de ativos, experiências ou modelos aprovados, dependendo da exibição selecionada. O botão de alternância de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar entre várias categorias para filtrar o conteúdo mostrado na galeria. No modo de exibição _[!UICONTROL Assets]_, clique no ícone de pesquisa (lupa) para usar uma palavra-chave para localizar um ativo.

A seguir, uma pesquisa sobre o termo `space` na galeria [!UICONTROL Assets]:

![exibição do Assets com pesquisa no espaço](/help/assets/content-assets-filter.png "Pesquisando ativos com atributo de espaço")

### Pesquisar conteúdo

O filtro e a interface de pesquisa são rápidos e responsivos e fornecem uma experiência produtiva de pesquisa. Cada exibição do [!DNL Content] fornece opções de filtro para restringir sua pesquisa pelo ativo, experiência ou modelo ideal. Para ativos e experiências, você pode selecionar uma campanha e diretrizes específicas, como o conteúdo criado para um produto específico.

Há filtros baseados em [diretrizes](/help/user-guide/guidelines/overview.md), [palavras-chave](asset-details.md#user-defined-metadata) e [categorias de atributo](/help/user-guide/insights/attributes.md#categories) para restringir os resultados da pesquisa. Por exemplo, talvez você queira encontrar um ativo de um tipo de arquivo ou assunto específico para ajudá-lo a criar uma nova experiência para sua campanha. Ou você pode filtrar o conteúdo com base no seu nome de usuário ou no nome de um membro da equipe:

- **[!UICONTROL Carregado por]**: limita a lista _[!UICONTROL Assets]_ para mostrar apenas os ativos carregados por você ou por uma pessoa específica.
- **[!UICONTROL Criado por]**: limita a lista _[!UICONTROL Experiências]_ para mostrar apenas as experiências criadas por você ou por uma pessoa específica.
- **[!UICONTROL Modelo]**: limita a lista _[!UICONTROL Experiências]_ para mostrar somente as experiências criadas com o modelo selecionado.

Se determinadas opções de filtro não estiverem visíveis, isso indicará que nenhum modelo no repositório corresponde aos critérios de metadados correspondentes. Verifique se os modelos estão marcados corretamente com metadados para torná-los detectáveis por meio desses filtros.

**Para pesquisar conteúdo a ser reutilizado**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Assets]**.

1. Selecione um repositório de ativos na lista **[!UICONTROL Local]** ou verifique se você está observando o repositório de ativos correto. `GenStudio assets` é o repositório padrão.

   >[!IMPORTANT]
   >
   >A lista _Local_ está disponível somente quando você [se conecta a um repositório do AEM](connect-aem-repo.md).

1. Clique em **[!UICONTROL Pesquisar]** (lupa) para inserir uma palavra-chave ou descrição.

1. Restrinja sua pesquisa selecionando uma categoria na lista _[!UICONTROL Filtro]_. Por exemplo, se você estiver procurando um arquivo PNG, clique em **[!UICONTROL Formato de arquivo]** e escolha **PNG**.

   Quanto mais você limitar sua pesquisa, menos opções de filtro estarão disponíveis. Clique em **[!UICONTROL Limpar tudo]** para remover todos os filtros.

1. Selecione um ativo para obter uma visualização completa e uma lista de detalhes.

   Clique em **[!UICONTROL Baixar]** (seta para baixo) para usar o ativo na sua estação de trabalho local.

### Local

Por padrão, os ativos adicionados a [!DNL Content] por meio do processo [!DNL Create] ou através de upload são armazenados no repositório `GenStudio assets`. O repositório `GenStudio assets` é um repositório leitura-gravação no GenStudio for Performance Marketing. Isso significa que você pode salvar, editar e excluir ativos no repositório `GenStudio assets`.

A lista **[!UICONTROL Local]** acima da galeria _[!UICONTROL Assets]_ à direita permite selecionar entre repositórios conectados do Adobe Experience Manager (AEM) [!DNL Assets Content Hub].

![Lista de locais de repositórios](/help/assets/content-location-selection.png "Selecione um repositório de conteúdo"){width="350"}

Quando você seleciona um repositório do AEM, a galeria mostra um inventário de ativos desse repositório, permitindo que você aproveite os ativos aprovados desses repositórios como entradas para a criação de conteúdo. As opções de filtro são alteradas para refletir as categorias configuradas em [!DNL AEM Assets Content Hub].

Consulte [Conectar um repositório do AEM](connect-aem-repo.md) para obter orientação sobre como adicionar seu repositório do [!DNL AEM Assets Content Hub] ao GenStudio for Performance Marketing.

O repositório do AEM é somente leitura, o que significa que você pode acessar o conteúdo, mas não pode salvar rascunhos, novos ativos ou metadados no repositório do AEM. Todos os rascunhos e atualizações finais para ativos, experiências e modelos são salvos no repositório do `GenStudio assets` com os novos [metadados do sistema](asset-details.md#system-metadata).

{{note-aem-assets}}

Um repositório do AEM pode aplicar determinados requisitos de licenciamento, como a expiração de ativos. Esses ativos podem não estar disponíveis para uso nos fluxos de trabalho do [!DNL Create]. Os ativos expirados podem precisar ser renovados ou substituídos para manter a continuidade dos projetos. Consulte o administrador do [!DNL AEM Assets Content Hub] para obter assistência com esses ativos.

## Gerenciamento do Assets

No [!UICONTROL Conteúdo], você pode armazenar, recuperar e gerenciar facilmente seus ativos digitais. Ao utilizar os repositórios `GenStudio assets` e AEM, é possível garantir que seus ativos estejam bem organizados e acessíveis para várias campanhas de marketing. Essa abordagem de vários repositórios oferece flexibilidade e controle sobre o uso de ativos em todos os ambientes, garantindo que somente ativos aprovados e atualizados sejam usados em esforços de marketing.

A tabela a seguir lista as tarefas de gerenciamento disponíveis para ativos, experiências e modelos:

| Tarefas | Ativos | Experiências | Modelos |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [Exibir detalhes](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [Criar experiência](/help/user-guide/create/overview.md) |        |             | ✓ |
| [Editar no Adobe Express](#edit-in-express) | ✓ |             |           |
| [Exportar experiências](#export-experiences) |        | ✓ |           |
| [Atualizar](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [Download](#download-assets) | ✓ |             | ✓ |
| [Excluir](#delete-assets) | ✓ | ✓ | ✓ |

### Adicionar ativos

Ao adicionar ativos ao [!DNL Content], eles são armazenados por padrão no repositório `GenStudio assets`. O botão _[!UICONTROL Adicionar ativos]_ está disponível somente quando o _[!UICONTROL Local]_ é o repositório `GenStudio assets`.

![Campo de localização](/help/assets/content-location.png "Campo de localização"){width="350"}

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

## Exportar experiências

É possível selecionar uma ou mais experiências aprovadas para download em um formato compatível com o canal de destino. O arquivo baixado é nomeado usando a data de exportação: `2025-06-15-export.zip`. Ao descompactar o arquivo, há uma pasta para cada tipo de canal que inclui os ativos exportados nos formatos selecionados. Cada ativo exportado retém o nome do ativo original como o nome do arquivo.

**Para exportar ou baixar experiências**:

1. Em _[!DNL Content]_, selecione uma ou mais experiências.

   Um banner é exibido com o número de experiências selecionadas à esquerda e as opções de [!UICONTROL Ativar], [!UICONTROL Baixar] ou [!UICONTROL Excluir] à direita.

1. (Opcional) Se optar por ativar, talvez você precise selecionar uma plataforma e continuar com o fluxo de trabalho [!DNL Activate]. Consulte [Ativar](/help/user-guide/activation/overview.md).

1. Clique em **[!UICONTROL Baixar]**.

1. No pop-up _Download_, selecione um dos formatos disponíveis.

   Se você selecionou várias experiências de canais diferentes, é possível selecionar o formato para cada tipo de canal.

   - Email, LinkedIn: `HTML`, `CSV`
   - Meta, banner e anúncio de exibição: `HTML`, `JPEG`, `PNG`

   ![Baixar experiências](/help/assets/content-bulk-export.png "Baixar várias experiências"){width=350}

## Editar no Express

Você pode editar ativos de imagem (JPG ou PNG) diretamente no GenStudio for Performance Marketing usando o Adobe Express. O Canvas _[!UICONTROL Powered by Adobe Express]_ fornece recursos convenientes para aprimorar suas imagens sem sair do aplicativo do GenStudio. É possível remover facilmente planos de fundo, aplicar preenchimentos gerativos, ajustar efeitos e recortar imagens.

>[!BEGINSHADEBOX]

Critérios para aprimorar imagens com o recurso [!DNL Edit in Adobe Express]:

- Os tipos MIME suportados incluem `image/png` e `image/jpeg`
- As dimensões mínimas da imagem são 50x50 pixels
- As dimensões máximas da imagem são 8000x8000 pixels
- O tamanho máximo é 40MB (40.000.000 bytes)

>[!ENDSHADEBOX]

**Para editar um ativo com o Express**:

1. Em _[!DNL Content]_, selecione um ativo de imagem. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição do ativo, clique no ícone **[!UICONTROL Editar no Adobe Express]** no canto superior direito.

1. Na Tela _[!UICONTROL Powered by Adobe Express]_, use os controles Expressos no painel esquerdo para aprimorar sua imagem.

1. Quando estiver satisfeito com a imagem atualizada, clique em **[!UICONTROL Salvar uma cópia]** no canto superior direito.

1. Selecione o formato de arquivo (JPG ou PNG) e clique em **[!UICONTROL Salvar uma cópia]**.

1. No pop-up _[!UICONTROL Salvar uma cópia do ativo]_, atualize o **[!UICONTROL Nome do ativo]**.

   - Selecione **[!UICONTROL Mesmos detalhes que o ativo original]** para transferir os detalhes do ativo para a nova imagem.

   - Expanda a seção **[!UICONTROL Mais detalhes]** para atualizar as diretrizes e outros metadados.

   >[!TIP]
   >
   >Quanto mais detalhes você fornecer, mais conhecerá os recursos avançados do GenStudio for Performance Marketing. Selecione um ou mais detalhes na lista ou insira um novo, onde aplicável, como com palavras-chave. Cada detalhe adicionado aparece abaixo da lista. Clique em **`x`** para remover um detalhe.

1. Clique em **[!UICONTROL Salvar]**.
