---
title: Notas de versão do Adobe GenStudio for Performance Marketing
description: Saiba mais sobre os recursos e aprimoramentos mais recentes do Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substanial-update: 2024-11-14T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 720b23061d7e56a9b1e712d7787158c6a1bb771c
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 2%

---

# Notas de versão do GenStudio for Performance Marketing

Estas informações de versão detalham as atualizações mais recentes do aplicativo do GenStudio for Performance Marketing.

## 2024.11.14 {#latest}

### Novos recursos

Adição de suporte para modelos de mídia avançada, permitindo que os clientes reutilizem ativos que já foram publicados por meio de seus próprios canais de conteúdo gerenciado. <!-- GS-6107 -->

### Correções e aprimoramentos

* Quando redimensionados em um navegador diferente do usado para gerar o conteúdo inicial, os rascunhos agora são carregados conforme esperado. <!-- GS-7204 -->

* Todos os caracteres agora são representados corretamente no HTML exportado. <!-- GS-7246 -->

* Os botões no pop-up [!DNL Content] _Experiências_ **[!UICONTROL Exportar]** não estão mais truncados em determinados idiomas. <!-- GS-6873 -->

* Anúncios de exibição criados com modelos dimensionados em 50x50 agora são exportados no tamanho de imagem esperado. Anteriormente, os arquivos PNG eram exportados com o dobro das dimensões esperadas. <!-- GS-7192 -->

* Os erros de modelo que ocorreram quando os anúncios de exibição foram redimensionados agora são resolvidos. <!-- GS-7322 -->

### Localização

Esta versão inclui melhorias na localização em toda a interface do usuário, incluindo:

* Todas as cadeias de caracteres no pop-up [!DNL Content] _Carregar ativo_ agora estão corretamente localizadas. <!-- GS-6872 6770 -->
* Todas as dicas de ferramentas no campo [!DNL Content] _Assets_ view **[!UICONTROL Search]** estão localizadas. <!-- GS-6879 -->
* Ao substituir uma imagem existente em uma variante de email na Tela [!DNL Create], a exibição _Selecionar do Conteúdo_ agora está localizada. <!-- GS-6906 -->

## Notas de versão anteriores

+++Notas de 2024.11.07

### Correções e aprimoramentos

* O ponteiro _Salvar em andamento_ não é mais exibido quando um usuário clica em **[!UICONTROL Carregar nova imagem]** e cancela a operação antes de concluir o carregamento. <!-- GS-6780 -->

* Agora os títulos de experiência são criados corretamente durante a regeneração da experiência. <!-- GS-7006 -->

* Problemas com barras de rolagem oscilantes durante o carregamento de rascunho foram resolvidos. <!-- GS-5587 -->

* O link `View documentation` no pop-up [!DNL Content] _Adicionar seu modelo aprovado_ agora funciona conforme esperado. <!-- GS-6881 -->

* Excluir uma imagem da gaveta do prompt durante uma operação de redimensionamento não resulta mais em erro. <!-- GS-7115 7009 -->

* Selecionar **[!UICONTROL Excluir]** no menu de ações [!DNL Create] (...) agora funciona conforme esperado. <!-- GS-6871 -->

* Os usuários agora podem controlar todos os elementos interativos do modelo de Metadados apenas pelo teclado. <!-- GS-4066 -->

* Adição da extração de dimensões de imagem de campos de imagem de modelo para Exibir modelos de anúncio. As solicitações de corte inteligente agora são enviadas para a dimensão real da imagem e não para o modelo inteiro. <!-- GS-6926 -->

* A cadeia de caracteres `Zoom to fit to screen` foi localizada no email gerado e em Meta ads. <!-- GS-5063 -->

* A gaveta do prompt [!DNL Create] agora fecha conforme esperado quando um usuário clica. <!-- GS-5254 -->

* A exportação de metadados agora inclui o rótulo de chamada para ação selecionado, conforme esperado. <!-- GS-6504 -->

* A pontuação da marca agora é atualizada e mantida conforme esperado para experiências regeneradas. <!-- GS-6535 -->

* A exportação de HTML de Metadados e anúncios de exibição não inclui mais elementos de wrapper `div` e `chrome`. <!-- GS-7116 -->

* Problemas com a renderização de rascunho de email durante a publicação agora são resolvidos. <!-- GS-6394 -->

* O botão **[!UICONTROL Marca]** da Tela de Pintura agora está desabilitado quando uma pontuação de marca não é gerada. <!-- GS-6429 -->

* O botão Facebook/Instagram na barra de ação da Tela de Pintura agora atualiza as renderizações da experiência conforme esperado quando a configuração da Tela de Pintura `ReadOnly` está habilitada. <!-- GS-7039 -->

#### Regeneração de imagem

* O redimensionamento de várias variantes de metadados agora funciona conforme esperado. Anteriormente, o Canvas não exibia variantes regeneradas, mas permanecia em branco. <!-- GS-7010 -->

* A regeneração de fragmentos agora funciona conforme esperado em experiências redimensionadas. <!-- GS-6836 -->

* Gerar novamente as imagens do Metadado após redimensioná-las não resulta mais em um erro. Anteriormente, o redimensionamento de imagens antes da regeneração alterava os metadados do canal de `meta` para `facebook`. <!-- GS-7042 -->

+++

+++Notas de 2024.10.31

### Novos recursos

* O filtro de pesquisa **[!DNL Content]** agora oferece suporte para pesquisa por marca de cor. <!-- GS-5501 -->

* A tela **[!DNL Create]** agora exibe contagens de caracteres para fragmentos de email. <!-- GS-5819 -->

### Correções e aprimoramentos

* Rótulos de leitores de tela ausentes foram adicionados aos elementos `view` para dispositivos móveis e da área de trabalho. <!-- GS-5624 4729 -->

* A linha de assunto do email da Tela **[!DNL Create]** e as áreas de texto pré-cabeçalho agora têm uma altura dinâmica. <!-- GS-6258 -->

* Problemas de layout com bordas de email foram resolvidos. <!-- GS-6631 -->

* O foco do teclado agora funciona conforme esperado no botão **[!DNL Content]** **[!UICONTROL Excluir]**. Anteriormente, esse botão não podia ser acessado ou operado pelo teclado.  <!-- GS-4065 -->

## Versão 2024.10.14 de Disponibilidade geral

Esta versão apresenta o Adobe GenStudio for Performance Marketing, um aplicativo generativo baseado em IA que acelera o planejamento, o desenvolvimento e a análise de campanhas de marketing. O GenStudio for Performance Marketing capacita as equipes de marketing a criar conteúdo multicanal na marca para anúncios, emails e campanhas enquanto fornece insights em tempo real para otimizar o desempenho do conteúdo.

### Recursos

Os principais recursos do produto incluem:

**[!DNL Create]** apresenta a Tela, que oferece uma experiência de prompt estruturado que permite aos editores de conteúdo gerar rapidamente conteúdo e variantes. Os gerentes de sistema treinam o produto de acordo com as diretrizes organizacionais da marca. O [!DNL Create] garante que todo o conteúdo gerado por IA esteja alinhado às diretrizes da sua marca (identidade visual, personalidades de clientes e descrições de produtos) e simplifica a produção de conteúdo de marketing de alto impacto e consistente com a marca.

O **[!DNL Content]** armazena experiências e ativos aprovados com curadoria e compatíveis com a marca. Os usuários do GenStudio for Performance Marketing podem facilmente encontrar, editar, redefinir objetivos e compartilhar ativos aprovados, reduzindo a necessidade de recriar conteúdo do zero para cada campanha.

**[!DNL Reviews and Approvals]** estabelece uma estrutura para os participantes revisarem e aprovarem as variantes geradas antes de salvar em **[!DNL Content]** ou exportar.

O **[!DNL Campaigns]** organiza e gerencia campanhas de marketing, garantindo execução e rastreamento otimizados. Os colaboradores podem visualizar, planejar e rastrear campanhas para gerenciar várias iniciativas de maneira eficaz e garantir a entrega em tempo hábil.

O **[!DNL Insights]** oferece avaliação em tempo real do desempenho do conteúdo, ajudando os profissionais de marketing a otimizarem suas estratégias e tomarem decisões orientadas por dados.

A GenStudio for Performance Marketing integra-se com outros produtos da Adobe Experience Cloud, incluindo o Adobe Express e o Adobe AEM Assets.

+++
