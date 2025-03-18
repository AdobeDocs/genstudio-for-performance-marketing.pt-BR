---
title: Preparar um modelo de email para o Adobe GenStudio for Performance Marketing
description: Saiba como criar um modelo de email personalizado para o Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
hidefromtoc: true
recommendations: noCatalog
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Preparar modelo de email para o Adobe GenStudio for Performance Marketing

Normalmente, um designer cria o design visual de um modelo em um programa de design, como o Adobe XD. Depois que um modelo de email for projetado, codificado e testado, você poderá prepará-lo para upload e uso no GenStudio for Performance Marketing.

Consulte [Elementos do modelo](use-templates.md#template-elements).

## Adicionar diretrizes

Antes de preparar um modelo de Metadados, verifique se você adicionou [diretrizes](/help/user-guide/guidelines/overview.md) à sua GenStudio for Performance Marketing e as preencheu com informações abrangentes sobre marcas relevantes. As [diretrizes de marca](/help/user-guide/guidelines/brands.md) influenciam diretamente o conteúdo gerado.

**Exemplo**: se você quiser que o corpo de um modelo de email não tenha mais de 500 caracteres, adicione esse requisito às [diretrizes do canal](/help/user-guide/guidelines/brands.md#channel-guidelines) para o campo &quot;corpo&quot;.

Se as diretrizes não forem adicionadas ao GenStudio for Performance Marketing, os padrões serão usados.

## Codifique um modelo de email

Depois que um modelo é projetado, ele é codificado usando HTML e CSS em linha. O código deve ser limpo e responsivo para vários dispositivos.

Consulte [Exemplos de modelo](/help/user-guide/content/customize-template.md#template-examples).

### Emails de várias seções

Você pode usar [prompts estruturados](/help/user-guide/effective-prompts.md#structured-prompts) durante a geração de conteúdo para instruir o GenStudio for Performance Marketing a gerar conteúdo variável por seção de um email.

Por exemplo, se as seções no seu modelo de email tiverem o prefixo `Pod`—`Pod1` e `Pod2`, o prompt estruturado para geração de conteúdo poderá incluir diretivas específicas para essas seções de email. O GenStudio for Performance Marketing corresponde a diretiva específica da seção no prompt à seção de email relacionada e gera conteúdo alinhado às diretivas.

Consulte [prompts estruturados](/help/user-guide/effective-prompts.md#structured-prompts).

## Testar um modelo de email

Use sua plataforma de entrega ou prova de email para testar seu email e verificar se ele é renderizado corretamente em diferentes clientes e dispositivos de email.

Teste para garantir que seu modelo de email atenda aos seguintes requisitos:

* O layout é ajustado para diferentes tamanhos de tela usando consultas de mídia CSS
* Os botões são clicáveis e navegam até o local desejado
* O modelo de email pode ser lido e usado em dispositivos móveis

## Definir áreas de conteúdo gerado

Defina as áreas no seu modelo de email que devem ser preenchidas dinamicamente com conteúdo do GenStudio for Performance Marketing.

Para definir áreas de conteúdo geradas:

* Identifique os elementos de texto no modelo que o GenStudio for Performance Marketing deve gerar automaticamente, como o título ou o CTA.
* Adapte o modelo do HTML inserindo espaços reservados usando a sintaxe Handlebars.

Consulte [Espaços reservados para conteúdo](/help/user-guide/content/customize-template.md#content-placeholders).

## Pré-visualizar o modelo

Controle a visibilidade de áreas de conteúdo específicas com Auxiliares incorporados. Por exemplo, é possível incluir parâmetros de rastreamento para links em um modelo exportado, mantendo links de visualização limpos.

Consulte [Visualização do modelo](/help/user-guide/content/customize-template.md#template-preview).

## Fazer upload e usar modelo

Depois que seu modelo for projetado, codificado, testado e visualizado, você poderá carregá-lo no GenStudio for Performance Marketing para uso na geração de conteúdo de marketing totalmente novo.

Consulte [Trabalhando com modelos](use-templates.md).
