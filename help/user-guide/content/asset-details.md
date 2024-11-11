---
title: Detalhes do ativo
description: O Adobe GenStudio for Performance Marketing armazena conteúdo aprovado com metadados avançados para pesquisa e rastreamento de desempenho.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: edd27a6151cb81213ee27813beb4ecee835a1229
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Detalhes do ativo

O Adobe GenStudio for Performance Marketing armazena conteúdo aprovado com metadados avançados para detecção e rastreamento de desempenho.

Cada ativo (incluindo experiências e modelos) associou _detalhes_ (metadados) que ajudam a identificar, rastrear, usar e aprender com o desempenho do conteúdo.

**Para exibir detalhes do ativo**:

1. Em _[!DNL Content]_, selecione um ativo, experiência ou modelo. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição do ativo, revise a seção _[!UICONTROL Detalhes]_ à direita.

   >[!TIP]
   >
   >Se a seção _[!UICONTROL Detalhes]_ não estiver visível, clique no ícone **[!UICONTROL Informações]** (i).

   Os detalhes do ativo incluem metadados aplicados durante o processo de criação ou upload. Os tipos de metadados de ativos incluem [metadados do sistema](#system-metadata) e [metadados definidos pelo usuário](#user-defined-metadata).

>[!NOTE]
>
>O Assets de repositórios AEM exibe metadados diferentes. Consulte [Configurar visibilidade do ativo](connect-aem-repo.md#step-4-configure-asset-visibility) para saber como configurar detalhes do ativo [!DNL AEM Assets Content Hub].

## Editar no Express

Você pode editar ativos de imagem (JPG ou PNG) diretamente no GenStudio for Performance Marketing usando o Adobe Express. A Tela _[!UICONTROL Powered by Adobe Express]_ fornece recursos convenientes para aprimorar suas imagens sem sair do aplicativo do GenStudio. É possível remover facilmente planos de fundo, aplicar preenchimentos gerativos, ajustar efeitos e recortar imagens.

1. Em _[!DNL Content]_, selecione um ativo de imagem. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição de ativos, clique no ícone **[!UICONTROL Editar no Adobe Express]** no canto superior direito.

1. Na Tela _[!UICONTROL Powered by Adobe Express]_, use os controles Expressos no painel esquerdo para aprimorar sua imagem.

1. Quando estiver satisfeito com a imagem atualizada, clique em **[!UICONTROL Salvar uma cópia]** no canto superior direito.

1. Selecione o formato de arquivo - JPG ou PNG - e clique em **[!UICONTROL Salvar uma cópia]**.

1. No pop-up _[!UICONTROL Salvar uma cópia do ativo]_, atualize o **[!UICONTROL Nome do ativo]**.

   - Selecione **[!UICONTROL Mesmos detalhes que o ativo original]** para transferir os detalhes do ativo para a nova imagem.

   - Expanda a seção **[!UICONTROL Mais detalhes]** para atualizar a Campanha, as Diretrizes e outros metadados.

   >[!TIP]
   >
   >Quanto mais detalhes você fornecer, mais conhecerá os recursos avançados do GenStudio for Performance Marketing. Selecione um ou mais detalhes na lista ou insira um novo, onde aplicável, como com palavras-chave. Cada detalhe adicionado aparece abaixo da lista. Clique em **`x`** para remover um detalhe.

1. Clique em **[!UICONTROL Salvar]**.

## Metadados do sistema

Alguns metadados de ativos são coletados automaticamente quando um ativo é carregado. Não é possível editar os metadados padrão do sistema.

Os metadados padrão armazenados e capturados para um ativo incluem o nome do arquivo, as dimensões, a origem e muito mais.

### Tags geradas

Quando você armazena um ativo aprovado no [!DNL Content], a GenStudio for Performance Marketing usa a IA de Adobe e os recursos de aprendizado de máquina para estudar o ativo e aplicar tags com base nos recursos do ativo. Por exemplo, uma imagem de um gato pode resultar em marcas de atributo como `pet photography` ou `cat`, e marcas de cor que identificam cores dominantes na imagem. Não é possível editar tags detectadas e aplicadas automaticamente.

Consulte [!DNL Insights] [Categorias de atributo](/help/user-guide/insights/attribute-category.md) para obter listas detalhadas de recursos de imagem, vídeo e texto.

### Metadados de conteúdo gerados

As informações usadas para gerar um novo ativo ou experiência se tornam metadados, como o prompt usado. Não é possível editar o prompt após a aprovação do conteúdo, mas você pode usá-lo como ponto de partida para gerar algo novo.

## Metadados definidos pelo usuário

Os metadados definidos pelo usuário adicionam contexto de marketing ao conteúdo do ativo, permitindo que os profissionais de marketing entendam como usar e se envolver com o ativo.

Ao [carregar um ativo](/help/user-guide/content/manage-assets.md#add-assets), você pode definir um conjunto de detalhes opcionais do ativo que existem no GenStudio for Performance Marketing como metadados. A inclusão de mais detalhes pode melhorar a identificação de ativos em pesquisas e filtragem.

### Detalhes de metadados

A tabela a seguir detalha os metadados (detalhes do ativo) que você pode definir ao criar um ativo.

| Texto | Descrição |
| ------------- | ----------- |
| Campanhas (nome do projeto) | Metadados padrão capturados e armazenados com o ativo |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) adicionado ao GenStudio for Performance Marketing e publicado para uso |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) adicionado ao GenStudio for Performance Marketing para uso |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) adicionado ao GenStudio for Performance Marketing para uso |
| Canais | Tipos de conteúdo no GenStudio for Performance Marketing para os quais o ativo é usado, como email e Metadados |
| Cronograma | Período para o qual o ativo foi usado, como trimestre, estação, ano etc. Exemplo: `Winter 2023` |
| Região | Regiões para as quais o ativo é usado. Exemplos: `North America`, `APAC`, `Italy` |
| Idioma | Idiomas para os quais o ativo é usado. Exemplo: `Spanish` |
| Palavras-chave | Palavras-chave usadas para identificação adicional de características e finalidade do ativo |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
