---
title: Trabalhar com modelos
description: Descubra como usar modelos de maneira eficaz para simplificar seu processo criativo no Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 624629700d8bf7d9e4c0e6d8b4373f40b14d4e05
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 1%

---

# Trabalhar com modelos

O GenStudio for Performance Marketing permite que os criadores de conteúdo produzam conteúdo de marketing consistente na marca rapidamente usando _modelos_. Um modelo reduz significativamente o tempo e o esforço necessários para gerar novo conteúdo, fornecendo um ponto de partida que inclui layouts pré-configurados e elementos de design.

Embora o GenStudio for Performance Marketing não ofereça suporte à criação direta de modelos no aplicativo, você pode facilmente projetar e preparar modelos usando ferramentas de design populares, como o Adobe InDesign, o Illustrator ou o Express. Depois que o design for concluído, você poderá adaptá-lo para uso no GenStudio for Performance Marketing. Comece a usar modelos seguindo estas etapas:

1. **Criar seu Modelo**: use sua ferramenta de design preferencial para criar o layout visual do seu [modelo com elementos](#template-elements), como um pré-cabeçalho, título, corpo, CTA, imagens e rodapé.

2. **Codifique seu modelo**: converta seu design em HTML e CSS em linha para garantir que ele seja limpo e responsivo em vários dispositivos. Considere as [diretrizes de acessibilidade](accessibility-for-templates.md) para ajudar a atingir o público-alvo máximo desejado.

3. **Preparar para o GenStudio for Performance Marketing**: adapte seu modelo do HTML usando a linguagem de modelo Handlebars. Insira espaços reservados para indicar onde o GenStudio for Performance Marketing deve gerar conteúdo dinamicamente. Veja como [Personalizar um modelo](customize-template.md) para o GenStudio for Performance Marketing.

Seguindo essas etapas, você pode criar modelos profissionais e eficazes que estejam prontos para uso no GenStudio for Performance Marketing, permitindo que você produza conteúdo sobre a marca de forma rápida e eficiente.

## Elementos do modelo

Um modelo é um conjunto de instruções definidas com o HTML e o CSS em linha que podem ser usadas para produzir uma experiência de email, anúncio social ou anúncio de exibição. Os elementos do modelo fornecem a estrutura para a criação de conteúdo.

Veja a seguir uma lista dos elementos usados em templates e alguns detalhes sobre suas características:

| **Elemento** | **Canal** | **Descrição** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Pré-cabeçalho** | Email | Uma linha de assunto secundária em um email, normalmente entre 40 e 50 caracteres, que melhora a linha de assunto principal. Ele fica visível na caixa de entrada ao lado do assunto antes que o email seja aberto. |
| **Cabeçalho** | Email | A seção superior do email que o recipient vê ao abrir o email define o tom e fornece o contexto para o conteúdo incluído. |
| **Título** | Meta anúncio, banner e anúncios de exibição, LinkedIn | O primeiro conteúdo que o recipient vê deve ser atraente para capturar interesse. |
| **Texto introdutório** | LinkedIn | A mensagem principal transmite a mensagem principal, semelhante à cópia do corpo. Pode usar até 150 caracteres, incluindo espaços, no máximo quatro emojis e pontuação. |
| **Corpo** | Email, Meta anúncio, Banner e Anúncios de exibição | O texto principal do anúncio transmite a mensagem principal. Deve ser envolvente, informativo e persuasivo para incentivar a ação desejada do público. |
| **CTA** | Email, Meta anúncio, Banner e Anúncios de exibição, LinkedIn | Um botão de frase de chamariz usa uma frase e um link para incentivar o recipient a realizar uma ação específica, como clicar em um link ou fazer uma compra. |
| **Imagens** | Email, Meta anúncio, Banner e Anúncios de exibição, LinkedIn | Aprimorar o apelo visual, dividir o texto e dar suporte à mensagem. As imagens devem ser de alta qualidade e atraentes. |
| **Rodapé** | Email | A seção inferior do email contém conteúdo adicional, como detalhes de contato, links de redes sociais, avisos de isenção de responsabilidade e opções de cancelamento de inscrição. |
| **Sobreposição de Texto** | Meta-anúncio | Texto inserido em uma imagem para suportar e aprimorar o conteúdo do título e do corpo. |

>[!TIP]
>
>Consulte os [nomes de campo reconhecidos](customize-template.md#recognized-field-names) aceitos pelo GenStudio for Performance Marketing para modelos de cada tipo de Canal.

## Personalizar modelo

Você [personaliza seu modelo](customize-template.md) para uso no GenStudio for Performance Marketing inserindo espaços reservados para conteúdo, ou campos, que a IA geradora usa para inserir conteúdo. O GenStudio for Performance Marketing reconhece determinados campos, como o campo `body`, e segue as diretrizes de canal configuradas para a marca selecionada.

>[!TIP]
>
>Siga as [diretrizes de acessibilidade](accessibility-for-templates.md) e as [práticas recomendadas](/help/user-guide/content/best-practices-for-templates.md) para que você possa alcançar mais de seu público-alvo e fornecer uma experiência ideal.

## Gerenciar modelos

A galeria _[!DNL Templates]_exibe seu inventário de modelos personalizados para gerar experiências no GenStudio for Performance Marketing. Você pode filtrar modelos por tipo de canal, como email, Anúncios de exibição, Metadados e Anúncios do LinkedIn.

![Lista de modelos de conteúdo](/help/assets/content-templates-filter.png "Pesquisar os modelos do LinkedIn"){width="650" zoomable="yes"}

### Adicionar um modelo

Antes de carregar um modelo, verifique se ele está totalmente preparado e pronto para uso no GenStudio for Performance Marketing seguindo as orientações de [Personalizar modelos](customize-template.md).

**Para adicionar um modelo**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Modelos]**.

1. Clique em **[!UICONTROL Adicionar modelo]**.

1. No painel _[!UICONTROL Adicionar modelo aprovado]_, procure o arquivo de modelo do HTML ou arraste o arquivo de modelo do HTML para o espaço. Clique em **[!UICONTROL Avançar]**.

1. No painel _[!UICONTROL Verificar campos detectados]_, examine os campos. Verifique se você está usando o modelo correto e se todos os detalhes estão conforme esperado.

   Exemplo de visualização para um modelo de email:

   ![Campos de visualização detectados](/help/assets/template-detected-fields.png){width="650" zoomable="yes"}

   >[!TIP]
   >
   >Se o modelo não estiver correto, clique em **[!UICONTROL Voltar]** e retorne à etapa anterior. Faça upload do arquivo de modelo corrigido. Ou use o [editor de código de modelo](/help/user-guide/content/code-editor.md) para fazer correções simples.

1. Clique em **[!UICONTROL Avançar]** quando estiver satisfeito com a visualização do modelo.

1. No painel _[!UICONTROL Fornecer detalhes do modelo e carregar]_, nomeie o modelo e selecione um tipo de **[!UICONTROL Canal]**.

   O nome do modelo e o tipo de canal são obrigatórios. Os requisitos adicionais podem incluir:

   - **Meta**: requer taxa de proporção
   - **Banner e Anúncio de exibição**: requer Dimensões

1. Adicione quantos detalhes forem possíveis para melhorar a identificação do modelo em pesquisas e filtragem.

1. Clique em **[!UICONTROL Concluído]**.

### Atualizar modelo

Os modelos podem incluir arquivos estáticos, como ícones ou logotipos. [O conteúdo estático](/help/user-guide/content/customize-template.md#static-content) não é armazenado após a criação da visualização do modelo. O GenStudio for Performance Marketing continua fazendo referência ao link de origem fornecido no template. Use Atualizar para atualizar a visualização do modelo com as versões mais recentes desses ativos.

**Para atualizar o modelo**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Modelos]**.

1. Clique em um modelo para obter uma exibição completa e uma lista de detalhes.

1. Clique em **[!UICONTROL Atualizar]** (setas circulares) no canto superior direito para atualizar todos os ativos usados no modelo.

### Criar uma experiência com um modelo

Encontre e use um modelo existente no GenStudio for Performance Marketing para criar mais experiências.

**Para criar uma experiência com um modelo**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Modelos]**.

1. Clique em um modelo para obter uma exibição completa e uma lista de detalhes.

1. Clique em **[!UICONTROL Criar experiência]** (pincel) no canto superior direito para usar o modelo.

1. Continue para [Criar](/help/user-guide/create/overview.md#create-use-cases) uma experiência.

## Modelos do AJO e do Marketo

Você pode fazer upload de um modelo criado no Adobe Journey Optimizer (AJO) ou no Marketo. O GenStudio for Performance Marketing detecta padrões específicos do aplicativo e os ignora, preservando o formulário original para uso contínuo no AJO ou no Marketo. Não é necessário fazer alterações na sintaxe original do AJO ou Marketo.

Os padrões de aplicação reconhecidos incluem:

- **AJO**: `{{profile.*}}`, `{{context.*}}`
- **Marketo**: `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Pré-requisitos**

- O aplicativo (AJO, Marketo) e o GenStudio for Performance Marketing devem pertencer à mesma Organização IMS para integração
- Os usuários devem ter a função &quot;Colaborador&quot; (o nível mais baixo) ou superior

>[!ENDSHADEBOX]

Em seguida, [personalize seu modelo](/help/user-guide/content/customize-template.md) com espaços reservados para indicar onde o GenStudio for Performance Marketing deve gerar conteúdo para você. [Adicione seu modelo](#add-a-template) ao repositório [!DNL Content] e valide o modelo. Faça pequenas correções usando o editor de código.
