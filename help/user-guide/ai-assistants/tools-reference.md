---
title: Referência das ferramentas do assistente do AI
description: Saiba mais sobre as ferramentas de Insights, Criação, Ativação e comentários que um assistente de IA pode usar com o [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# Referência das ferramentas do assistente de IA

Esta referência descreve as ferramentas que um assistente de IA conectado pode usar com [!DNL GenStudio for Performance Marketing]. A lista de ferramentas disponível depende da configuração de sua organização.

Pergunte ao assistente de IA quais ferramentas ele pode acessar antes de iniciar um fluxo de trabalho.

## Áreas de capacidade

| Área | Propósito | Comportamento |
|---|---|---|
| Insights | Consulte o desempenho de mídia paga e recupere recomendações criativas. | Somente leitura. |
| Criar | Reunir rascunhos de modelos do Express ou recomendações do Insights e gerenciar a revisão. | Ler e gravar. Cria documentos no Creative Cloud. |
| Ativar | Resolva um público alvo de publicação e publique uma experiência aprovada. | Escrita e destrutiva. Podem publicar um anúncio ao vivo e gerar gastos com anúncios. |
| Feedback | Envie comentários sobre o produto para a equipe do [!DNL GenStudio for Performance Marketing]. | Gravar. |

A maioria das ferramentas do Insights abrange `meta`, `linkedin` e `innovid`. As ferramentas de métrica de conversão abrangem `meta` e `linkedin`.

A criação dá suporte a `meta`, `linkedin`, `display`, `tiktok` e `youtube`. A ativação oferece suporte a `META`, `LINKEDIN` e `GOOGLECM360`.

## Ferramentas do Insights

### get_insights_capabilities

Retorna os canais de Insights, as operações e as métricas de conversão personalizadas habilitadas para sua organização. Use essa ferramenta primeiro quando a disponibilidade não estiver clara.

Essa ferramenta retorna os metadados do recurso, não os valores de campanha, anúncio ou métrica.

### get_insights_summary

Retorna as métricas e tendências de desempenho do título de um canal em um intervalo de datas selecionado.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `startDate` | Não | Data inicial no formato `YYYY-MM-DD`. O padrão é 30 dias atrás. |
| `endDate` | Não | Data final no formato `YYYY-MM-DD`. O padrão é hoje. |
| `metrics` | Não | Métricas para o gráfico, como `spend`, `ctr`, `cpc`, `cpm`, `impressions`, `clicks` ou `conversions`. |

### list_insights_campaigns

Retorna uma tabela classificável de métricas de desempenho de campanha e uma linha de totais.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. O padrão são os últimos 30 dias. |
| `search` | Não | Filtro de nome de campanha. |
| `sortBy` | Não | Campo de classificação, como `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` ou `name`. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

### list_insights_ads

Retorna o desempenho no nível do anúncio. Use o modo de navegação padrão para uma tabela classificável ou um modo de camada para anúncios de alto e baixo desempenho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `tier` | Não | `all`, `high` ou `low`. O padrão é `all`. |
| `mainMetric` | Condicional | Métrica de classificação necessária para o modo de camada `high` ou `low`. |
| `campaigns` | Não | Identificadores de campanha usados para limitar o resultado. |
| `search` | Não | Filtro de nome de anúncio. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

O modo de camada retorna os identificadores de anúncios necessários para `get_insights_ad_attributes`.

### get_insights_ad_details

Retorna metadados criativos de um anúncio, incluindo cópia, call to action, ativos e posicionamentos. Ela não retorna métricas de desempenho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `accountId` | Sim | Identificador de conta de mídia paga. |
| `campaignId` | Sim | Identificador da campanha. |
| `adId` | Sim | Identificador de anúncio. |
| `adgroupId` | Não | Identificador de grupo de anúncios quando o canal usa grupos de anúncios. |

### get_insights_ad_attributes

Compara as características criativas de anúncios selecionados com a média do canal. Use-o depois que `list_insights_ads` identificar anúncios de alto ou baixo desempenho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `ads` | Sim | Anúncios para explicar, incluindo os identificadores retornados por `list_insights_ads`. |
| `mainMetric` | Sim | A métrica usada para classificar os anúncios. |
| `campaigns` | Não | Identificadores de campanha usados para definir a população de comparação. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. |

### get_insights_tag_categories

Retorna as categorias de tags disponíveis para sua organização durante o período solicitado. Ele retorna nomes de categoria, não métricas de desempenho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channels` | Sim | Um ou mais canais compatíveis. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. |

### get_insights_ad_tags

Retorna o desempenho pelo valor da tag em uma categoria, como produto, região ou tema criativo.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `tagCategory` | Sim | Uma categoria retornada por `get_insights_tag_categories`. |
| `tagSource` | Não | `ad_tags` ou `campaign_tags`. |
| `sortBy` | Não | Métrica usada para classificar o resultado. |
| `search` | Não | Filtro do valor de tag. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. |

### get_insights_custom_metrics

Retorna as métricas de conversão personalizadas configuradas para sua organização. Use-o antes de `get_insights_conversion_metrics`.

Essa ferramenta retorna identificadores de métrica, não valores de métrica.

### get_insights_conversion_metrics

Retorna valores e tendências de métricas de conversão configurados para o Meta e o LinkedIn.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channels` | Não | Canal de conversão compatível. O padrão é `meta`. |
| `metrics` | Não | Identificadores de métrica retornados por `get_insights_custom_metrics`. |
| `campaigns` | Não | Identificadores de campanha usados para limitar o resultado. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. |

### get_insights_recommendations

Retorna as alterações criativas propostas com base nos dados de desempenho de sua organização. Uma solicitação não pode retornar nenhuma recomendação quando o escopo selecionado não contém anúncios elegíveis.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channels` | Sim | Um ou mais canais compatíveis. |
| `campaigns` | Não | Identificadores de campanha usados para limitar o resultado. |
| `search` | Não | Filtro de nome de campanha. |
| `recommendationId` | Não | Identificador usado para recuperar uma recomendação em detalhes. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

## Criar ferramentas

Crie ferramentas para reunir rascunhos de modelos do Adobe Express e gerenciar a revisão antes que uma experiência esteja pronta para ativação.

### list_express_templates

Lista os modelos do Express disponíveis com filtragem e contagem de facetas.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Não | `meta`, `display`, `linkedin`, `tiktok`, `youtube` ou `__unspecified__`. |
| `query` | Não | Termo de pesquisa para modelos. |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | Não | Filtros de facetas de modelo. |
| `sortBy`, `order` | Não | Classificar campo e ordem. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

### describe_express_template

Retorna os campos de texto editáveis e as disposições de imagem em um modelo.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `templateId` | Sim | Identificador de modelo expresso. |

### list_cta_options

Retorna os valores de call-to-action permitidos para um canal.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `linkedin`, `meta`, `display`, `tiktok` ou `youtube`. |

### create_draft

Cria um rascunho editável de um modelo Expresso com uma ou mais experiências.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `templateId` | Sim | Identificador de modelo expresso. |
| `prompt` | Sim | As instruções resumidas e de cópia do Creative são armazenadas com o rascunho. |
| `experiences` | Sim | Sobreposições de canal, campos de conteúdo e campo de modelo opcional para cada experiência. |
| `name` | Não | Nome do documento. |

Use `list_cta_options` antes de criar um rascunho para um canal com valores fixos de call-to-action.

### create_draft_from_recommendation

Cria um rascunho editável a partir de uma recomendação específica do Insights.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta` ou `linkedin`. |
| `adUid` | Sim | Identificador de recomendação retornado por `get_insights_recommendations`. |
| `prompt` | Sim | Resumo do Creative com base na recomendação. |
| `name` | Não | Nome do documento. |

### list_recent_drafts

Lista os rascunhos recentes do modelo expresso com seus status e links.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

### get_draft_metadata

Retorna o nome, os canais, o status de aprovação, os resultados do revisor e o acesso do colaborador de um rascunho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `draftId` | Sim | Identificador de ativo de rascunho. |

### share_draft

Concede aos colaboradores acesso de visualização ou edição a um rascunho sem solicitar aprovação.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `draftId` | Sim | Identificador de ativo de rascunho. |
| `emails` | Sim | Um ou mais endereços de email de colaborador. |
| `role` | Sim | `editor` ou `viewer`. |
| `message` | Não | Mensagem de convite. |

### request_draft_approval

Envia um rascunho a uma ou mais pessoas para aprovação.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `draftId` | Sim | Identificador de ativo de rascunho. |
| `emails` | Sim | Um ou mais endereços de email de revisor. |

### list_experience

Retorna experiências aprovadas e publicadas que estão prontas para ativação. Os rascunhos não estão incluídos.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Não | Filtro de canal de experiência. |
| `createdByMe` | Não | Limita os resultados às experiências criadas pelo usuário atual. |
| `campaignNames` | Não | Filtros de nome de campanha exatos. |
| `creatorEmail` | Não | Filtro de email do criador. |
| `createdAtFrom`, `createdAtTo` | Não | Limites da data de criação. |
| `language` | Não | Marca de idioma BCP 47. |
| `limit`, `cursor` | Não | Tamanho da página e cursor de paginação. |

## Ativar ferramentas

Ative ferramentas para resolver um público-alvo de mídia paga e publicar uma experiência aprovada. A publicação não é reversível por meio dessas ferramentas e pode gerar gastos com anúncios.

### configure_ativation_target

Resolve e valida a conta de mídia paga, a campanha, o conjunto de anúncios e a página do Facebook, quando necessário.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `platform` | Sim | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `platformAccountId` | Não | Identificador de conta de mídia paga. Omita-o para descobrir contas. |
| `campaignId` | Não | Identificador de campanha para Meta ou LinkedIn. |
| `adsetId` | Não | Conjunto de anúncios do Meta ou identificador de campanha do LinkedIn. |
| `pageId` | Não | Identificador de página do Facebook para Meta. |

### create_ativation

Publica um anúncio de imagem única ao vivo de uma experiência aprovada e de um público-alvo validado.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `platform` | Sim | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `targetId` | Sim | Destino validado retornado por `configure_activation_target`. |
| `experienceId` | Sim | Identificador de experiência aprovado retornado por `list_experiences`. |
| `assetId` | Não | Identificador de variante para uma experiência com várias variantes elegíveis. |
| `name` | Não | Nome de exibição do posicionamento do anúncio. |

Chamar `create_activation` duas vezes cria dois anúncios separados em vez de atualizar o primeiro anúncio.

## Ferramenta de feedback

### submit_mcp_feedback

Envia comentários sobre uma ferramenta ou fluxo de trabalho para a equipe [!DNL GenStudio for Performance Marketing].

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `category` | Sim | `bug`, `feature_request` ou `workflow_friction`. |
| `comment` | Sim | Uma descrição concisa do feedback. |
| `tags` | Não | Tags usadas para categorizar o feedback. |
| `tool_name` | Não | A ferramenta associada ao feedback. |

## Fluxos de trabalho comuns

Use essas sequências quando uma ferramenta fornecer identificadores ou configuração para outra:

- **Diagnostique um anúncio:** Chame `list_insights_ads` no modo de camada `high` ou `low` e chame `get_insights_ad_attributes` com a mesma métrica de classificação.
- **Analisar por marca:** Chame `get_insights_tag_categories` e, em seguida, chame `get_insights_ad_tags` com uma categoria retornada.
- **Revisar métricas de conversão:** Chame `get_insights_custom_metrics`, em seguida, chame `get_insights_conversion_metrics` com identificadores de métrica retornados.
- **Transformar uma recomendação em um rascunho:** Chamar `get_insights_recommendations`, depois chamar `create_draft_from_recommendation`.
- **Compilação a partir de um modelo:** Chame `list_express_templates`, `describe_express_template` e `list_cta_options`, depois chame `create_draft`.
- **Publique uma experiência aprovada:** Ligue para `list_experiences`, depois ligue para `configure_activation_target` e `create_activation`.

## Recursos relacionados

- [Visão geral dos assistentes de IA](overview.md)
- [Conectar um assistente de IA](connect-ai-assistants.md)
- [Usar assistentes de IA](use-ai-assistants.md)
