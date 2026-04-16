---
name: generate-release-notes
description: ""
source-git-commit: 85ad74d3f24fb809b11f57b23bd24a7ae3310f43
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---


# Gerar notas de versão do GenStudio

**Arquivo de destino canônico:** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Exemplos completos:** [exemplos.md](examples.md)

**Mapeamento de campo KT/wiki e caminhos de documento:** [reference.md](reference.md)

## Escopo de edição (estrito)

Ao usar esta habilidade, **o único local** onde você pode **adicionar** ou **editar** o conteúdo do corpo da nota de versão é a seção chefiada com **`## … {#latest}`** (o único bloco que contém a âncora `{#latest}`).

- **Não** edite as **notas de versão anteriores**—qualquer `+++Notes from YYYY.MM.DD+++` bloco recolhível—ou **qualquer** seção mensal `##` mais antiga que não tenha mais `{#latest}`, mesmo quando o tópico parecer relacionado, um link pareça incorreto ou uma cópia pareça duplicada ou desatualizada.
- **Não** &quot;retocar&quot; antes de `###` subseções, marcadores, links ou palavras fora do bloco `{#latest}` atual, a menos que o usuário dê uma solicitação **explícita, separada** que não seja coberta por esta habilidade.
- **Exceção:** [Arquivar a última](#archive-previous-latest) anterior ao introduzir um **novo** bloco `{#latest}` superior: **mover** toda a seção `{#latest}` anterior em uma **nova** recolhível em **notas de versão anteriores** conforme descrito abaixo. Durante essa passagem, **não** regravar ou adicionar a **outros blocos de arquivos** mais antigos.

Se novas informações pertencerem ao documento, coloque-as no cabeçalho **`{#latest}`** atual (ou arquive primeiro e, em seguida, adicione somente no novo `{#latest}`).

## Lista de verificação do fluxo de trabalho

Trabalhe nesta ordem. Copie a lista de verificação e rastreie o progresso das edições de várias etapas.

1. [ ] Abra `help/user-guide/release-notes.md` e leia o bloco `## YYYY.MM {#latest}` atual. Trate as **notas de versão anteriores** como um contexto **somente leitura**, a menos que você esteja executando a etapa de arquivamento na etapa 2.
2. [ ] Se estiver adicionando uma **nova** versão mensal: arquive a versão mais recente atual (consulte [Arquivar versões mais recentes](#archive-previous-latest)).
3. [ ] Adicionar ou editar **somente** a seção `## YYYY.MM {#latest}` principal (mês mais recente na parte superior da lista de versões).
4. [ ] Para cada item, aplique as [Regras de decisão](#decision-rules) (recurso `###` versus **Correções e aprimoramentos**, selo do Beta ou não).
5. [ ] Adicione ou verifique os links de documentação na frase mais relevante (consulte [reference.md](reference.md#documentation-linking)).
6. [ ] Execute [Verificações de qualidade](#quality-checks) antes de concluir.
7. [ ] Preserve [frontmatter](reference.md#frontmatter) na página, a menos que a tarefa atualize explicitamente os metadados.

## Regras de decisão

Use estas regras if/then para que o conteúdo chegue ao lugar certo:

| Se | Depois |
|----|------|
| O recurso é novo e está presente no Beta | Adicione a linha de selo do Beta imediatamente abaixo do cabeçalho `###` (consulte [examples.md](examples.md)). |
| O material da Source rotula explicitamente o item como uma **correção** ou **melhoria** | Coloque-o em `### Fixes and enhancements` com apenas `*` marcadores. |
| O item é um recurso ou uma história de recursos novos | Use uma seção de recurso `###` com 1-3 frases (não a lista de correções). |
| Você não tem certeza se algo é uma correção ou um recurso | O padrão é uma seção de recurso `###`, a menos que a fonte diga claramente correção/aprimoramento. |

**Regra de seção de correções:** não adicione marcadores a **Correções e aprimoramentos**, a menos que a origem esteja rotulada explicitamente como uma correção ou aprimoramento.

## Arquivar o mais recente anterior

Ao introduzir um novo `## YYYY.MM {#latest}`:

1. Recortar toda a seção `## YYYY.MM {#latest}` anterior (do seu cabeçalho até o final do conteúdo dessa versão, antes das próximas `##` ou **notas de versão anteriores**).
2. Cole-o nas **notas de versão anteriores**, dentro de um bloco recolhível **novo**.
3. Substitua o cabeçalho antigo por: `+++Notes from YYYY.MM.DD+++` (use a data de lançamento real; formato definido nas notas existentes no arquivo).
4. Remover `{#latest}` do cabeçalho arquivado; a nova seção superior é a única com `{#latest}`.
5. Mantenha a ordem cronológica dentro das **notas de versão anteriores** (os blocos arquivados mais recentes estão na parte superior, a menos que o arquivo já use uma ordem diferente—**corresponda ao arquivo existente**).

**não** edite o corpo dos **blocos `+++Notes from …+++`** preexistentes ao executar este arquivo—apenas insira o bloco recém-arquivado e preserve os arquivos antigos como estão.

## Estrutura necessária

### Título e introdução da página

Após o primeiro contato, usar:

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

Se o arquivo já usar uma frase de introdução um pouco diferente (por exemplo, &quot;fornece&quot; em vez de &quot;detalhes&quot;), mantenha a consistência com o restante da página.

### Título da versão mais recente

- Formato: `## YYYY.MM {#latest}` para o bloco de lançamento mais recente.
- Somente uma âncora `{#latest}` na página.

### Seções de recursos

- Use `###` para as principais categorias de recursos.
- O tempo presente, 1-3 frases, esclarecer o quê/porquê e as ações do usuário foram úteis.
- Nomes de produtos: `[!DNL Create]`, `[!DNL Content]`, `[!DNL Insights]`, etc.
- Interface do usuário: `[!UICONTROL Control Name]` onde apropriado.
- Ênfase: `_italics_` para áreas/seções da interface do usuário; `**bold**` para termos-chave com moderação.

### Selo Beta

Usar exatamente:

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### Links de documentação

- Padrão: `[link text](/help/user-guide/section/page.md#anchor)`
- Prefira âncoras; vincule a frase que os usuários mais gostam, e não &quot;clique aqui&quot;.

### Correções e aprimoramentos

- As linhas de marcador usam `*`.
- Somente itens rotulados explicitamente como correção/aprimoramento no material de origem.
- Mesmas convenções de link e terminologia que recursos do.

## Conteúdo proibido

- **não** inclua chaves Jira, números de edição internos, URLs somente internas ou links wiki corporativos nas notas de versão publicadas.
- **não** cite documentos de Transferência de Conhecimento, tíquetes ou ferramentas internas como prova — resuma apenas os resultados voltados para o usuário.
- **não** duplicar `{#latest}` em várias seções.

## Verificações de qualidade

Antes de concluir a tarefa:

- [ ] **Escopo:** Somente o bloco `## … {#latest}` foi adicionado ou editado; as **notas de versão anteriores** e as seções mensais mais antigas não foram modificadas, exceto pelo [Arquivar último](#archive-previous-latest) recortar/colar do antigo `{#latest}` em um bloco de arquivo **novo**.
- [ ] Todos os links relativos novos ou alterados são resolvidos para caminhos reais em `help/`, quando possível.
- [ Os recursos do Beta ] incluem o trecho de selo do Beta, quando necessário.
- [ ] A terminologia corresponde às notas de versão existentes (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] Verifique o rascunho em busca de IDs internas acidentais (`[A-Z]+-\d+`), URLs wiki ou linguagem &quot;veja Jira&quot;; remova-as.
- [ ] **Correções e aprimoramentos** contém apenas correções/aprimoramentos rotulados explicitamente.
- [ ] A última seção anterior foi arquivada corretamente quando um novo mês foi adicionado.

## Fontes de conteúdo (resumo)

Ao extrair dos documentos de Transferência de conhecimento ou dos wikis de versão internamente, mapeie os campos conforme descrito em [reference.md](reference.md#internal-sources-kt-and-release-wikis). A página remetida deve ser lida como documentação do usuário independente.

## Opcional: polir novas subseções

Depois de adicionar o novo conteúdo `###` em `{#latest}`, execute as [notas de versão polonesas](../polish-release-notes/SKILL.md) para uma passagem no estilo copyeditor (tom de avanço de benefícios, **2-3 frases por parágrafo**, sem instruções) **only** nas **novas** subseções—**não** das notas de versão anteriores ou do texto preexistente, a menos que seja solicitado explicitamente.

## Recursos adicionais

- [examples.md](examples.md) — exemplos prontos para colar (recursos, correções, bloco de arquivamento).
- [reference.md](reference.md) — notas sobre assuntos principais, caminhos de documentos, estratégia de vinculação.
- [Notas de versão polonesas](../polish-release-notes/SKILL.md) — passagem editorial opcional sobre `###` recém-adicionado em `{#latest}`.
