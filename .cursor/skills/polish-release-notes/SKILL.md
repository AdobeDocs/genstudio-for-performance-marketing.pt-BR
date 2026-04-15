---
name: polish-release-notes
description: ""
notes: refines only newly added
source-git-commit: 1a33b08048233c5f9a82b5f428082aa5c71b0052
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---


# Notas de versão do GenStudio em polonês

**Arquivo de destino canônico:** [help/user-guide/release-notes.md](../../../help/user-guide/release-notes.md)

**Exemplos:** [exemplos.md](examples.md)

**Fluxo de trabalho de rascunho (upstream):** [generate-release-notes](../generate-release-notes/SKILL.md)

## Escopo (obrigatório)

Polonês **somente** conteúdo que o usuário identifica como **recém-adicionado** nesta rodada:

- **No arquivo:** `###` subseções sob o único cabeçalho `## YYYY.MM {#latest}` em `help/user-guide/release-notes.md`.
- **Não** edite o título da página, o parágrafo de introdução, o assunto principal ou qualquer texto em **Notas de versão anteriores** (blocos `+++` recolhíveis).
- **Não** edite os `##` blocos mensais anteriores ou os `###` preexistentes na mesma seção `{#latest}`, a menos que o usuário **explicitamente** solicite.
- Se não estiver claro quais `###` são novos, **pergunte** ou use **git diff** / edite o contexto antes de alterar a prosa.
- **Conteúdo colado:** somente o markdown de polimento que o usuário cola quando confirma que ele corresponde às **mesmas** novas subseções (não trate colagens não relacionadas como dentro do escopo).

Manter diferenças **mínimas**: somente quebras de texto e parágrafo, sem refatoração de drive-by em outro lugar no arquivo.

## Voz e tom

- Escreva como um **redator** para notas de versão de produtos: **conciso**, **digitalizável** e **energizado** sobre o **novo valor**—forneça resultados e diga &quot;o que você ganha com isso&quot;, use verbos fortes e linguagem clara para seus benefícios.
- **Mantenha-se preciso:** nenhuma afirmação além do que o recurso oferece; combine o tom do Experience League/Adobe (confiante e claro, não sensacionalista).
- **Gere entusiasmo** com benefícios e deltas **específicos** (o que os profissionais de marketing podem fazer agora, qual fricção é removida), não hipes vazios ou superlativos não fundamentados.

## Regras de parágrafo

- Cada parágrafo: **2-3 frases**. **Nunca mais do que três frases** em um parágrafo. Se precisar de mais, inicie um **novo parágrafo**.
- Opcional: se um parágrafo ainda for executado por mais de **~3 linhas** em documentos renderizados em um comprimento de linha típico, divida ainda mais.

## Não adicionar

- **Conteúdo de procedimento &quot;como fazer&quot;**: etapas numeradas, &quot;clique em **[!UICONTROL ...]** e depois...&quot;, apresentações completas da interface do usuário ou frases de tutorial. As notas de versão resumem **o que foi enviado** e **por que é importante**, não lições práticas.
- Conteúdo que viola [Conteúdo proibido](../generate-release-notes/SKILL.md#prohibited-content) na habilidade de geração (sem chaves Jira, URLs somente internas, wiki as-proof etc.).

## Preservar (não retirar nem reescrever estruturalmente)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]` e outros códigos de atalho ExL.
- Links de documentação **relativos** e padrões de âncora existentes: `[phrase](/help/...)` em texto de âncora significativo.
- O selo do Beta é bloqueado exatamente como usado em [exemplos de generate-release-notes](../generate-release-notes/examples.md).

## Lista de verificação do fluxo de trabalho

1. [ ] Confirmar **quais** `###` em `## … {#latest}` estão no escopo (novo nesta rodada).
2. [ ] Para cada `###` dentro do escopo, restringir cópia por [Voz e tom](#voice-and-tone) e [Regras de parágrafo](#paragraph-rules).
3. [ ] Remova ou reduza quaisquer **instruções passo a passo**; mantenha os **resultados do usuário**.
4. [ ] Verifique se os links e os códigos de atalho ainda são válidos; execute uma verificação rápida de IDs internas ou padrões proibidos por [Verificações de qualidade](#quality-checks).

## Verificações de qualidade

- [ ] Apenas os **novos** `###` blocos acordados em `{#latest}` foram alterados; arquivos e meses mais antigos permanecem intocados.
- [ ] Nenhuma ID de estilo Jira nova, URLs wiki internas ou linguagem &quot;ver tíquete&quot;.
- [ ] Os parágrafos são **2-3 frases** cada (máximo de três frases por parágrafo).
- [ A cópia ] permanece **fatual** e alinhada com o recurso descrito.

## Recursos adicionais

- [examples.md](examples.md) — padrões antes/depois.
- [generate-release-notes](../generate-release-notes/SKILL.md) — rascunho, arquivamento, selos do Beta, vinculação.
