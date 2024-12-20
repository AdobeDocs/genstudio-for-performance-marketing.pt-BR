---
title: Detalhes do ativo
description: O Adobe GenStudio for Performance Marketing armazena conteúdo aprovado com metadados avançados para pesquisa e rastreamento de desempenho.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: e9c398cc81413fc22746d85abd6444c6bd42efe4
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Detalhes do ativo

O Adobe GenStudio for Performance Marketing armazena conteúdo aprovado com metadados avançados para detecção e rastreamento de desempenho.

Cada ativo (incluindo experiências e modelos) associou _detalhes_ (metadados) que ajudam a identificar, rastrear, usar e aprender com o desempenho do conteúdo.

**Para exibir detalhes do ativo**:

1. Em _[!DNL Content]_, selecione um ativo, experiência ou modelo. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição do ativo, revise a seção _[!UICONTROL Detalhes]_ à direita.

1. Se a seção _[!UICONTROL Detalhes]_ não estiver visível, clique no ícone **[!UICONTROL Informações]** (i).

Os detalhes do ativo incluem metadados aplicados durante o processo de criação ou upload. Os tipos de metadados de ativos incluem [metadados do sistema](#system-metadata) e [metadados definidos pelo usuário](#user-defined-metadata).

O ativo de imagem a seguir contém metadados do sistema que descrevem o tipo de arquivo, o tamanho e outras características, uma palavra-chave definida pelo usuário e vários atributos e cores detectados pela IA.

![detalhes de um ativo com várias marcas](/help/assets/content-asset-details.png)

>[!NOTE]
>
>O Assets de repositórios AEM exibe metadados diferentes. Consulte [Configurar visibilidade do ativo](connect-aem-repo.md#step-4-configure-asset-visibility) para saber como configurar detalhes do ativo [!DNL AEM Assets Content Hub].

## Metadados do sistema

Alguns metadados de ativos são coletados automaticamente quando um ativo é carregado, como tipo de arquivo, tamanho, dimensões, origem e muito mais. Exceto pelo nome do arquivo, não é possível editar os metadados padrão do sistema.

### Tags geradas

Quando você armazena um ativo aprovado no [!DNL Content], a GenStudio for Performance Marketing usa a IA de Adobe e os recursos de aprendizado de máquina para estudar o ativo e aplicar tags com base nos recursos do ativo. Por exemplo, uma imagem de um gato pode resultar em marcas de atributo como `pet photography` ou `cat`, e marcas de cor que identificam cores dominantes na imagem. Não é possível editar tags detectadas e aplicadas automaticamente.

Consulte [!DNL Insights] [Categorias de atributo](/help/user-guide/insights/attribute-category.md) para obter listas detalhadas de recursos de imagem, vídeo e texto.

### Metadados de conteúdo gerados

As informações usadas para gerar um novo ativo ou experiência se tornam metadados, como o prompt usado. Não é possível editar o prompt após a aprovação do conteúdo, mas você pode usá-lo como ponto de partida para gerar algo novo.

## Metadados definidos pelo usuário

Os metadados definidos pelo usuário adicionam contexto de marketing ao conteúdo do ativo, permitindo que os profissionais de marketing entendam como usar e se envolver com o ativo.

Ao [carregar um ativo](/help/user-guide/content/manage-assets.md#add-assets), você pode definir um conjunto de detalhes opcionais do ativo que existem no GenStudio for Performance Marketing como metadados. A inclusão de mais detalhes pode melhorar a identificação de ativos em pesquisas e filtragem.

**Para editar os metadados definidos pelo usuário**:

1. Em _[!DNL Content]_, selecione um ativo, experiência ou modelo. Clicar em um ativo abre uma exibição focada do ativo.

1. Na exibição do ativo, revise a seção _[!UICONTROL Detalhes]_ à direita.

1. Clique em **[!UICONTROL Editar detalhes]** (lápis) para editar os metadados do ativo, da experiência ou do modelo.

   Quanto mais detalhes você fornecer, mais conhecerá os recursos avançados do GenStudio for Performance Marketing. Selecione um ou mais detalhes na lista ou insira um novo, onde aplicável, como com palavras-chave. Cada detalhe adicionado aparece abaixo da lista. Clique em **`x`** para remover um detalhe.

### Detalhes de metadados

A tabela a seguir detalha os metadados (detalhes do ativo) que você pode definir ao criar um ativo.

| Texto | Descrição |
| -------------- | ----------- |
| Título | Nome do ativo; o título padrão pode ser o nome do arquivo original |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) inclua conteúdo promocional com mensagens consistentes para atingir uma meta comercial<br>Ao clicar em um link de campanha, você será direcionado para a página de visão geral da campanha |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) adicionado ao GenStudio for Performance Marketing e publicado para uso |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) adicionado ao GenStudio for Performance Marketing para uso |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) adicionado ao GenStudio for Performance Marketing para uso |
| Canais | Plataformas para distribuição de determinados tipos de conteúdo, como email e anúncios de exibição |
| [!UICONTROL Cronograma] | Intervalo de tempo para o qual o ativo é usado, como trimestre, estação, ano etc. Exemplo: `Winter 2023` |
| Região | Regiões para as quais o ativo é usado. Exemplos: `North America`, `APAC`, `Italy` |
| Idioma | Idiomas para os quais o ativo é usado. Exemplo: `Spanish` |
| Palavras-chave | As palavras-chave definidas pelo usuário são usadas para identificar melhor as características e a finalidade do ativo |

>[!TIP]
>
>Clique em **[!UICONTROL Editar detalhes]** (lápis) para editar os metadados do ativo. Por exemplo, você pode alterar o nome do ativo ou adicionar ou remover palavras-chave.

## Contexto gerativo

A seção [!UICONTROL Contexto Gerativo] mostra quais informações foram usadas para gerar a experiência, como o `Prompt` usado durante o processo [!DNL Create]. Esse insight pode ajudar você a criar variantes ainda mais bem-sucedidas.

As informações podem incluir:

- Parâmetros de `Brand`, `Product` e `Persona` selecionados durante o processo [!DNL Create]
- `Subject line` e `Preheader` para experiências de email
- `Headline` e `Body` para Metadados

## Histórico

Expanda a seção _[!UICONTROL Histórico]_ em uma experiência para exibir uma linha do tempo de aprovações e atividades. Por exemplo, uma experiência aprovada revela a data, a hora e o aprovador da aprovação:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
