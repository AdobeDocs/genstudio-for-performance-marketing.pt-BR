---
title: Ativar um meta anúncio
description: Saiba como ativar uma experiência de Metadados.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 19f36badd66a5dc90585b4399b87230847474a81
workflow-type: tm+mt
source-wordcount: '1356'
ht-degree: 1%

---

# Ativar um meta anúncio

O Adobe GenStudio for Performance Marketing é compatível com a ativação de Meta ads, ou criativos, para o Instagram e o Facebook.

Você pode [criar uma Metaexperiência](/help/user-guide/create/create-meta-ad.md) no GenStudio for Performance Marketing e selecioná-la para ativação ou criar uma nova experiência a partir de ativos aprovados em [!DNL Activate].

A ativação de um Metadado segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais pagos. O processo de ativação permite preparar sua experiência criativa a partir de anúncios para os requisitos específicos do Meta. Depois de ativar uma experiência Meta, ou um criativo, no GenStudio for Performance Marketing, use o [Gerenciador de Metads](https://adsmanager.facebook.com/) para ajustar a experiência para inserções específicas de metaanúncios antes da publicação final.

## Etapa 1: configurar suas contas Meta

Antes de iniciar uma ativação, [faça logon no Meta](https://adsmanager.facebook.com/) para acessar sua conta do Gerenciador de Metadados. Confirme se as contas conectadas do MetaAd incluem:

* Página do Facebook
* Meta campaign
* Conjunto de metadados
* Perfil do Instagram (opcional)

Você deve ter permissão para publicar conteúdo no Gerenciador de metadados.

## Etapa 2: conectar-se às suas contas Meta

Antes que sua organização possa ativar experiências, um gerente de sistema da GenStudio precisa conectar suas contas Meta à GenStudio for Performance Marketing. Essa conexão permite que os dados fluam entre o GenStudio e as ferramentas de marketing externas, como o Meta, permitindo os processos de ativação.

Consulte [Conectar-se a uma conta Meta (Facebook)](/help/user-guide/connectors/connect-channel.md#meta-ads-connect).

Após a conclusão da sincronização, você poderá visualizar as contas adicionadas. Grandes quantidades de dados levam mais tempo para sincronizar.

## Etapa 3: Prepare sua experiência para ativação

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

**Para preparar sua experiência para a ativação**:

1. Em _[!DNL Activate]_, clique em **[!UICONTROL Novo]**no bloco de produtos Meta. A exibição_ Configuração do Creative _é aberta.

   A página de configuração do Creative fornece um local central para preparar a ativação do Meta ad. A preparação do anúncio inclui estas três tarefas:

1. Atribua um nome à sua experiência. Após a ativação, você poderá usar esse nome para procurar essa experiência na tabela _Experiências ativadas_.
1. Selecione ativos de mídia. Você pode usar ativos de Conteúdo ou carregar ativos externos (por exemplo, do OneDrive ou do Dropbox).
1. [Adicionar texto](#add-ad-text).
1. [Adicionar metadados](#assign-metadata).

   O _painel de Visualização_ oferece suporte a uma exibição interativa do seu texto e dos seus ativos no contexto de um posicionamento de anúncio específico. Use o menu suspenso _Selecionar posicionamento_ para alternar entre os posicionamentos de anúncios com suporte. As visualizações fornecem a oportunidade de finalizar decisões sobre elementos de anúncios para disposições específicas. Ao selecionar um posicionamento no painel _Visualização_, somente a exibição do anúncio será afetada. Sua seleção de posicionamento no painel _Visualização_ não foi salva.

### Selecione seus ativos de mídia

Use a seção _Mídia_ para selecionar pelo menos um ativo de imagem a ser incluído na sua experiência. Os posicionamentos de anúncios estão associados a proporções de imagem com suporte, que estão listadas como opções no menu suspenso _Posicionamentos_. Esse menu exibe os posicionamentos de anúncios compatíveis com postagens do Facebook ou histórias do Instagram, organizados por taxa de proporção.

Após o carregamento, os ativos são salvos em _[!DNL Content]_. A área_ Mídia _exibe a imagem por padrão com uma taxa de proporção de 1:1. As taxas de aspecto alternativas incluem apenas os valores compatíveis com o canal de anúncios pagos. Eles são agrupados por orientação vertical e horizontal. O GenStudio for Performance Marketing oferece suporte à inclusão de até seis taxas de aspecto por experiência ativada.

**Para carregar um ativo do Conteúdo**:

O _[!DNL Content]_fornece uma exibição central para os ativos e experiências aprovados da sua organização. Você pode focalizar o inventário de ativos exibido na galeria[_[!DNL Content]_](/help/user-guide/content/manage-assets.md) usando as opções de menu **[!UICONTROL Pesquisar]** (lupa) e _Filtrar_.

1. De _[!DNL Activate]_, clique em **[!UICONTROL Novo]**no bloco de Meta Ads. A exibição_ Configuração do Creative _é aberta.

1. Clique em **[!UICONTROL Selecionar]** e selecione **[!UICONTROL Selecionar do Conteúdo]**. A exibição _Selecionar conteúdo_ é aberta, exibindo uma galeria de ativos de imagem que você pesquisa ou filtra.

1. Use as ferramentas de pesquisa e filtro da galeria _[!DNL Content]_para selecionar pelo menos um ativo para carregamento.

1. Clique em **[!UICONTROL Usar]** para incluir o ativo selecionado no criativo. A janela _Configuração do Creative_ inclui o ativo em sua proporção padrão na área _Mídia_. O painel _Visualização_ visualiza o ativo no posicionamento do anúncio que dá suporte a essa taxa de proporção.

Se o upload não for bem-sucedido, uma mensagem de erro informativa que inclui um link para o ativo em _[!DNL Content]_será aberta.

**Para carregar um ativo externo**:

Você pode carregar até seis imagens estáticas externas para a galeria _[!DNL Content]_do Microsoft OneDrive ou do Dropbox.

1. Em _[!DNL Activate]_, clique em **[!UICONTROL Novo]**no bloco Meta. A janela_ Configuração do Creative _é aberta.

1. Na seção _Mídia_, clique em **[!UICONTROL Selecionar]**. Um menu suspenso exibe opções para _Selecionar Conteúdo_ ou _Carregar_.

1. Clique em **[!UICONTROL Fazer upload]**. A janela _Adicionar taxas de proporção_ é aberta.

1. Selecione imagens nas taxas de proporções compatíveis arrastando e soltando arquivos de imagem na área de upload de imagem. Como alternativa, você pode procurar ativos no seu dispositivo.

1. (Opcional) Para carregar ativos do seu dispositivo, clique em **[!UICONTROL Procurar]** e selecione _Procurar arquivos_ ou _Procurar pastas_ para identificar ativos a serem carregados.

1. Na área _Adicionar detalhes_, adicione detalhes informativos aos ativos carregados para facilitar a pesquisa e a filtragem no _[!DNL Content]_. Esses detalhes são salvos como metadados.

1. Depois de carregar seus ativos e atribuir detalhes, clique em **[!UICONTROL Adicionar Assets]** na parte inferior direita.

### Adicionar texto de anúncio

Use a seção _Texto_ da página _Ativar Metadado_ para adicionar texto atraente e que siga a marca aos campos de texto necessários. O texto inclui o texto principal (corpo) do anúncio e o texto da frase de chamariz.

| Texto | Obrigatório | Limite de caracteres (máximo) |
|-----------------|---------------------------|---------------------------------|
| Nome do anúncio | sim | 500 |
| Texto primário | sim | 500 |
| Título | sim | 255 |
| Descrição | não | 125 |
| Chamada para ação | sim | somente opções do menu suspenso |
| Exibir URL | não | 1000 |
| URL do site | sim | 1000 |
| Imagem | é necessário pelo menos um |                                 |

O GenStudio for Performance Marketing requer _Texto primário_ e _título_, não Meta.

### Atribuir metadados

Os detalhes da experiência são salvos como metadados e ajudam os usuários a pesquisar por uma experiência. Esses detalhes aumentam a visibilidade da experiência no [!DNL Content]. Use esses detalhes opcionais definidos pelo usuário para identificar a finalidade da experiência e o contexto, ou as campanhas, nas quais ela é implantada.

| Detalhe | Descrição |
|------------|-------------|
| Campanhas | Todas as campanhas do GenStudio for Performance Marketing às quais a experiência de anúncio pertence |
| Marca | Diretrizes, definidas pelo usuário ou padrão, que permitem aos usuários estabelecer diretrizes de marca, capturando a essência da identidade de uma marca. |
| Produtos | Produtos associados à sua organização e identificados na GenStudio for Performance Marketing |
| Personas | Pessoas associadas à sua organização e identificadas no GenStudio for Performance Marketing |
| Cronograma | O trimestre, a estação, o ano ou outra unidade de tempo definida organizacionalmente durante a qual a experiência do anúncio está ativa |
| Região | Região geográfica na qual a experiência é iniciada |
| Idioma | Idiomas para os quais a experiência de anúncio é usada |
| Palavras-chave | Palavras-chave definidas pelo usuário que facilitam a pesquisa e a categorização da experiência de anúncio |

Depois de reunir o criativo, clique em **[!UICONTROL Avançar]** para confirmar a configuração do Meta.

## Etapa 4: Confirmar configuração da conta Meta

Depois de preparar o criativo, você deve confirmar as informações da conta Meta e atribuir uma ID de rastreamento à experiência de anúncio. A exibição _Configuração de metadados_ foi preenchida com opções derivadas das contas Meta configuradas.

| Detalhe | Descrição |
|------------|-------------|
| Contas | Metacontas que foram conectadas ao GenStudio for Performance Marketing |
| Página do Facebook | Página do Facebook onde a experiência é publicada |
| Conta do Instagram | Contas do Instagram que foram conectadas ao GenStudio for Performance Marketing |
| Campanhas | Meta campanhas às quais a experiência de anúncio pertence |
| Conjuntos de anúncios | Conjuntos de metadados aos quais a experiência de anúncio ativada pertence. As configurações determinam os posicionamentos finais do anúncio. |

### ID de rastreamento

As IDs de rastreamento (nome do anúncio) fornecem um mecanismo para coletar métricas vinculadas ao desempenho da experiência. Digite o nome do anúncio neste campo.

Clique em **[!UICONTROL Avançar]** no canto superior direito para visualizar sua experiência com anúncios e finalizar a ativação.

## Etapa 5: visualize e ative seu anúncio

A página _Revisão_ exibe sua experiência de anúncio conforme reunido na _configuração do Creative_ e fornece uma oportunidade final de visualizar e editar sua experiência. Clique em **[!UICONTROL Editar seção]** ao lado do rótulo _Configuração do Creative_ para fazer as alterações. Você também pode clicar em **[!UICONTROL Voltar]** no canto superior direito para retornar à página _Configuração do Creative_.

### Etapa 6: conclua a ativação de sua experiência de anúncio

1. Clique em **[!UICONTROL Publicar]**.

   A experiência completa do Meta Ads e seus metadados associados são enviados diretamente para o conjunto de anúncios do Gerenciador de metadados selecionado. As experiências são entregues ao Gerenciador de metadados em um estado inativo. No Gerenciador de metadados, é possível gerenciar as etapas finais de implantação da experiência de publicidade e da campanha Meta.

1. [Faça logon no Gerenciador de Metadados](https://adsmanager.facebook.com/) para analisar sua experiência de publicidade e finalizar a publicação em canais Meta específicos.
