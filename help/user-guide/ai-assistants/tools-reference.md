---
title: Referência das ferramentas do assistente do AI
description: Saiba mais sobre as ferramentas de Insights, Criação, Planejamento, Ativação e comentários que um assistente de IA pode usar com o [!DNL GenStudio for Performance Marketing].
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# Referência das ferramentas do assistente de IA

Esta referência descreve as ferramentas que um assistente de IA conectado pode usar com [!DNL GenStudio for Performance Marketing]. A lista de ferramentas disponível depende da configuração de sua organização.

Pergunte ao assistente de IA quais ferramentas ele pode acessar antes de iniciar um fluxo de trabalho.

## Áreas de capacidade

| Área | Propósito | Comportamento |
|---|---|---|
| Insights | Consulte o desempenho de mídia paga e de email e recupere recomendações criativas. | Somente leitura. |
| Criar | Localize ativos, monte rascunhos de modelos do Express ou recomendações do Insights e gerencie a revisão. | Ler e gravar. Cria documentos no Creative Cloud. |
| Plano | Extraia os detalhes da campanha de um resumo e salve-os no Workfront Planning. | A extração é somente leitura. Salvar cria registros no Workfront Planning e não pode ser revertido automaticamente. |
| Ativar | Resolva um público alvo de publicação e envie uma experiência aprovada para a plataforma. | Gravar. Os anúncios são enviados para a plataforma e publicados em estado desativado. Você as ativa separadamente. Não é reversível com essas ferramentas. |
| Feedback | Envie comentários sobre o produto para a equipe do [!DNL GenStudio for Performance Marketing]. | Gravar. |

A maioria das ferramentas do Insights abrange `meta`, `linkedin` e `innovid`. As ferramentas de valor de métrica abrangem `meta` e `linkedin`. Os relatórios de campanha de email abrangem Adobe Journey Optimizer (`ajo`) e Adobe Campaign (`acc`).

A criação dá suporte a `meta`, `linkedin`, `display`, `tiktok` e `youtube`. A ativação oferece suporte a `META`, `LINKEDIN` e `GOOGLECM360`.

## Ferramentas do Insights

### get_insights_capabilities

Retorna os canais de Insights e as operações de relatórios habilitadas para sua organização. Use essa ferramenta primeiro quando a disponibilidade não estiver clara. Os canais com suporte são `meta`, `linkedin`, `innovid`, `ajo` e `acc`.

Essa ferramenta retorna os metadados do recurso, não os valores de campanha, anúncio ou métrica. Para encontrar as chaves de métrica personalizadas de sua organização, use `list_connected_channels_and_metrics`.

### list_connected_channels_and_metrics

Retorna as conexões ativas do Meta, LinkedIn e Google Campaign Manager 360 da sua organização, os canais e operações do Insights compatíveis e as métricas de conversão personalizadas configuradas. Use-o para localizar chaves de métrica antes de chamar `get_insights_metric_values`.

Essa ferramenta retorna chaves de métrica, rótulos e formatos, não valores de métrica. Uma conexão não garante que os dados históricos de relatórios estejam disponíveis.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. Omita ambos para retornar o catálogo completo. |

### get_insights_summary

Retorna as métricas e tendências de desempenho do título de um canal em um intervalo de datas selecionado.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `startDate` | Não | Data inicial no formato `YYYY-MM-DD`. O padrão é 30 dias atrás. |
| `endDate` | Não | Data final no formato `YYYY-MM-DD`. O padrão é hoje. |
| `metrics` | Não | Métricas para o gráfico: `spend`, `ctr`, `cpc`, `cpm`, `cpa`, `impressions`, `clicks`, `conversions`, `videoPlays`, `engagement`, `likes`, `comments` ou `shares`. O padrão é `spend`, `ctr`, `cpc` e `cpm`. |

### list_insights_campaigns

Retorna uma tabela classificável de métricas de desempenho de campanha e uma linha de totais.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. O padrão são os últimos 30 dias. |
| `search` | Não | Filtro de nome de campanha. |
| `sortBy` | Não | Campo de classificação: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` ou `name`. O padrão é `spend`. Os resultados são sempre classificados em ordem decrescente. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. O tamanho de página padrão é 20. |

### list_insights_email_campaigns

Retorna uma tabela classificável de campanhas de email com métricas de entrega e envolvimento para Adobe Journey Optimizer e Adobe Campaign. Para campanhas publicitárias, use `list_insights_campaigns`.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `ajo` ou `acc`. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. O padrão são os últimos 30 dias antes da data final. |
| `search` | Não | Filtro de nome de campanha. |
| `sortBy` | Não | Campo de classificação: `campaignName`, `emailsNumber`, `emailsDelivered`, `totalClicks`, `openRate`, `ctr`, `ctor`, `bounceRate`, `unsubscribeRate` ou `spamComplaintRate`. O padrão é `emailsDelivered`. Os resultados são sempre classificados em ordem decrescente. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

### list_insights_ads

Retorna o desempenho no nível do anúncio. Use o modo de navegação padrão para uma tabela classificável ou um modo de camada para anúncios de alto e baixo desempenho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `meta`, `linkedin` ou `innovid`. |
| `tier` | Não | `all`, `high` ou `low`. O padrão é `all`. |
| `mainMetric` | Não | Métrica de classificação para `high` ou modo de camada `low`: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` ou `clicks`. Ignorado no modo de navegação. |
| `metrics` | Não | Métricas adicionais para relatar cada anúncio no modo de camada. |
| `campaigns` | Não | Campanhas usadas para limitar o resultado, até 50. Cada campanha inclui `channel`, `accountId` e `campaignId`. |
| `search` | Não | Filtro de nome de anúncio. |
| `sortBy` | Não | Campo de classificação do modo de navegação: `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` ou `name`. O padrão é `spend`. Os resultados são sempre classificados em ordem decrescente. |
| `spendMin`, `spendMax` | Não | Limites de gasto total para cada anúncio. Somente modo de camada. |
| `includeUnsupported` | Não | Inclui anúncios cujo criativo não pode ser renderizado. O padrão é `false`. |
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
| `ads` | Sim | Um a 200 anúncios para explicar. Cada anúncio inclui `channel`, `accountId`, `campaignId` e `adId` e, opcionalmente, `adGroupId` e `performanceTier` (`high` ou `low`). Use os identificadores retornados por `list_insights_ads` no modo de camada. |
| `mainMetric` | Sim | A métrica usada para classificar os anúncios: `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` ou `clicks`. |
| `campaigns` | Não | Campanhas usadas para definir a população de comparação, até 50. Cada campanha inclui `channel`, `accountId` e `campaignId`. |
| `spendMin`, `spendMax` | Não | Limites de gasto para a população de comparação. |
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
| `tagSource` | Não | `ad_tags` ou `campaign_tags`. O padrão é `ad_tags`. |
| `sortBy` | Não | Campo de classificação: `adsCount`, `spend`, `impressions`, `clicks`, `conversionCount`, `ctr`, `cpc`, `cpm` ou `cpa`. O padrão é `adsCount`. |
| `search` | Não | Filtro do valor de tag. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

### get_insights_metric_values

Retorna os valores e as tendências das métricas rastreadas de sua organização, como prospetos, inscrições ou retorno do investimento em anúncios, para Meta e LinkedIn.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channels` | Não | `meta`, `linkedin` ou ambos. |
| `metrics` | Não | Até 20 chaves de métrica retornadas por `list_connected_channels_and_metrics`. O padrão é o conjunto visível padrão de sua organização. |
| `campaigns` | Não | Campanhas usadas para limitar o resultado, até 50. Cada campanha inclui `channel`, `accountId` e `campaignId`. |
| `startDate`, `endDate` | Não | Intervalo de datas no formato `YYYY-MM-DD`. O padrão são os últimos 30 dias. |

### get_insights_recommendations

Retorna as alterações criativas propostas com base nos dados de desempenho de sua organização. Uma solicitação não pode retornar nenhuma recomendação quando o escopo selecionado não contém anúncios elegíveis.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channels` | Sim | Um ou mais de `meta`, `linkedin` ou `innovid`. |
| `campaigns` | Não | Campanhas usadas para limitar o resultado, até 50. Cada campanha inclui `channel`, `accountId` e `campaignId`. |
| `search` | Não | Filtro de nome de campanha. |
| `recommendationId` | Não | O `adUid` de uma recomendação, usado para recuperá-la em detalhes. |
| `onlyWithPreview` | Não | Exclui recomendações que não têm um exemplo de visualização criativa. O padrão é `true`. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

## Criar ferramentas

Crie ferramentas, localize ativos, monte rascunhos de modelos do Adobe Express e gerencie a revisão antes que uma experiência esteja pronta para ativação.

### list_express_templates

Lista os modelos do Express disponíveis com filtragem e contagem de facetas.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Não | `meta`, `display`, `linkedin`, `tiktok`, `youtube` ou `__unspecified__`. |
| `query` | Não | Termo de pesquisa para modelos. |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | Não | Filtros de facetas de modelo. |
| `sortBy` | Não | `modified` ou `created`. O padrão é `modified`. |
| `order` | Não | `asc` ou `desc`. O padrão é `desc`. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

### describe_express_template

Retorna os campos de texto editáveis e as disposições de imagem em um modelo.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `templateId` | Sim | Identificador de modelo expresso. |

### list_cta_options

Retorna os valores de call-to-action permitidos para um canal. Display retorna uma lista vazia porque aceita texto de forma livre.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `linkedin`, `meta`, `display`, `tiktok` ou `youtube`. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. Omitir ambos para retornar todas as opções. |

### search_assets

Pesquisa imagens e vídeos no seu conteúdo do GenStudio. Use-a para selecionar ativos existentes para um rascunho. Os ativos derivados, externos e expirados são excluídos. Essa ferramenta não faz upload, edita, exclui ou gera ativos e requer o direito ao Conteúdo do GenStudio.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `query` | Não | Pesquisa por palavra-chave ou idioma natural nos metadados do ativo. |
| `mediaTypes` | Não | `image`, `video` ou ambos. O padrão inclui ambos. |
| `aspectRatios` | Não | Taxas de proporção como `1:1` ou `16:9`. Se uma proporção não estiver disponível, a ferramenta retornará as opções disponíveis. |
| `brands`, `campaigns`, `products`, `personas`, `channels` | Não | Filtra por nome. |
| `customMetadata` | Não | Até 5 campos de metadados, cada um com um ou mais valores. |
| `uploadedBy` | Não | `me` ou um endereço de email do carregador. |
| `createdAtFrom`, `createdAtTo` | Não | Limites de tempo de criação no formato ISO 8601. |
| `aiGenerated` | Não | Filtros por status de geração de IA. |
| `contentCredentials` | Não | Filtros por status do Content Credentials. |
| `limit`, `offset` | Não | Tamanho da página e deslocamento de página. |

O resultado inclui referências de ativos estáveis para `create_draft` e URLs assinadas de curta duração.

### create_draft

Cria um rascunho editável de um modelo Expresso com uma ou mais experiências. Cada chamada cria um novo rascunho.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `templateId` | Sim | Identificador de modelo expresso. |
| `prompt` | Sim | As instruções resumidas e de cópia do Creative são armazenadas com o rascunho. |
| `experiences` | Sim | Uma ou mais experiências. Consulte a tabela a seguir. |
| `name` | Não | Nome do documento. |
| `allowAssetReuse` | Não | Permite que um ativo selecionado seja reutilizado em várias experiências. O padrão é `false`. |

Cada experiência aceita estes campos:

| Campo | Obrigatório | Descrição |
|---|---|---|
| `channel` | Sim | `linkedin`, `meta`, `display`, `tiktok` ou `youtube`. |
| `title` | Não | Título da experiência. O padrão é &quot;Conceito *n*&quot;. |
| `headline` | Meta e LinkedIn | Título principal. |
| `body` | Meta, LinkedIn e TikTok | Cópia do corpo. Para o LinkedIn, este é o texto introdutório. Para o TikTok, esse é o texto principal. |
| `description` | YouTube | Descrição do anúncio. Opcional para Meta e LinkedIn. |
| `display_url` | Meta e LinkedIn | URL de exibição mostrado no anúncio. |
| `destination_url` | Não | URL ao qual o anúncio está vinculado. |
| `cta` | Não | Texto call-to-action de `list_cta_options`. |
| `templateFields` | Não | Substituições para elementos de modelo nomeados de `describe_express_template`. Cada substituição define texto, um URL de imagem com dimensões ou um URL de vídeo. |
| `assetTemplateFields` | Não | Ativos de conteúdo de `search_assets` para campos de imagem ou vídeo no modelo. |

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
| `emails` | Sim | De um a 20 endereços de email de colaborador. |
| `role` | Sim | `editor` ou `viewer`. |
| `message` | Não | Mensagem de convite. |

### request_draft_approval

Envia um rascunho a uma ou mais pessoas para aprovação.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `draftId` | Sim | Identificador de ativo de rascunho. |
| `emails` | Sim | De um a 20 endereços de email de revisores. |

### list_experience

Retorna experiências aprovadas e publicadas que estão prontas para ativação. Os rascunhos não estão incluídos.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `channel` | Não | `email`, `meta`, `meta_organic`, `display`, `ctv`, `linkedin`, `linkedin_organic`, `tiktok`, `chatgpt` ou `youtube`. |
| `createdByMe` | Não | Limita os resultados às experiências criadas pelo usuário atual. |
| `campaignNames` | Não | Até 5 filtros exatos de nome de campanha. |
| `creatorEmail` | Não | Filtro de email do criador. |
| `createdAtFrom`, `createdAtTo` | Não | Limites da data de criação. |
| `language` | Não | Marca de idioma BCP 47. |
| `limit`, `cursor` | Não | Tamanho da página (1-50, padrão 20) e cursor de paginação. |

## Ferramentas de planejamento

As ferramentas de plano transformam um resumo da campanha em um rascunho de campanha revisável e o salvam no Workfront Planning.

### extract_campaign_from_brief

Extrai um rascunho de campanha revisável de um resumo de marketing colado. Esta ferramenta não salva nenhum registro. Fatos e datas ausentes não são inferidos.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `briefText` | Sim | O texto completo de um resumo da campanha, até 100.000 caracteres. Arquivos e links não são compatíveis. |

O resultado inclui um rascunho da campanha, resultados com aspas de apoio, públicos sugeridos e avisos.

### create_workfront_campaign

Cria uma campanha do Workfront Planning com produtos e perfis vinculados a partir de um rascunho que você revisou e aprovou. Essa ferramenta não é idempotente e os registros não podem ser revertidos automaticamente. Inspecione o Workfront antes de tentar novamente uma gravação que pode ter sido bem-sucedida.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `campaignDraft` | Sim | O rascunho aprovado. Requer `name`. Os campos opcionais são `description`, `objective`, `keyMessaging`, `startDate`, `endDate` (`YYYY-MM-DD`), `status`, `channels`, `products` e `personas`. |
| `channelSelections` | Não | Opções aprovadas para nomes de canal ambíguos. |
| `entitySelections` | Não | Registros de produto e persona existentes aprovados. Use `null` para solicitar um novo registro. |
| `createMissingEntities` | Não | Cria os produtos e personalidades selecionados como novos. O padrão é `false`. |

Se um produto, perfil ou canal for ambíguo, a ferramenta retornará opções para confirmar e não fará alterações.

## Ativar ferramentas

Ative as ferramentas para resolver um público-alvo de mídia paga e enviar uma experiência aprovada para a plataforma. Os anúncios são publicados no estado desativado (Meta pausado, LinkedIn rascunho, Campaign Manager 360 inativo), portanto, você deve ativá-los separadamente antes de serem entregues. O envio de anúncios para a plataforma não é reversível por meio dessas ferramentas.

### configure_ativation_target

Resolve e valida a conta de mídia paga, a campanha, o conjunto de anúncios e a página do Facebook, quando necessário.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `platform` | Sim | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `platformAccountId` | Não | Identificador de conta de mídia paga. Omita-o para descobrir contas. |
| `campaignId` | Não | Identificador de campanha para Meta ou LinkedIn. Não usado para o Campaign Manager 360. |
| `adsetId` | Não | Conjunto de anúncios do Meta ou identificador de campanha do LinkedIn. Não usado para o Campaign Manager 360. |
| `pageId` | Não | Identificador de página do Facebook para Meta. |

Para o Campaign Manager 360, somente a conta de anúncio é necessária.

### create_ativation

Envia uma experiência aprovada para a plataforma como anúncios, usando um público alvo validado. Os anúncios são publicados em estado desativado. O Meta cria um anúncio com a primeira imagem para cada taxa de proporção. O LinkedIn e o Campaign Manager 360 criam um anúncio para cada imagem resolvida.

| Parâmetro | Obrigatório | Descrição |
|---|---|---|
| `platform` | Sim | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `targetId` | Sim | Destino validado retornado por `configure_activation_target`. |
| `experienceId` | Sim | Identificador de experiência aprovado retornado por `list_experiences`. |
| `name` | Não | Nome de exibição do posicionamento do anúncio. O padrão é o título do anúncio da experiência. |

O resultado lista o número de anúncios criados, enfileirados e ignorados com o status inicial de cada anúncio e um link para ele em [!DNL GenStudio for Performance Marketing]. Um status de `PENDING` significa que o trabalho está na fila, não que o anúncio está sendo entregue.

Chamar `create_activation` duas vezes cria anúncios adicionais em vez de atualizar os primeiros anúncios.

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
- **Revisar métricas rastreadas:** Chame `list_connected_channels_and_metrics`, em seguida, chame `get_insights_metric_values` com chaves de métrica retornadas.
- **Transformar uma recomendação em um rascunho:** Chamar `get_insights_recommendations`, depois chamar `create_draft_from_recommendation`.
- **Compilação a partir de um modelo:** Chame `list_express_templates`, `describe_express_template` e `list_cta_options`, depois chame `create_draft`.
- **Compilação a partir de ativos existentes:** Chame `search_assets` e passe as referências de ativos retornados para `create_draft` em `assetTemplateFields`.
- **Salve um resumo da campanha no Workfront:** Ligue para `extract_campaign_from_brief`, revise o rascunho e ligue para `create_workfront_campaign`.
- **Enviar uma experiência aprovada para uma plataforma:** Chamar `list_experiences`, depois chamar `configure_activation_target` e `create_activation`.

## Recursos relacionados

- [Visão geral dos assistentes de IA](overview.md)
- [Conectar um assistente de IA](connect-ai-assistants.md)
- [Usar assistentes de IA](use-ai-assistants.md)
