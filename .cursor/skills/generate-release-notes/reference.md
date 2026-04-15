---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# Referência: criação das notas de versão

## Frontmatter

A página ao vivo [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md) inclui metadados Experience League além de um conjunto mínimo (por exemplo, `TQID`, `product_v2`, `feature_v2`, IDs de taxonomia).

**Regras:**

- Ao editar o conteúdo da nota de versão **body**, **preserve as chaves e os valores de frontmatter** existentes, a menos que a tarefa solicite explicitamente a alteração dos metadados.
- Não remova a taxonomia ou os metadados do produto para corresponder a um modelo mais curto.
- Os conceitos necessários para as páginas ExL geralmente incluem `title`, `description` e `role`; siga as [orientações de metadados do Experience League](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata) para as novas páginas.

## Fontes internas (KT e wikis de versão)

Use estes campos **somente durante o rascunho**; as notas de versão publicadas não devem fazer referência a documentos internos.

### Documentos de transferência de conhecimento (KT)

Extrair de:

| Campo | Usar |
|-------|-----|
| Descrição | Explicação do recurso principal |
| Argumento do elevador | Proposta de valor |
| Recurso(s) entregue(s) | Comportamento concreto |
| Declaração do problema | Ponto problemático do usuário |
| Tipo e data de lançamento | Intervalo |

### Lançar páginas wiki

Agrupar e analisar por:

| Campo | Usar |
|-------|-----|
| Data de lançamento (versão fixa) | Mesma data → mesmo lote de notas de versão |
| Iniciativa | Somente contexto; não vincular internamente em texto público |
| O PM apresenta o recurso usando o KT | Sinaliza detalhes mais profundos do KT |

**Regra de escopo:** itens que compartilham a mesma Data de Lançamento (Versão Fixa) pertencem ao mesmo bloco de lançamento mensal.

## Vinculação de documentação

- Link para a frase **mais relevante** (por exemplo, link de &quot;ativos de imagem e vídeo não suportados&quot; para a seção de formatos de anúncio).
- Preferir links `#anchor` para a subseção direita.
- As páginas de visão geral são aceitáveis quando não existe uma âncora mais profunda.

## Caminhos comuns da documentação

| Área | Prefixo de caminho |
|------|-------------|
| Criar | `/help/user-guide/create/` |
| Conteúdo | `/help/user-guide/content/` |
| Ativação | `/help/user-guide/activation/` |
| Aprovações | `/help/user-guide/approvals/` |
| Insights | `/help/user-guide/insights/` |
| Diretrizes | `/help/user-guide/guidelines/` |
| Modelos | `/help/user-guide/templates/` |
| Campanhas | `/help/user-guide/campaigns/` |
| Extensibilidade | `/help/extensibility/` |
