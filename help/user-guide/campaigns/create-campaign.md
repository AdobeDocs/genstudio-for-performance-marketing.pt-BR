---
title: Campanhas do Adobe GenStudio for Performance Marketing
description: Saiba como criar e gerenciar campanhas de marketing digital que aproveitam os ativos e as experiências de IA gerativa.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."
source-git-commit: edbeb7f0d08e2215a23f15cfeff77a5217cd264b
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Criar uma campanha

Uma campanha do GenStudio for Performance Marketing define as principais características da campanha digital e evolui à medida que os estágios são implantados e avaliados. O GenStudio for Performance Marketing apoia o processo dinâmico de lançar uma campanha, rastrear o desempenho de componentes individuais da campanha e redirecionar experiências de anúncio com base em métricas de desempenho.

Os principais elementos da campanha são armazenados em um objeto de campanha, o que cria um contexto compartilhado para todos os ativos e experiências rotulados com o mesmo nome de campanha exclusivo. Este rótulo identifica a campanha no GenStudio for Performance Marketing.

Os gerentes de sistema da GenStudio e editores do Genstudio podem criar campanhas.

## Definir detalhes da campanha

{{$include /help/_includes/campaign-details.md}}


**Para inserir detalhes da campanha**:

1. De [!DNL Campaigns], clique em **[!UICONTROL Adicionar campanha]**. A visualização _Criar uma campanha_ é aberta.

   Os detalhes incluem campos opcionais e obrigatórios que definem a campanha. Esses detalhes são salvos em [!DNL Campaigns] como atributos de metadados da campanha.

1. Clique duas vezes no cabeçalho _Nova campanha_ e insira um nome informativo e exclusivo.

   Este nome se torna um _rótulo de campanha_ no GenStudio for Performance Marketing, permitindo associar ativos ou experiências à campanha durante o carregamento e a criação.

1. Insira valores nos campos _Detalhes_ que descrevem sua campanha. Consulte a tabela _Detalhes da campanha_ para obter as definições desses recursos de campanha.

## Atribuir canais e regiões

As configurações de canal e região determinam onde a campanha é implantada e seus canais de distribuição.

O GenStudio for Performance Marketing usa modelos predefinidos chamados _registros_ para representar os principais componentes da campanha, como canais, regiões, perfis e produtos. Ao criar uma campanha, você a associa aos registros relevantes para cada um desses componentes.

* **Configurações de canal** — Define os canais de distribuição públicos da sua campanha, incluindo contas de mídia pagas, serviços de marketing por email e redes de anúncios de exibição. Os dados sobre o desempenho de campanhas, ativos e experiências nesses canais são alimentados no [[!DNL Insights]](/help/user-guide/insights/overview.md) para análise específica do canal.

* **Configurações de região** — Especifica as áreas geográficas nas quais você implanta sua campanha. Conectando-se a fontes de dados regionais, o GenStudio for Performance Marketing pode adaptar o conteúdo e a estratégia às preferências do público-alvo local. Isso permite um direcionamento e uma análise de desempenho mais precisos com base em métricas regionais.

**Para selecionar canais de distribuição para sua campanha**:

1. Clique no sinal + (**[!UICONTROL Conectar registros +]**) ao lado de **[!UICONTROL Canais]**.

   A janela pop-up _Selecionar Canais_ é aberta.

1. Selecione os canais nos quais a campanha é implantada. Os valores válidos incluem `Email`, `Paid media`, `Web` e `Display ads`.

   Opcionalmente, escolha **[!UICONTROL Ver tudo]** para abrir um modo de exibição de todos os canais com suporte.

**Para atribuir regiões à sua campanha**:

1. Clique no sinal + (**[!UICONTROL Conectar registros +]**) ao lado de **[!UICONTROL Regiões]**.

   O pop-up _Selecionar regiões_ é aberto. Você pode pesquisar por uma região suportada específica.

1. Selecione as regiões uma ou mais regiões de destino para sua campanha. As regiões válidas incluem `AMER`, `LATAM`, `EMEA`, `APAC` e `Japan`.

   Opcionalmente, escolha **[!UICONTROL Ver tudo]** para abrir uma exibição de todas as regiões com suporte.

## Atribuir personalidades e produtos

[Personalidades](/help/user-guide/guidelines/personas.md) e [produtos](/help/user-guide/guidelines/products.md) são salvos como registros. Um registro pessoal define as características de um segmento de cliente específico, ou seja, seu público-alvo para o conteúdo gerado. Pode incluir detalhes demográficos e um histórico de interações com o cliente.

Os registros de produtos definem as principais especificações e atributos de produtos no contexto das diretrizes da sua marca. Os atributos podem incluir recursos, imagens associadas e posicionamento do produto na sua marca.

As opções nos menus suspensos _Personas_ e _Produtos_ são definidas no nível organizacional. Ao criar uma campanha, selecione um desses registros predefinidos para garantir uma representação de produto consistente e suporte a direcionamento, mensagens e rastreamento de desempenho precisos.

**Para atribuir personalidades à sua campanha**:

1. Clique no sinal + (**[!UICONTROL Conectar registros +]**) ao lado de **[!UICONTROL Personas]**.

   O pop-up _Selecionar personas_ é aberto. Você pode pesquisar por um perfil suportado específico.

1. Selecione os perfis que sua campanha está direcionando. Personas válidas são definidas por sua organização durante a [criação de diretrizes](/help/user-guide/guidelines/personas.md).

   Opcionalmente, escolha **[!UICONTROL Ver tudo]** para abrir uma exibição de todos os perfis disponíveis.

**Para atribuir produtos à sua campanha**:

1. Clique no sinal + (**[!UICONTROL Conectar registros +]**) ao lado de **[!UICONTROL Produtos]**.

   O pop-up _Selecionar produtos_ é aberto. Você pode procurar por um produto suportado específico.

1. Selecione um ou mais produtos. Os produtos são definidos pela sua organização durante a [criação das diretrizes](/help/user-guide/guidelines/products.md).

   Opcionalmente, escolha **[!UICONTROL Ver tudo]** para abrir uma exibição de todos os produtos disponíveis.

## Concluir criação da campanha

Clique em **[!UICONTROL Criar]** para salvar os valores inseridos e criar a campanha.

O novo nome de campanha agora está disponível como um rótulo de campanha em [!DNL Content] e [!DNL Create]. Você pode adicionar ativos e experiências aprovados à sua campanha por meio do [!DNL Content] ou atribuir um ativo e uma experiência a uma campanha durante a criação do conteúdo.

## Adicionar conteúdo à campanha

O GenStudio for Performance Marketing vincula o conteúdo às campanhas usando rótulos de campanha armazenados nos metadados [!DNL Content]. Um único conteúdo pode ser associado a várias campanhas.

Os rótulos de campanha identificam a campanha e seus atributos. Atribuir um rótulo a um ativo ou experiência o conecta à campanha correspondente.

**Para adicionar ativos e experiências do[!DNL Content]**:

1. Na galeria [!DNL Content] _Experiências_ ou _Assets_, escolha a experiência ou o ativo aprovado.

1. Na exibição _Detalhes_, selecione o nome da campanha no menu suspenso _Campanhas_.

**Para adicionar ativos e experiências durante a criação de conteúdo**:

Durante a criação do conteúdo, você pode publicar o ativo ou a experiência recém-criada no [!DNL Content].

1. Na janela pop-up _Confirmar detalhes do conteúdo aprovado_, selecione uma campanha no menu suspenso _Campanhas_.

1. Clique em **[!UICONTROL Publicar]**.

Esta campanha agora está disponível no painel _Campanhas_.
