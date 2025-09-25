---
title: Ativar um anúncio do Meta
description: Saiba como ativar uma experiência de anúncio do Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '1907'
ht-degree: 1%

---

# Ativar um anúncio do Meta

O Adobe GenStudio for Performance Marketing oferece suporte à ativação de experiências de anúncios do Meta para o Instagram e o Facebook.

Você pode [criar uma experiência do Meta](/help/user-guide/create/create-meta-ad.md) no GenStudio for Performance Marketing e selecioná-la para ativação ou criar uma nova experiência a partir de ativos aprovados em [!DNL Activate].

A ativação de um anúncio Meta segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais pagos. O processo de ativação permite preparar sua experiência de anúncio para os requisitos específicos do Meta. Depois de ativar uma experiência do Meta no GenStudio for Performance Marketing, use o [Meta Ads Manager](https://adsmanager.facebook.com/) para ajustar a experiência para inserções específicas de anúncios do Meta antes da publicação final.

Os gerentes e editores de sistema da GenStudio podem ativar experiências de anúncios.

## Etapa 1: configurar as contas do Meta

Antes de iniciar uma ativação, [faça logon no Meta](https://adsmanager.facebook.com/) para acessar sua conta do Meta Ads Manager.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

Confirme se suas contas de anúncio conectadas do Meta têm permissão total para gerenciar anúncios nestes componentes da plataforma de publicidade da Meta:

* Página do Facebook
* Campanha do Meta
* Conjunto de anúncios do Meta
* Perfil do Instagram (opcional)

>[!ENDSHADEBOX]

## Etapa 2: conectar-se às contas do Meta

Antes que sua organização possa ativar experiências, um gerente de sistema da GenStudio deve conectar suas contas da Meta à GenStudio for Performance Marketing. Essa conexão permite que os dados fluam entre o GenStudio e as ferramentas de marketing externas, como o Meta, habilitando o processo de ativação.

Consulte [Conectar-se ao Meta Ads](/help/user-guide/connectors/meta-ads.md).

Após a conclusão da sincronização, você poderá visualizar as contas adicionadas. Grandes quantidades de dados levam mais tempo para sincronizar.

## Etapa 3: Prepare sua experiência para ativação

Você pode iniciar uma ativação de duas maneiras:

* **Ativar diretamente de[!DNL Content]**. Selecionar uma experiência aprovada com configurações predefinidas é a maneira mais simples de iniciar uma ativação em um único canal.

* **Combine sua experiência com anúncios em [!DNL Activate] > _Configuração de experiência_**. Você pode criar uma experiência selecionando ativos visuais de [!DNL Content], adicionando elementos de texto e selecionando taxas de proporções. Essa abordagem tem mais etapas, mas oferece maior flexibilidade ao criar sua experiência criativa.

### Ativar uma experiência aprovada pelo Conteúdo

Você pode selecionar mais de uma experiência para ativar em um único canal pago. Talvez seja necessário selecionar uma plataforma antes de continuar com a ativação.

Se você selecionou mais de uma experiência para ativar como grupo, use a barra lateral esquerda para focalizar a exibição _Configuração da experiência_ nos detalhes da experiência selecionada.

1. Use as ferramentas de pesquisa e filtro da galeria [!DNL Content] para identificar a experiência que você deseja ativar e clique em **[!UICONTROL Ativar]**.

   A página _Configuração da experiência_ dos anúncios do Meta é aberta para esta experiência. Ela é pré-preenchida com detalhes da experiência selecionada. Você pode editar os campos **[!UICONTROL Call-to-action]**, **[!UICONTROL URL do site]** e **[!UICONTROL Exibir link]**. Se você selecionar mais de uma experiência para ativar, a exibição _Configuração da experiência_ incluirá uma barra lateral esquerda que exibirá miniaturas de todas as experiências selecionadas. Use esta barra lateral esquerda para focalizar a exibição _Configuração da experiência_ nos detalhes da experiência selecionada.

1. Selecione uma campanha no menu suspenso **[!UICONTROL Campanhas]**.

   Se estiver trabalhando com várias experiências, alterne pelas experiências na barra lateral esquerda até concluir a preparação de cada experiência.

1. Clique em **[!UICONTROL Avançar]** para confirmar a configuração dos anúncios do Meta.

1. Atribua um nome a cada experiência. Após a ativação, você poderá usar esse nome para procurar essa experiência na tabela _Experiências ativadas_.

### Montar componentes de experiência

Se você optar por não ativar diretamente uma experiência aprovada do [!DNL Content], poderá selecionar ativos, atribuir taxas de proporção e rascunhar elementos de texto.

**Para preparar sua experiência para a ativação**:

1. De [!DNL Activate], clique em **[!UICONTROL Novo]** no ícone que representa o canal pago escolhido. A exibição _Configuração de experiência_ é aberta.

   A página _Configuração da experiência_ fornece um local central para preparar a ativação de seus anúncios. A preparação do anúncio inclui estas três tarefas:

1. Atribua um nome à sua experiência. Após a ativação, você poderá usar esse nome para procurar essa experiência na tabela _Experiências ativadas_.
1. Selecione ativos de mídia. Você pode usar ativos de [!DNL Content] ou carregar ativos externos (por exemplo, do OneDrive ou Dropbox).
1. [Adicionar texto](#add-ad-text).
1. [Adicionar metadados](#assign-metadata).

   O _painel de Visualização_ oferece suporte a uma exibição interativa do seu texto e dos seus ativos no contexto de um posicionamento de anúncio específico. Use o menu suspenso _Selecionar posicionamento_ para alternar entre os posicionamentos de anúncios com suporte. As visualizações fornecem a oportunidade de finalizar decisões sobre elementos de anúncios para disposições específicas. Ao selecionar um posicionamento no painel _Visualização_, somente a exibição do anúncio será afetada. Sua seleção de posicionamento no painel _Visualização_ não foi salva.

### Selecione seus ativos de mídia

Use a seção _Mídia_ para selecionar pelo menos um ativo de imagem a ser incluído na sua experiência. Os posicionamentos de anúncios estão associados a proporções de imagem com suporte, que estão listadas como opções no menu suspenso _Posicionamentos_. Esse menu exibe os posicionamentos de anúncios compatíveis com postagens do Facebook ou histórias do Instagram, organizados por taxa de proporção.

Após o carregamento, os ativos são salvos em [!DNL Content]. A área _Mídia_ exibe a imagem por padrão com uma proporção de 1:1. As taxas de aspecto alternativas incluem apenas os valores compatíveis com o canal de anúncios pagos. Eles são agrupados por orientação vertical e horizontal. O GenStudio for Performance Marketing oferece suporte à inclusão de até seis taxas de aspecto por experiência ativada.

**Para carregar um ativo do Conteúdo**:

O [!DNL Content] fornece uma exibição central para os ativos e experiências aprovados da sua organização. Você pode focalizar o inventário de ativos exibido da [[!DNL Content] galeria](/help/user-guide/content/manage-assets.md) usando as opções de menu **[!UICONTROL Pesquisar]** (lupa) e _Filtro_.

1. Em [!DNL Activate], clique em **[!UICONTROL Novo]** no cartão do canal. A exibição _Configuração de experiência_ é aberta.

1. Clique em **[!UICONTROL Selecionar]** e selecione **[!UICONTROL Selecionar do Conteúdo]**. A exibição _Selecionar conteúdo_ é aberta, exibindo uma galeria de ativos de imagem que você pesquisa ou filtra.

1. Use as ferramentas de pesquisa e filtro da galeria [!DNL Content] para selecionar pelo menos um ativo para carregamento.

1. Clique em **[!UICONTROL Usar]** para incluir o ativo selecionado na sua experiência com anúncios. A janela _Configuração de experiência_ inclui o ativo em sua taxa de proporção padrão na área _Mídia_. O painel _Visualização_ visualiza o ativo no posicionamento do anúncio que dá suporte a essa taxa de proporção.

Se o upload não for bem-sucedido, uma mensagem de erro informativa que inclui um link para o ativo em _[!DNL Content]_&#x200B;será aberta.

**Para carregar um ativo externo**:

Você pode carregar até seis imagens estáticas externas para a galeria [!DNL Content] do Microsoft OneDrive ou do Dropbox.

1. Em [!DNL Activate], clique em **[!UICONTROL Novo]** no bloco do Meta. A janela _Configuração da experiência_ é aberta.

1. Na seção _Mídia_, clique em **[!UICONTROL Selecionar]**. Um menu suspenso exibe opções para _Selecionar Conteúdo_ ou _Carregar_.

1. Clique em **[!UICONTROL Fazer upload]**. A janela _Adicionar taxas de proporção_ é aberta.

1. Selecione imagens nas taxas de proporções compatíveis arrastando e soltando arquivos de imagem na área de upload de imagem. Como alternativa, você pode procurar ativos no seu dispositivo.

1. (Opcional) Para carregar ativos do seu dispositivo, clique em **[!UICONTROL Procurar]** e selecione _Procurar arquivos_ ou _Procurar pastas_ para identificar ativos a serem carregados.

1. Na área _Adicionar detalhes_, adicione detalhes informativos aos ativos carregados para facilitar a pesquisa e a filtragem no _[!DNL Content]_. Esses detalhes são salvos como metadados.

1. Depois de carregar seus ativos e atribuir detalhes, clique em **[!UICONTROL Adicionar Assets]** na parte inferior direita.

### Adicionar texto de anúncio

Use a seção _Texto_ da página _Ativar anúncio do Meta_ para adicionar texto convincente e compatível com a marca aos campos de texto necessários. O texto inclui o texto principal (corpo) do anúncio e do call-to-action. Você não pode editar os campos _Texto primário_, _Títulos_ e _Descrição_. Você pode editar os campos _Call-to-action_, _Exibir link_ e _URL do site_.

| Texto | Obrigatório | Limite de caracteres (máximo) |
|-----------------|---------------------------|---------------------------------|
| Nome do anúncio | sim | 500 |
| Texto primário | sim | 500 |
| Título | sim | 255 |
| Descrição | não | 125 |
| Call to action | sim | somente opções do menu suspenso |
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

Depois de reunir ou selecionar sua experiência, clique em **[!UICONTROL Avançar]** para confirmar a instalação do Meta.

## Etapa 4: confirmar configuração de conta do Meta

Depois de preparar suas experiências de anúncio, você deve confirmar as informações de sua conta do Meta. A exibição _Anúncio do Meta_ é preenchida com opções que são derivadas das contas do Meta configuradas.

| Detalhe | Descrição |
|------------|-------------|
| Contas | Contas do Meta que foram conectadas ao GenStudio for Performance Marketing |
| Página do Facebook | Página do Facebook onde a experiência é publicada |
| Conta do Instagram | Contas do Instagram que foram conectadas ao GenStudio for Performance Marketing |
| Campanhas | Campanhas do Meta às quais a experiência de anúncio pertence |
| Conjuntos de anúncios | Conjuntos de anúncios do Meta aos quais a experiência de anúncio ativada pertence. As configurações determinam os posicionamentos finais do anúncio. |

### Criar um novo conjunto de anúncios

Você pode criar um novo conjunto de anúncios durante a configuração da plataforma clonando um conjunto de anúncios existente durante a configuração da plataforma. Os conjuntos de metadados definem o tempo, os detalhes do canal e o público-alvo de um anúncio específico. Uma Meta campanha pode conter vários conjuntos de anúncios, mas um conjunto de anúncios é associado exclusivamente a uma campanha.

**Para criar um novo conjunto de anúncios**:

1. Selecione uma campanha no menu suspenso _Campanhas do Meta_.

   A campanha selecionada determina os conjuntos de anúncios disponíveis como opções no menu suspenso _Conjuntos de anúncios_.

1. Clique em **[!UICONTROL + Criar novo conjunto de anúncios]**.

   O pop-up _Criar novo conjunto de anúncios_ é aberto, identificando a campanha do Meta em que o novo conjunto de anúncios é criado.

1. Selecione o conjunto de anúncios que deseja clonar no menu suspenso _Usar configuração de_.

   O GenStudio for Performance Marketing atribui um nome de conjunto de anúncios padrão ao anexar `- Copy` ao nome de conjunto de anúncios selecionado.

1. (Opcional, mas recomendado) Insira um nome de anúncio exclusivo no campo **[!UICONTROL Nome do novo conjunto de anúncios]** para substituir o valor padrão.

1. Clique em **[!UICONTROL Criar conjunto de anúncios]**.

   Você retornará à exibição _Configuração da plataforma_, na qual o novo conjunto de anúncios é pré-selecionado. Uma mensagem de sucesso é exibida, incluindo um link para o anúncio definido no Meta Ads Manager. Este conjunto de anúncios está disponível para ativações futuras.

>[!NOTE]
>
>Se o conjunto de anúncios for criado com êxito, mas não for possível salvar o nome do conjunto de anúncios, o conjunto de anúncios será salvo no Meta Ads Manager com o nome padrão (_nome do conjunto de anúncios original - Cópia_).

### ID de rastreamento

As IDs de rastreamento (nome do anúncio) fornecem um mecanismo para coletar métricas vinculadas ao desempenho da experiência. Digite o nome do anúncio neste campo.

Clique em **[!UICONTROL Avançar]** no canto superior direito para visualizar sua experiência com anúncios e finalizar a ativação.

## Etapa 5: visualize e ative seu anúncio

A página _Revisão_ exibe sua experiência de anúncio conforme reunido na _Configuração da experiência_ e fornece uma oportunidade final de visualizar e editar sua experiência. Clique em **[!UICONTROL Editar seção]** ao lado do rótulo _Configuração da experiência_ para fazer as alterações. Você também pode clicar em **[!UICONTROL Voltar]** no canto superior direito para retornar à página _Configuração da experiência_.

### Etapa 6: conclua a ativação de sua experiência de anúncio

1. Clique em **[!UICONTROL Publicar]**.

   A experiência completa de anúncios do Meta e seus metadados associados são enviados diretamente para o conjunto de anúncios selecionado do Meta Ads Manager. As experiências são entregues ao Meta Ads Manager no estado inativo. No Meta Ads Manager, é possível gerenciar as etapas finais da implantação da experiência de anúncio e da campanha do Meta.

1. [Faça logon no Meta Ads Manager](https://adsmanager.facebook.com/) para analisar sua experiência com anúncios e finalizar a publicação em canais específicos da Meta.
