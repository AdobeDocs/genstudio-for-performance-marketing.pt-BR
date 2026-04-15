---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---
## Propósito

Ajude os assistentes de codificação de IA a fazer edições pequenas e seguras no repositório de documentação do GenStudio for Performance Marketing.

## Arquitetura de alto nível (curta)
- Este repositório é um site de documentação composto por Markdown em `help/` com inclusões compartilhadas em `help/_includes/` e imagens selecionadas em `help/_includes/assets/`.
- O conteúdo das notas de versão, guia do usuário e extensibilidade está disponível em `help/`. As grandes alterações de conteúdo devem preservar o conteúdo principal e a estrutura de cabeçalho existente.
- O site é construído usando o Jekyll e hospedado em páginas do GitHub. O processo de compilação usa convenções Jekyll padrão com alguns plug-ins personalizados.

## Convenções específicas do projeto
- Regras de cursor: a automação e a orientação personalizadas residem em `.cursor/rules/*.mdc`. Exemplos: `.cursor/rules/docs-lint.mdc` (processo lint), `.cursor/rules/generate-release-notes.mdc` (aponta para a habilidade das notas de versão ao editar `help/user-guide/release-notes.md`). Siga estas instruções para tarefas automatizadas.
- Habilidades do agente: os fluxos de trabalho da tarefa ficam em `.cursor/skills/<name>/SKILL.md`. Exemplo: `.cursor/skills/generate-release-notes/SKILL.md` (procedimento completo das notas de versão do GenStudio; use com `examples.md` e `reference.md` na mesma pasta).
- Nomes de arquivos e material de frente:
   - Notas de versão: preserve o conteúdo principal existente do Experience League em `help/user-guide/release-notes.md` (consulte `.cursor/skills/generate-release-notes/reference.md#frontmatter`); a regra reduzida `.cursor/rules/generate-release-notes.mdc` é anexada automaticamente quando esse arquivo é editado.
   - Use kebab-case para arquivos de regras e a extensão `.mdc`.
- Convenções de formatação: os documentos usam o Markdown com sabor do GitHub. Os títulos geralmente seguem as frases em maiúsculas e minúsculas e os parágrafos curtos. Prefira `*` marcadores para listas nas notas de versão e `###` para seções de recursos.

## Diretrizes de estilo da documentação
- Siga o [Guia de Estilo de Escrita do Microsoft](https://learn.microsoft.com/en-us/style-guide/) para obter as práticas recomendadas da documentação técnica:
   - Escreva frases claras e concisas com foco nas ações do usuário
   - Use a voz ativa e o tempo presente
   - Dividir o texto em partes curtas e digitalizáveis
   - Mantenha um tom quente e direto enquanto mantém a precisão técnica
- Criação no Markdown:
   - Use as letras maiúsculas e minúsculas para os cabeçalhos (use as letras maiúsculas apenas na primeira palavra)
   - Manter parágrafos curtos (2-3 frases) para facilitar a leitura
   - Adicionar linhas em branco antes e depois dos cabeçalhos e listas
   - Usar acentos graves para elementos da interface, caminhos de arquivo e código
   - Incluir texto alternativo para todas as imagens
   - Vincular a seções específicas usando texto descritivo

## Regras de segurança para edições (o que a IA deve fazer)
- Nunca adicione IDs Jira, links internos ou referências somente corporativas a documentos públicos. Consulte `.cursor/skills/generate-release-notes/SKILL.md` (seção **Conteúdo proibido**).
- Preservar o YAML de frente exatamente ao editar os arquivos que o incluem. Muitos modelos e notas de versão dependem de chaves fixas (título, descrição, função, exl-id).
- Para correções de linhas, prefira edições automatizadas e idempotentes de `.cursor/rules/docs-lint.mdc` (remova espaços à direita, garanta a nova linha final). Exemplo de comandos usados por humanos:

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Exemplos (o que alterar e como)
- Correções de cópias pequenas: atualize o texto dentro dos arquivos do Markdown `help/`, mantenha os cabeçalhos e as âncoras intactos.
- Atualizações de imagem: faça referência a imagens em `help/_includes/assets/`. Não mova ou renomeie imagens sem atualizar todas as referências.

## Onde procurar primeiro
- `help/_includes/` — fragmentos e imagens compartilhadas.
- `.cursor/rules/` — automação e orientação de impressão; use-as como regras autoritativas para formatação e processos.
- `markdownlint_custom.json` — substituições do markdown local.
- `.github/pull_request_template.md` — Expectativas de PR.

## Quando perguntar ao humano
- Se uma alteração exigir a execução ou a modificação de ferramentas baseadas em Docker (a regra de link menciona Docker) ou afetar os pipelines de build do site.
- Se um arquivo referenciar uma configuração externa desconhecida (por exemplo, `markdownlint.json` está ausente) — pergunte se deseja criar ou ignorar.

## Comandos mínimos para humanos

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

---
Se desejar, posso mesclar isto em `.github/copilot-instructions.md` no repositório (ou ajustar o texto/comprimento). O que devo alterar ou adicionar?
