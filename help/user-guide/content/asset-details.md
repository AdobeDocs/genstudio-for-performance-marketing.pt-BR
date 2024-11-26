---
title: Detalhes do ativo
description: O Adobe GenStudio for Performance Marketing armazena conteúdo aprovado com metadados avançados para pesquisa e rastreamento de desempenho.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: 7cb19de7f1fe61465046b0d27a528c2f5e1a4d5e
workflow-type: tm+mt
source-wordcount: '508'
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

O ativo de imagem a seguir contém metadados do sistema que descrevem o tipo de arquivo, o tamanho e outras características, uma palavra-chave definida pelo usuário e vários atributos e cores detectados pela IA.

![detalhes de um ativo com várias marcas](/help/assets/content-asset-details.png)

>[!NOTE]
>
>O Assets de repositórios AEM exibe metadados diferentes. Consulte [Configurar visibilidade do ativo](connect-aem-repo.md#step-4-configure-asset-visibility) para saber como configurar detalhes do ativo [!DNL AEM Assets Content Hub].

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
| Cronograma | Período para o qual o ativo é usado, como trimestre, estação, ano etc. Exemplo: `Winter 2023` |
| Região | Regiões para as quais o ativo é usado. Exemplos: `North America`, `APAC`, `Italy` |
| Idioma | Idiomas para os quais o ativo é usado. Exemplo: `Spanish` |
| Palavras-chave | Palavras-chave definidas pelo usuário usadas para identificar melhor as características e a finalidade do ativo |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
