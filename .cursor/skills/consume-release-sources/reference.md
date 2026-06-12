---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# Referência: fontes de liberação de consumo (MCP)

## Descoberta de página de cerimônia

| Padrão | Exemplo |
|---------|---------|
| Título | `YYYY/MM Release Ceremony` no espaço **GenStudio** |
| De Jira | Link wiki no tíquete `description` (preferencial) |
| Fallback CQL | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## Grupos de recursos de cerimônia

Os wikis de cerimônia de lançamento contêm até **dois** tabelas de recursos. Analise ambos a partir do **armazenamento** HTML.

### Recursos da versão do GA

- Título da seção: `GA Release Features` (`<h2>`)
- Subtítulo: `Feature Group:` com link opcional do Floodgate
- As colunas da tabela incluem **Tipo** (`GA`, `Limited`, `EA`, `Beta` ou vazias)
- **Coluna Documentação do KT**: `<ac:link><ri:page ri:content-title="..."/></ac:link>`

Extração por linha:

| Campo | Origem |
|-------|--------|
| `featureDescription` | Primeiro `<td>` na linha de dados |
| `type` | Digitar texto da célula da coluna |
| `ktPageTitle` | `ri:content-title` na coluna do KT |
| `jiraKeys` | `ac:macro ac:name="jira"` → `key` parâmetro (somente interno) |
| `releaseTier` | `ga` quando o Tipo for `GA`; herdar Tipo para outros valores da tabela de GA |

### Recursos da versão do Beta

- Título da seção: `Beta Release Features` (pode estar **ausente** em alguns meses)
- Segunda tabela; **nenhuma coluna Type** — cada linha é Beta
- Mesma extração de KT e Jira que a tabela de GA
- Definir `releaseTier: beta` e `requiresBetaBadge: true` em cada linha de seção Beta

Se a seção Beta estiver ausente, registre zero linhas de Beta e continue.

### Padrões de HTML de armazenamento

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## Uso da ferramenta MCP

| Etapa | Ferramenta | Parâmetros |
|------|------|------------|
| Tíquete | `jira_getIssue` | `issueKey`, `expand: renderedFields` opcional |
| Cerimônia | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| Pesquisa de KT | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| Corpo de KT | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**Não** use `bodyMode: text` para páginas de cerimônia ao analisar links de KT.

## Mapeamento de campo do KT (entradas de elaboração)

Mapear em generate-release-notes; não cole nas notas de versão públicas textualmente.

| Seção do KT | Usar |
|------------|-----|
| Descrição | Recurso principal |
| Arremesso do elevador | Proposta de valor |
| Recursos entregues | Comportamento concreto |
| Declaração do problema | Dor do usuário (somente contexto) |
| Tipo e data de lançamento | GA / Beta / Limitado (interno); selo de unidades decisão |

## Filtros de inclusão

Confirme o escopo com o usuário quando não estiver claro. Predefinições comuns:

| Predefinição | Inclui |
|--------|----------|
| `ga_only` | Linhas da tabela GA onde Tipo = `GA` |
| `ga_and_beta` | **Padrão recomendado para os próximos meses** — Linhas do GA onde Tipo = `GA` **mais todas** linhas da tabela Recursos da Versão do Beta |
| `ga_plus_empty` | Tabela GA: Tipo = `GA` ou Tipo vazio |
| `all_except_pilot` | Linhas da tabela GA exceto `Limited`; mais a seção Beta ao usar `ga_and_beta` |
| `all_with_badges` | Todas as linhas da tabela GA; as linhas da seção Beta sempre recebem o selo Beta |

## Entrega do selo do Beta

| Condição | `requiresBetaBadge` |
|-----------|---------------------|
| Linha da tabela **Recursos da versão do Beta** | `true` |
| Linha de tabela GA com Tipo = `Beta` | `true` |
| Linha de tabela GA com Tipo = `GA` | `false` |

Downstream: [gerar-notas-de-versão Regras de decisão](../generate-release-notes/SKILL.md#decision-rules) e [trecho do selo da Beta](../generate-release-notes/SKILL.md#beta-badge).

## Carga de transferência (informal)

Passe para generate-release-notes como uma lista de itens:

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
