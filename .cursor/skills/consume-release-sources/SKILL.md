---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Fontes de liberação do consumidor (Jira + Confluence MCP)

**Rascunho downstream:** [generate-release-notes](../generate-release-notes/SKILL.md) → [polish-release-notes](../polish-release-notes/SKILL.md) opcional

**Referência de análise:** [reference.md](reference.md)

**Arquivo de saída de destino (apenas downstream):** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## Pré-requisitos

- **Jira MCP** (`jira_getIssue`, `jira_searchIssues`) autenticado
- **MCP de Confluência** (`confluence_getContent`, `confluence_searchContent`) autenticado
- Chave do tíquete Jira do nome da filial (`GS-#####`), entrada do usuário ou descrição do tíquete

## Lista de verificação do fluxo de trabalho

1. [ ] **Resolver tíquete Jira** — `jira_getIssue` com `issueKey`. Leia `description` para o link da wiki da cerimônia e o mês de lançamento.
2. [ ] **Localizar página de cerimônia** — usar URL wiki do tíquete; CQL de fallback: `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`.
3. [ ] **Buscar corpo de cerimônia** — `confluence_getContent` com `bodyMode: storage` (obrigatório; `text` perde links de KT e estrutura de tabela).
4. [ ] **Analisar grupos de recursos** — extrair linhas dos **Recursos da Versão do GA** e dos **Recursos da Versão do Beta** (consulte [reference.md](reference.md#ceremony-feature-groups)).
5. [ ] **Aplicar filtro de inclusão** — por escopo de usuário (consulte [reference.md](reference.md#inclusion-filters)); confirmar contagem de linhas do Beta (pode ser zero).
6. [ ] **Resolver páginas do KT** — `confluence_searchContent` por título do KT; `confluence_getContent` com `bodyMode: text`.
7. [ ] **Extrair campos KT** — Descrição, Densidade do elevador, Recursos fornecidos, Declaração do problema, Tipo de lançamento e Data.
8. [ ] **Definir sinalizadores Beta** — `requiresBetaBadge: true` para linhas de seção Beta ou linhas de tabela GA com Tipo `Beta`.
9. [ ] **Entrega** a [gerar-notas-versão](../generate-release-notes/SKILL.md) com lista de linhas estruturadas (sem referências wiki/Jira na cópia remetida).

## Rotulação do Beta (entrega para gerar habilidades)

Quando `requiresBetaBadge: true`, a seção downstream `###` deve incluir imediatamente sob o título:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

Não adicione itálico de isenção de responsabilidade de agendamento para o Beta; o símbolo é o padrão compatível.

## Proibido nas notas de versão enviadas

IDs internas, URLs wiki, citações de KT e chaves Jira permanecem somente nesta fase de assimilação. Resumir os resultados voltados para o usuário na página pública por [conteúdo proibido de generate-release-notes](../generate-release-notes/SKILL.md#prohibited-content).

## Fallback

Se as chamadas de MCP falharem, peça ao usuário para colar o conteúdo de cerimônia e KT, em seguida, continue com generate-release-notes usando o [mapeamento de campo de KT reference.md](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis).

## Recursos adicionais

- [reference.md](reference.md) — análise de cerimônia, CQL, filtros de inclusão, parâmetros MCP
- [generate-release-notes](../generate-release-notes/SKILL.md) — arquivo, rascunho, links, verificações de qualidade
- [notas de versão da polonesa](../polish-release-notes/SKILL.md) — passagem editorial no novo `###` em `{#latest}`
