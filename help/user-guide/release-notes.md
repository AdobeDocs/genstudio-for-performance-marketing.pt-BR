---
title: Notas de versão do Adobe GenStudio for Performance Marketing
description: Saiba mais sobre os recursos e aprimoramentos mais recentes do Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 778be59db2bf159c57095fbb2d89cff8c9704b33
workflow-type: tm+mt
source-wordcount: '3411'
ht-degree: 0%

---

# Notas de versão do GenStudio for Performance Marketing

Estas informações de versão fornecem as atualizações mais recentes para o aplicativo do GenStudio for Performance Marketing.

## 2025.08.15 {#latest}

### Insights para atributos de texto

Os Insights de atributo de texto no Adobe GenStudio analisam o tom emocional, as técnicas de persuasão e o estilo narrativo usados na cópia de anúncio. Quando uma campanha é ativada, o GenStudio acompanha a forma como esses atributos de texto se correlacionam com as principais métricas de desempenho, como CTR, CPA, CPC, impressões e gastos.

No momento, isso está disponível somente para anúncios em inglês. Consulte [Recursos de Texto](/help/user-guide/insights/text-features.md) para obter informações detalhadas.

### Melhorias no modelo de insights

* O cartão Visualização de anúncio agora inclui a opção &quot;Ver mais&quot; para texto.
* Novos modelos para cartões de Alvenaria de página de anúncios.

### Gerar conteúdo em vários idiomas com validação de marca

O novo seletor de Idioma na gaveta de prompt suporta a criação de conteúdo multilíngue, permitindo que os profissionais de marketing regionais desenvolvam conteúdo na marca para seus públicos locais. No momento, esse recurso oferece suporte a 12 idiomas.

### Suporte a ativos de vídeo em modelos

* Os ativos de vídeo podem ser adicionados aos modelos Meta e LinkedIn.

### Ativar melhorias de experiência

* Nova funcionalidade para salvar rascunhos de ativações.
* Nova funcionalidade para repetir ativações com falha.

### Usar a mesma função em vários campos de texto

Agora há suporte para vários campos de texto com a mesma função (por exemplo, &quot;body&quot;, &quot;cta&quot;, &quot;on image text&quot; etc.) para modelos de clientes complexos.

Explore os detalhes em [as orientações para o Editor de Código de Modelo](/help/user-guide/content/code-editor.md).

### Novos modelos de geração de imagens do Firefly compatíveis

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

O Adobe GenStudio for Performance Marketing agora é compatível com o conjunto Firefly Image Model 4 mais recente, incluindo duas variantes avançadas:

**Imagem do Firefly 4**: otimizada para velocidade e simplicidade, ideal para gerar ilustrações, ícones, fotos básicas de objetos e retratos de uma única pessoa, cobrindo 90% das necessidades criativas diárias.

**Firefly Image 4 Ultra**: prioriza o fotorealismo e a precisão, destacando a renderização de retratos humanos, grupos de médio porte e cenas complexas para tarefas criativas sofisticadas.

Consulte [Gerar ativos](/help/user-guide/create/generate-assets.md) para obter informações detalhadas sobre como usar esses novos modelos de geração de imagem.

### Tradução pronta para uso para email

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

O Adobe GenStudio for Performance Marketing agora oferece recursos de tradução de email integrados que permitem aos profissionais de marketing dimensionar suas campanhas de email globalmente de maneira eficiente. Esse recurso permite que você obtenha uma experiência de email aprovada e a traduza para vários idiomas de destino usando os serviços de tradução da IA aberta do Azure.


## Notas de versão anteriores

+++Notas de 2025.07.25

### Filtro de ativos compatíveis

Um novo filtro no módulo [!DNL Insights] oculta automaticamente [ativos de imagem e vídeo não suportados](/help/user-guide/insights/ads.md#ad-formats) das visualizações de anúncios, eliminando a confusão visual e os blocos com falha. Esse aprimoramento garante que os usuários vejam apenas as mídias que estão realmente disponíveis e prontas para uso, criando uma experiência mais limpa e confiável. O filtro funciona junto com o filtro de anúncios de Compatibilidade existente.

### Ativação de vários ativos para o Meta

A Ativação de imagem com proporção múltipla para metadados permite que os anunciantes façam o upload e ativem vários ativos de imagem em proporções diferentes em um único anúncio criativo. Esse recurso permite que um anúncio forneça a adequação criativa certa para vários posicionamentos de Meta, como Feed, Histórias e Bobinas. Os anunciantes podem visualizar como cada imagem será renderizada entre os posicionamentos e publicar todas as versões no Meta em uma única chamada de API.

### Formatação de rich text em variantes

[Editar campos de texto em variantes geradas com formatação rich text](/help/user-guide/create/manage-variants.md#manually-edit-text) opções incluindo negrito, itálico, sublinhado, alinhamento de texto, listas, cor do texto, tamanho do texto e links. Isso permite refinar o texto e o estilo para o público-alvo e aplicar formatação para acomodar os requisitos de layout.

### Rótulos de acessibilidade para imagens e links

Adicione rótulos de acessibilidade (rótulos Aria) a imagens e links do call-to-action em suas variantes para fornecer nomes acessíveis que ajudam os usuários a entender a finalidade dos elementos interativos. Consulte [Gerenciar variantes](/help/user-guide/create/manage-variants.md) para obter instruções detalhadas.

### Geração de conteúdo em outros idiomas

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

O novo menu suspenso Seletor de idioma na gaveta de prompts é compatível com a criação de conteúdo multilíngue, permitindo que os profissionais de marketing regionais desenvolvam conteúdo na marca para seus públicos locais. Atualmente, esse recurso é compatível com 12 idiomas GA e 5 idiomas Beta, com a lista de idiomas fornecendo um fluxo de trabalho definido e uma diretiva de idioma clara para o LLM para saídas mais consistentes.

### Seleção opcional de modelo para meta anúncios

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

A seleção de modelos agora é opcional com Meta anúncios, permitindo que os usuários criem anúncios sem exigir texto e logotipo na parte superior da mídia. Esse aprimoramento permite outros tipos de mídia, como GIFs animados e vídeos que podem não exigir sobreposições de texto ou posicionamento de logotipo.

+++

+++Notas de 2025.06.15

### Modelos iniciais disponíveis

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

Os [modelos iniciais](/help/user-guide/templates/starter-templates.md) oferecem uma maneira de iniciar rapidamente o processo criativo. Agora é possível selecionar um modelo inicial de anúncio do Meta ou LinkedIn.

### Funcionalidade de IA de expansão de geração

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

Agora, no GenStudio for Performance Marketing [!DNL Create] você pode usar os [recursos de IA de expansão gerativa](/help/user-guide/create/manage-variants.md#use-generative-expand) para expandir as dimensões das imagens e adicionar conteúdo gerativo para ajustar os modelos de anúncios em variantes de mídia paga.

### Adicionar vídeos a anúncios

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

Juntamente com o conteúdo da imagem, agora é possível adicionar vídeos ao [LinkedIn](/help/user-guide/create/create-linkedin.md#manage-videos) e ao [Meta](/help/user-guide/create/create-meta-ad.md#manage-videos) anúncios. Veja as visualizações de reprodução automática dos vídeos diretamente no GenStudio for Performance Marketing conforme você escolhe e adiciona vídeos às suas variantes.

### Correções e aprimoramentos

* Adicionado suporte para [publicar experiências de anúncio](/help/user-guide/activation/activate-linkedin-ad.md) do GenStudio for Performance Marketing no LinkedIn Campaign Manager. [!DNL Activate] dá suporte a visualizações detalhadas de anúncios do LinkedIn antes de publicar no Gerenciador de campanhas do LinkedIn.

* A [integração com o Workfront Proof](/help/user-guide/approvals/overview.md) traz os recursos robustos de revisão e aprovação da Proof para a GenStudio for Performance Marketing. O conteúdo revisado no GenStudio for Performance Marketing é sincronizado com o Workfront Proof, e os comentários e o status da revisão são preservados.

* Adicionada a capacidade de [fornecer nomes acessíveis para imagens e links do call-to-action](/help/user-guide/create/manage-variants.md#add-accessibility-labels) em suas variantes, adicionando rótulos de acessibilidade (rótulos de Aria).

* Ao adicionar ou revisar as [Diretrizes da marca](/help/user-guide/guidelines/brands.md) em um idioma diferente do inglês, o GenStudio for Performance Marketing exibe essas diretrizes no mesmo idioma.

* Depois de adicionar manualmente uma [!DNL Brand] ou criar uma [!DNL Brand] por extração manual de um documento, você pode [alterar ou adicionar imagens de miniatura da marca](/help/user-guide/guidelines/add-guidelines.md#change-brand-thumbnail) para garantir que cada marca seja facilmente distinguível na sua lista [!DNL Brands].

* Agora você pode [usar a formatação de edição de rich text](/help/user-guide/create/manage-variants.md#manually-edit-text) nas variantes geradas. Experimente uma variedade de opções de formatação para textos variantes, como cor, tamanho, listas e muito mais.

* Agora você pode [criar um novo conjunto de anúncios](/help/user-guide/activation/activate-meta-ad.md#create-a-new-ad-set) durante a configuração da plataforma, clonando um conjunto de anúncios existente durante a configuração da plataforma. Os conjuntos de metadados definem o tempo, os detalhes do canal e o público-alvo de um anúncio específico. Uma Meta campanha pode conter vários conjuntos de anúncios, mas um conjunto de anúncios é associado exclusivamente a uma campanha.

* Agora você pode exportar detalhes da campanha para torná-los acessíveis externamente como resumos de campanha no Word ou PDF. Selecione uma campanha e clique em **[!UICONTROL Exportar]** (canto superior direito).

+++

+++Notas de 2025.05.15

### Correções e aprimoramentos

* Funcionalidade habilitada para [adicionar texto alternativo](/help/user-guide/create/manage-variants.md#add-alt-text-for-images) a uma imagem para uma variante individual.
* Adição de uma [nova Taxa de proporção Meta](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) —Paisagem 1.19:1 (largura de 1080 pixels).
* Agora é possível escolher mais de uma experiência para exportar ou baixar. Consulte [Exportar experiências](/help/user-guide/content/manage-assets.md#export-experiences).
<!-- * Added support for [publishing ad experiences](/help/user-guide/activation/activate-meta-ad.md) directly from _[!DNL Content]_ [into Google Campaign Manager 360 and Meta Ads Manager](/help/user-guide/activation/activate-cm360-ad.md). -->

+++

+++Notas de 2025.04.15

### Correções e aprimoramentos

* Novas opções de filtro para modelos! Agora você pode refinar sua lista _[!UICONTROL Selecionar modelos]_ em [!DNL Create] e em _[!UICONTROL Conteúdo]_ > _[!UICONTROL Modelos]_. Consulte [Modelos de pesquisa](/help/user-guide/content/use-templates.md#search-templates). Verifique se os modelos estão marcados corretamente com metadados para torná-los detectáveis por meio desses filtros.
* Funcionalidade habilitada para [exibir e selecionar camadas individuais](/help/user-guide/create/manage-variants.md#view-layers)—campos de texto editáveis ou imagens editáveis—de uma experiência para destacá-las para revisões, como regeneração de conteúdo ou recorte de imagens.
* Adição de um [novo campo de modelo](/help/user-guide/content/use-templates.md#template-elements), `sub-headline`, para texto adicional em experiências para capturar a atenção do público e destacar mensagens de marketing.
* Adicionado suporte para [publicar experiências de anúncio](/help/user-guide/activation/overview.md) do GenStudio for Performance Marketing no Google Campaign Manager 360. A Ativate oferece suporte a visualizações detalhadas de anúncios do Google Campaign Manager 360 antes da publicação em um anunciante do Campaign Manager 360. Os anúncios publicados por meio da função Ativar são automaticamente transferidos para os Insights uma vez ao vivo, permitindo que os usuários acompanhem e relatem o desempenho dos anúncios.

+++

+++Notas de 2025.03.13

### Ativar meta anúncios

Agora os profissionais de marketing podem [publicar experiências de anúncios](/help/user-guide/activation/overview.md) do GenStudio for Performance Marketing no Gerenciador de metadados. [!DNL Activate] dá suporte a visualizações detalhadas de Metadados antes da implantação. Os meta anúncios publicados por meio do [!DNL Activate] são automaticamente puxados para o [!DNL Insights] assim que estiverem online, permitindo que os usuários acompanhem e relatem o desempenho do anúncio.

### Criar experiências do LinkedIn

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

Adicionado suporte para [criar experiências do LinkedIn](/help/user-guide/create/create-linkedin.md). Consulte a guia [Anúncio do LinkedIn](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) nas diretrizes específicas do canal.

### Criar experiências com banner

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

Adicionado suporte para [criar experiências de banner](/help/user-guide/create/create-banner-experience.md). Consulte a guia [Banner](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) nas diretrizes específicas do canal.

### Conformidade

Como parte do processo de validação da marca, os [padrões de conformidade](/help/user-guide/guidelines/overview.md) foram introduzidos em [verificações de conteúdo](/help/user-guide/guidelines/brand-validation.md). Essas verificações analisam cada variante em uma experiência em relação às diretrizes do [!DNL Brand], diretrizes da plataforma (como para Meta) e padrões da ADA. Esse processo fornece um resumo abrangente das diretrizes e dos padrões que precisam ser revisados para melhorar a conformidade.

### Extensibilidade

A nova [estrutura de extensibilidade](/help/extensibility/overview.md) do GenStudio for Performance Marketing fornece ferramentas para que as organizações incorporem seus próprios protocolos de conformidade com declarações no fluxo de trabalho de criação de conteúdo e validação por meio de complementos ou aplicativos extensíveis.

### Modelos

* **Editor de código de modelo** — o novo [Editor de código de modelo](/help/user-guide/content/code-editor.md) ajuda a verificar e refinar seu modelo para uso ideal ao gerar novas experiências com o GenStudio for Performance Marketing.

  ![Modo de exibição do editor de código](/help/assets/template-detected-fields.png "Verificar campos detectados"){width="500" zoomable="yes"}

* **Links na imagem** — Personalize seu modelo de email habilitando links de imagem. Consulte [Personalizar um modelo: Link na imagem](/help/user-guide/content/customize-template.md#link-on-image).
* **Modelos do AJO e do Marketo**—Carregue um modelo criado no Adobe Journey Optimizer (AJO) ou no Marketo. Consulte [Trabalhar com modelos do AJO e do Marketo](/help/user-guide/content/use-templates.md#templates-from-ajo-and-marketo).

### Correções e aprimoramentos

* Habilitou a funcionalidade para as diretrizes [canal padrão](/help/user-guide/guidelines/brands.md#channel-guidelines), [imagem](/help/user-guide/guidelines/brands.md#image-guidelines), [logotipo](/help/user-guide/guidelines/brands.md#logos) e [cor](/help/user-guide/guidelines/brands.md#colors) para [[!DNL Brands]](/help/user-guide/guidelines/brands.md).
* Adicionada a capacidade de [adicionar links a imagens](/help/user-guide/create/manage-variants.md#add-image-link) em uma variante.
* A [Verificação de conteúdo](/help/user-guide/guidelines/brand-validation.md) e a funcionalidade de Revisão e aprovação foram movidas para a nova barra de ação direita para maximizar o espaço na Tela e melhorar a experiência do usuário.
* Fluxo simplificado para [carregar ou adicionar manualmente uma marca](/help/user-guide/guidelines/add-guidelines.md#add-brands).
* Introdução da capacidade de [adicionar ou trocar ativos de imagem em uma variante](/help/user-guide/create/manage-variants.md#swap-image) na Tela.
* Melhoria na experiência do usuário e na visibilidade das categorias de canal [em Criar página inicial](/help/user-guide/create/overview.md), separando-as em Mídia própria, Mídia paga e Seções de conteúdo.
* Filtragem aprimorada em [!DNL Insights] exibições de tabela e galeria.

+++

+++Notas de 2025.02.13

### Melhorias na página de aterrissagem para [!DNL Create]

A página de aterrissagem do [!DNL Create] no GenStudio for Performance Marketing inclui aprimoramentos na interface do usuário que melhoram a experiência do usuário. A seção _Trabalho recente_ é refinada e configurada com a exibição em lista como a exibição padrão. O preenchimento e outras melhorias visuais simplificam a aparência da Tela [!DNL Create].

### Exportação de insights para CSV

Agora você pode baixar a tabela visível de qualquer exibição [!DNL Insights] em um arquivo CSV. Esse recurso permite exportar e analisar dados de várias exibições do [!DNL Insights], facilitando a análise de dados e as opções de relatório.

+++

+++Notas de 2025.01.16

### Integração com o Adobe Workfront Proof

[!BADGE Beta]{type=Informative tooltip="No momento, esse recurso está no Beta, portanto, algumas funcionalidades podem estar limitadas ou sujeitas a alterações."}

O programa Beta de integração do GenStudio for Performance Marketing e do Adobe Workfront Proof é iniciado este mês. O Workfront Proof impulsiona o ciclo de vida de criação e ativação de conteúdo com modelos de aprovação, fluxos de trabalho de vários estágios e anotações. Usuários do GenStudio for Performance Marketing com direitos ao Workfront Proof podem usar os recursos avançados do Proof no GenStudio for Performance Marketing para revisar e comentar sobre conteúdo gerado pelo GenStudio.

Os programas da Beta fornecem uma maneira de ajudar a moldar o desenvolvimento de produtos e determinar a disponibilidade geral.

### Gerar novas chamadas para ação

Agora é possível gerar novas frases do call-to-action (CTA) ao gerenciar variantes. Use as novas opções _Rephrase_ e _Adicionar link_ para gerar novas frases e editar o link CTA. Seu modelo deve ser configurado corretamente para que essas novas funções do CTA funcionem. Siga as diretrizes em _Personalizar um modelo_: [Chamadas para ação](/help/user-guide/content/customize-template.md#calls-to-action). Para obter diretrizes sobre o gerenciamento de CTAs em variantes, consulte [Revise Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action). <!-- GS-6676 -->

### Correções e aprimoramentos

* As contagens de caracteres agora são exibidas em todos os campos gerados e manuais de anúncios de exibição. Consulte _Contagens de caracteres_ em [Metaexperiências](/help/user-guide/create/meta-experiences.md#character-counts). <!-- GS-7732 -->

* _Os colaboradores_ agora podem exibir ativos, mas não podem criar, editar ou excluir esses ativos. Anteriormente, os direitos de colaborador não eram aplicados como esperado em [!DNL Create]. <!-- GS-7614 -->

* Agora, os editores de conteúdo podem editar metadados de ativos, experiências e modelos. <!-- GS-4905 -->

* Agora há suporte para tamanhos de imagem personalizados em modelos de Metadados. <!-- GS-7512 -->

* As seleções de persona, marca e produto agora são pré-carregadas durante a geração do modelo. <!-- GS-8069 -->

* O link do call-to-action de email não é mais um campo obrigatório. <!-- GS-8103 -->

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

* Use o botão **[!UICONTROL Atualizar]** na exibição [!DNL Content]Detalhes do ativo _do modelo_ para atualizar o modelo selecionado. <!-- GS-7102 -->

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

* A exportação de metadados agora inclui o rótulo call-to-action selecionado, conforme esperado. <!-- GS-6504 -->

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
