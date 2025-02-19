---
title: Notas de versão do Adobe GenStudio for Performance Marketing
description: Saiba mais sobre os recursos e aprimoramentos mais recentes do Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substantial-update: 2025-02-13T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 0d55b89d550a8e44e7dd354d809f00699fccf468
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 1%

---

# Notas de versão do GenStudio for Performance Marketing

Estas informações de versão detalham as atualizações mais recentes do aplicativo do GenStudio for Performance Marketing.

## 2025.2.13 {#latest}

### Melhorias na página de aterrissagem para [!DNL Create]

A página de aterrissagem do [!DNL Create] no GenStudio for Performance Marketing inclui aprimoramentos na interface do usuário que melhoram a experiência do usuário. A seção _Trabalho recente_ é refinada e configurada com a exibição em lista como a exibição padrão. O preenchimento e outras melhorias visuais simplificam a aparência da Tela [!DNL Create].

### Exportação de insights para CSV

Agora você pode baixar a tabela visível de qualquer exibição [!DNL Insights] em um arquivo CSV. Esse recurso permite exportar e analisar dados facilmente de várias exibições do [!DNL Insights], facilitando a análise de dados e as opções de relatório.

## Notas de versão anteriores

+++Notas de 2025.1.16

### Integração com o Adobe Workfront Proof

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

O programa Beta de integração do GenStudio for Performance Marketing e do Adobe Workfront Proof é iniciado este mês. O Workfront Proof impulsiona o ciclo de vida de criação e ativação de conteúdo com modelos de aprovação, fluxos de trabalho de vários estágios e anotações. Usuários do GenStudio for Performance Marketing com direitos ao Workfront Proof podem usar os recursos avançados do Proof no GenStudio for Performance Marketing para revisar e comentar sobre conteúdo gerado pelo GenStudio.

Os programas da Beta fornecem uma maneira de ajudar a moldar o desenvolvimento de produtos e determinar a disponibilidade geral.

### Gerar novas chamadas para ação

Agora é possível gerar novas frases de chamada para ação (CTA) ao gerenciar variantes. Use as novas opções _Rephrase_ e _Adicionar link_ para gerar novas frases e editar o link CTA. Seu modelo deve ser configurado corretamente para que essas novas funções do CTA funcionem. Siga as diretrizes em _Personalizar um modelo_: [Chamadas para ação](/help/user-guide/content/customize-template.md#calls-to-action). Para obter diretrizes sobre como gerenciar CTAs em variantes, consulte [Chamada para ação de revisão](/help/user-guide/create/manage-variants.md#revise-call-to-action). <!-- GS-6676 -->

### Correções e aprimoramentos

* As contagens de caracteres agora são exibidas em todos os campos gerados e manuais de anúncios de exibição. Consulte _Contagens de caracteres_ em [Metaexperiências](/help/user-guide/create/meta-experiences.md#character-counts). <!-- GS-7732 -->

* _Os colaboradores_ agora podem exibir ativos, mas não podem criar, editar ou excluir esses ativos. Anteriormente, os direitos de colaborador não eram aplicados como esperado em [!DNL Create]. <!-- GS-7614 -->

* Agora, os editores de conteúdo podem editar metadados de ativos, experiências e modelos. <!-- GS-4905 -->

* Agora há suporte para tamanhos de imagem personalizados em modelos de Metadados. <!-- GS-7512 -->

* As seleções de persona, marca e produto agora são pré-carregadas durante a geração do modelo. <!-- GS-8069 -->

* O link de chamada para ação por email não é mais um campo obrigatório. <!-- GS-8103 -->

* O menu suspenso do seletor [!DNL Brand] agora funciona conforme esperado para modelos. Anteriormente, o seletor não carregava com êxito alguns modelos. <!-- GS-8908 -->

* Os editores agora podem selecionar um máximo de quatro imagens para emails de pod único e Meta ads. <!-- GS-2631 -->

* O valor anual do campo `Created by` de uma experiência aprovada agora permanece consistente, conforme esperado, após a edição dos metadados da experiência. <!-- GS-8344 -->

* Os editores de conteúdo agora podem selecionar um modelo de [!DNL Create] com êxito. Anteriormente, o aplicativo exibia um erro de console quando um editor selecionava um modelo.  <!-- GS-8798 -->

* Problemas com as operações de redimensionamento e regeneração de Meta anúncios foram resolvidos. <!-- GS-8900 -->

* O botão **[!UICONTROL Voltar]** agora retorna os usuários à página anterior ou à página de aterrissagem [!DNL Create], conforme esperado. <!-- GS-8622 -->

+++

+++Notas de 2024.12.12

### Novos recursos

Os editores agora podem executar as seguintes tarefas relacionadas aos metadados:

* Edite os metadados do ativo, da experiência e do modelo. Consulte [detalhes do ativo](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* Exiba as marcas geradas de um ativo na exibição _Detalhes_ de qualquer experiência que use o ativo. Consulte _Tags geradas_ em [Detalhes do ativo](/help/user-guide/content/asset-details.md#generated-tags). <!-- GS-3705 -->

Os editores agora podem especificar valores personalizados para esses aspectos das variantes geradas:

* Largura e altura dos banners da Web em modelos de anúncios de exibição. Esses valores agora são salvos como metadados do modelo. <!-- GS-6735 -->

* Dimensões de imagens em experiências de anúncio de exibição durante o carregamento da imagem.<!-- GS-7166 -->

* Consulte as diretrizes específicas do canal nas [Práticas recomendadas para modelos](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

As opções de exportação agora incluem:

* Exporte anúncios de exibição e Metadados como HTML, JPEG ou PNG. Consulte [Criar uma experiência de anúncio de exibição](/help/user-guide/create/create-display-ad.md) e [Criar uma experiência de meta anúncio](/help/user-guide/create/create-meta-ad.md). <!-- GS-7093 6655 5152-->

Novos recursos adicionais permitem aos editores:

* Use o botão **[!UICONTROL Atualizar]** na exibição _Detalhes do ativo_ do modelo [!DNL Content] para atualizar o modelo selecionado. <!-- GS-7102 -->

* Gere novamente as seções do anúncio de exibição e das variantes de email. Consulte [Criar uma experiência de anúncio de exibição](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) e [Criar uma experiência de email](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Duplicar marcas existentes. Consulte [Gerenciar marcas](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

### Correções e aprimoramentos

* Os títulos dos anúncios de exibição agora são salvos em [!DNL Content], conforme esperado. <!-- GS-7239 -->

* A gaveta do prompt não fecha mais quando um editor clica fora do menu suspenso da gaveta. <!-- GS-7275 -->

* O menu suspenso [!DNL Create] [!DNL Persona]/[!DNL Product] agora é carregado conforme esperado quando ocorre um erro de serviço de URL de miniatura. <!-- GS-7277 -->

* Os anúncios de exibição que contêm elementos que sobrepõem fragmentos agora são editáveis. <!-- GS-7186 -->

* O botão **[!UICONTROL Marca]** da Tela de Pintura agora está desabilitado quando as pontuações da marca não são geradas para uma experiência. <!-- GS-6429 -->

* A Tela de desenho agora exibe experiências redimensionadas em ordem consistente. <!-- GS-7123 -->

* O recorte manual agora usa dimensões de imagem, não dimensões de modelo, ao editar anúncios de exibição. Anteriormente, quando uma imagem era menor que as dimensões especificadas no modelo de anúncio de exibição, a caixa delimitadora usava dimensões de modelo, não dimensões de imagem. <!-- GS-7315 -->

* Agora, os editores podem selecionar até quatro imagens ao criar um anúncio de exibição. <!-- GS-7189 -->

* Agora os rascunhos de anúncio de exibição e Meta ad são carregados conforme esperado quando redimensionados em um navegador diferente. <!-- GS-7204 -->

* Os campos de modelo não utilizados não são mais exibidos no conteúdo gerado.  <!-- GS-5670 -->

* Os editores agora podem clicar uma vez nos links para editar conforme esperado nas variantes geradas. <!-- GS-7423 -->

* [!DNL Create] agora respeita corretamente os privilégios de colaborador. <!-- GS-7614 -->

* O botão **[!UICONTROL Redimensionar]** da Tela de Pintura agora está desabilitado depois que todas as opções de redimensionamento foram selecionadas e renderizadas. <!-- GS-5940 -->

* Os revisores com acesso somente visualização agora podem ampliar e reduzir as variantes durante as revisões. <!-- GS-7371 -->

* O foco do teclado foi adicionado somente aos botões acionáveis na exibição [!DNL Create] _Trabalho recente_. <!-- GS-4060 -->

* A mensagem **Salvando em andamento** exibida durante as operações de salvamento de fragmento de email agora é exibida somente durante a operação de salvamento. Anteriormente, a Tela exibia essa mensagem indefinidamente. <!-- GS-6964 -->

* Os editores agora veem uma mensagem de erro como esperado quando um rascunho não é carregado na área [!DNL Create] _Trabalho recente_.  <!-- GS-8081 -->

* Agora a Tela de Pintura exibe metadados redimensionados e anúncios exibidos na ordem correta.  <!-- GS-7375 -->

* Agora, os editores podem clicar uma vez nos campos de email e exibir anúncios. <!-- GS-6297 -->

* A capacidade de edição de fragmentos para email e Meta ads agora é acionada conforme esperado por um único clique. <!-- GS-8081 -->

* Desempenho aprimorado do botão [!DNL Create] **[!UICONTROL Voltar]**. <!-- GS-6767 -->

+++

+++Notas de 2024.11.14

### Novos recursos

Adição de suporte para exibição de conteúdo estático hospedado em domínios externos. O GenStudio for Performance Marketing valida a fonte de conteúdo definida no modelo e incorpora uma cópia para produzir a pré-visualização do modelo. Consulte [Conteúdo estático](/help/user-guide/content/customize-template.md#static-content). <!-- GS-6107 -->

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

+++

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

* A exportação de Metadados e anúncios de exibição do HTML não inclui mais elementos `div` e `chrome` do invólucro. <!-- GS-7116 -->

* Problemas com a renderização de rascunho de email durante a publicação agora são resolvidos. <!-- GS-6394 -->

* O botão **[!UICONTROL Marca]** da Tela de Pintura agora está desabilitado quando uma pontuação de marca não é gerada. <!-- GS-6429 -->

* O botão Facebook/Instagram na barra de ação da Tela agora atualiza as renderizações da experiência conforme esperado quando a configuração da Tela `ReadOnly` está habilitada. <!-- GS-7039 -->

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

* O foco do teclado agora funciona conforme esperado no botão **[!DNL Content]** **[!UICONTROL Excluir]**. Anteriormente, os usuários não podiam acessar esse botão pelo teclado.  <!-- GS-4065 -->

+++

+++Notas de 2024.10.14 Disponibilidade geral

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
