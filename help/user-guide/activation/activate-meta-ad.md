---
title: Ativar um meta anúncio
description: Saiba como ativar uma experiência de Metadados.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 8e61fa5c08102c5dd9905e693d7f129105d9f633
workflow-type: tm+mt
source-wordcount: '1372'
ht-degree: 1%

---

# Ativar um meta anúncio

O Adobe GenStudio for Performance Marketing é compatível com a ativação de Meta ads, ou criativos, para o Instagram e o Facebook.

Você pode [criar uma Metaexperiência](/help/user-guide/create/create-meta-ad.md) no GenStudio for Performance Marketing e selecioná-la para ativação ou criar uma nova experiência a partir de ativos aprovados em [!DNL Activate].

A ativação de um Metadado segue as [mesmas etapas gerais](create-activation.md) necessárias para a ativação em outros canais pagos. O processo de ativação permite preparar suas experiências de anúncio para os requisitos específicos do Meta. Depois de ativar uma experiência Meta, ou um criativo, no GenStudio for Performance Marketing, use o [Gerenciador de Metads](https://adsmanager.facebook.com/) para ajustar a experiência para inserções específicas de metaanúncios antes da publicação final.

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

**Para preparar suas experiência para o ativação**:

1. A partir de _[!DNL Activate]_então, clique **[!UICONTROL Novo]**no mosaico de metadados. A_ visualização de configuração _Creative é aberta.

   A página de configuração do Creative fornece um local central para preparar a ativação do Meta ad. A preparação do anúncio inclui estas três tarefas:

1. Atribua um nome à sua experiência. Após a ativação, você poderá usar esse nome para procurar essa experiência na tabela _Experiências ativadas_.
1. Selecione ativos de mídia. Você pode usar ativos de Conteúdo ou carregar ativos externos (por exemplo, do OneDrive ou do Dropbox).
1. [Adicionar texto](#add-ad-text).
1. [Adicionar metadados](#assign-metadata).

   O _painel de Visualização_ oferece suporte a uma exibição interativa do seu texto e dos seus ativos no contexto de um posicionamento de anúncio específico. Use o menu suspenso _Selecionar posicionamento_ para alternar entre os posicionamentos de anúncios com suporte. As visualizações fornecem a oportunidade de finalizar decisões sobre elementos de anúncios para disposições específicas. Ao selecionar um posicionamento no painel _Visualização_, somente a exibição do anúncio será afetada. Sua seleção de posicionamento no painel _Visualização_ não foi salva.

### Selecione seus ativos de mídia

Use a _seção Mídia_ para selecionar pelo menos uma imagem ativo para incluir no experiência. As disposições de anúncios estão associadas às taxas de proporção de imagem suportadas, que são listadas como opções no _menu suspenso Posições_ . Esse menu exibe as disposições de publicidade suportadas para postagens do Facebook ou histórias do Instagram, organizadas por proporção de aspecto.

Após upload, ativos são salvas _[!DNL Content]_em . A_&#x200B;área mídia _exibe a imagem por padrão com uma taxa de proporção de 1:1. As taxas de proporção alternativas incluem apenas os valores suportados pelo publicidade pago canal. Eles são agrupados por orientação vertical e horizontal. GenStudio para Marketing de desempenho suporta a inclusão de até seis taxas de proporção por experiência ativado.

**Para upload um ativo de Conteúdo**:

O _[!DNL Content]_fornece uma exibição central para os ativos e experiências aprovados da sua organização. Você pode focalizar o inventário de ativos exibido na galeria[_[!DNL Content]_](/help/user-guide/content/manage-assets.md) usando as opções de menu **[!UICONTROL Pesquisar]** (lupa) e _Filtrar_.

1. De _[!DNL Activate]_, clique em **[!UICONTROL Novo]**no bloco de Meta Ads. A exibição_ Configuração do Creative _é aberta.

1. Clique em **[!UICONTROL Selecionar]** e selecione **[!UICONTROL Selecionar do Conteúdo]**. A exibição _Selecionar conteúdo_ é aberta, exibindo uma galeria de ativos de imagem que você pesquisa ou filtra.

1. Use as ferramentas de pesquisa e filtro da galeria _[!DNL Content]_para selecionar pelo menos um ativo para carregamento.

1. Clique em **[!UICONTROL Usar]** para incluir o ativo selecionado no criativo. A janela _Configuração do Creative_ inclui o ativo em sua proporção padrão na área _Mídia_. O painel _Visualização_ visualiza o ativo no posicionamento do anúncio que dá suporte a essa taxa de proporção.

Se o upload não for bem-sucedido, uma mensagem de erro informativa que inclui um link para o ativo em _[!DNL Content]_será aberta.

**Para carregar um ativo externo**:

Você pode carregar até seis imagens estáticas externas para a galeria _[!DNL Content]_do Microsoft OneDrive ou do Dropbox.

1. De _[!DNL Activate]_outra forma, clique **[!UICONTROL Novo]**no bloco Meta. A_ janela de configuração _do Creative é aberta.

1. _Na seção Mídia_, clique **[!UICONTROL em Selecionar]**. Um menu suspenso exibe opções para _Selecionar a partir de Conteúdo_ ou _Fazer upload_.

1. Clique em **[!UICONTROL Fazer upload]**.A _janela Adicionar proporções de proporção_ é aberta.

1. Selecione imagens nas proporções de aspecto compatíveis arrastando e soltando arquivos de imagem na área de upload imagem. Como alternativa, você pode procurar ativos no seu dispositivo.

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
| Exibir URL | Não | 1000 |
| URL do site | sim | 1000 |
| Imagem | é necessário pelo menos um |                                 |

_Texto primário_ e _título_ são exigidos apenas pelo GenStudio for Performance Marketing, não pelo Meta.

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

## Etapa 4: confirmar configuração de meta conta

Depois de preparar sua criativo, você deve confirmar suas informações de Meta conta e atribuir um ID de rastreamento ao experiência publicidade. A _configuração visualização de configuração_ do Meta publicidade é preenchida com opções derivadas das contas Meta configuradas.

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

### Ativação completa da sua experiência com anúncios

Clique em **[!UICONTROL Publicar]**. A experiência completa do Meta Ads e seus metadados associados são enviados diretamente para o conjunto de anúncios do Gerenciador de metadados selecionado. As experiências são entregues ao Gerenciador de metadados inativado. No Gerenciador de metadados, é possível gerenciar as etapas finais de implantação da experiência de publicidade e da campanha Meta.

### Faça logon no Gerenciador de metadados para concluir a ativação

Depois que a ativação for concluída, você deverá fazer logon no Gerenciador de metadados. No [Meta Ads Manager](https://adsmanager.facebook.com/), você pode revisar sua experiência com anúncios e finalizar a publicação em canais Meta específicos.
