---
title: Notas de versão do Adobe GenStudio for Performance Marketing Beta
description: Saiba mais sobre os recursos e aprimoramentos mais recentes do Adobe GenStudio for Performance Marketing.
hidefromtoc: true
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 9b5e8b37ba988c3dd4a1e5a828487997375474ac
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Notas de versão do Adobe GenStudio for Performance Marketing Beta

Essas notas destacam correções e aprimoramentos significativos do Adobe GenStudio for Performance Marketing para a semana que terminou em 4 de outubro.

## Novos recursos e melhorias

* O recurso de filtragem no produto foi aprimorado. Problemas com a filtragem por idade e sexo em [!DNL Insights] foram resolvidos.  <!-- GS-1198 -->

* É possível editar ativos de imagem (JPG ou PNG) diretamente usando o Adobe Express. Os editores de conteúdo podem usar a Tela _[!UICONTROL Powered by Adobe Express]_ para remover planos de fundo, aplicar preenchimentos generativos, ajustar efeitos e recortar imagens sem sair do GenStudio for Performance Marketing. <!-- GS-4615 -->

* Melhoria na experiência de carregamento progressivo para variantes geradas, email gerado e mensagens contextuais. <!-- GS-4651 3062-->

* Os editores de conteúdo agora podem usar o recurso de ajuste de corte para cortar imagens renderizadas em variantes. <!-- GS-2342 -->

* Problemas com o redimensionamento e a duplicação de modelos foram resolvidos. <!-- GS-4895 -->

* A validação da marca agora explica a causa das falhas que ocorrem durante a validação.

* As visualizações do modelo agora exibem o texto na imagem conforme esperado. <!-- GS-5917 -->

## Melhorias adicionais e problemas corrigidos

* A Tela de Pintura [!DNL Create] agora renderiza fontes personalizadas de modelos conforme esperado. <!-- GS-3415 -->

* A fonte correta agora é aplicada durante a exportação de Metadados. <!-- GS-5875 -->

* Problemas com o upload do modelo que resultaram em upload bem-sucedido, mas a falta de visibilidade na interface do produto foi resolvida. <!-- GS-4815 5650-->

* Os usuários agora podem recortar manualmente os Metadados após redimensioná-los. <!-- GS-5871 -->

* Os usuários não precisam mais fazer logon duas vezes em uma conta de Metadados do canal quando também estão conectados ao Facebook. <!-- GS-3009 -->

* A visualização da Tela de ativos e experiências agora permanece consistente em todo o processo de criação, revisão e aprovação de conteúdo. <!-- GS-5877 -->

* A Tela de desenho agora exibe apenas quatro variantes ao regenerar após uma operação de redimensionamento. <!-- GS-5869 -->

* A verificação ortográfica baseada em navegador agora funciona como esperado na Tela [!DNL Create]. <!-- GS-5760 -->

* Anúncios de Exibição agora são exportados como arquivos PNG quando **[!UICONTROL Exportar como PNG]** é selecionado. Anteriormente, os anúncios de exibição eram exportados como JPEG quando o formato PNG era selecionado. <!-- GS-5545 -->

* O preenchimento foi aumentado entre o botão **[!UICONTROL Recorte manual]** e o botão **[!UICONTROL Gerar]**. Anteriormente, o botão **[!UICONTROL Recorte manual]** estava parcialmente obscurecido. <!-- GS-6084 -->

* As visualizações do modelo agora exibem as fontes do Google conforme esperado. <!-- GS-5946 -->

* As fontes TypeKit e Google importadas agora são carregadas conforme esperado durante a exportação. <!-- GS-5948 -->

* Solução de problemas com a geração de conteúdo com modelos personalizados. Anteriormente, quando um editor de conteúdo tentava gerar um ativo usando um modelo personalizado, o pop-up de geração não era exibido e o console exibia erros. <!-- GS-5262 -->

* A Tela de rascunho do DisplayAds agora mantém sua posição quando um usuário clica com o botão direito do mouse na Tela antes de clicar com o botão esquerdo do mouse fora do menu de contexto. Anteriormente, a Tela de desenho era deslocada quando o usuário clicava com o botão esquerdo do mouse, o que tornava o conteúdo de rascunho parcialmente inacessível.  <!-- GS-5687 -->

* Os efeitos de carregamento do shimmer agora persistem até que a regeneração da imagem seja concluída.  <!-- GS-5811 -->

* As pontuações de validação de marca não são mais invalidadas depois que um usuário faz edições em emails gerados, Metadados ou anúncios de exibição. Anteriormente, essa pontuação estava oculta. <!-- GS-5379 -->

* Os modelos que têm estilos CSS anexados ao elemento `body` agora são aproveitados conforme esperado durante a exportação de experiências. <!-- GS-5947 -->

* Correção de problemas com o recorte manual de imagens de grandes dimensões. <!-- GS-6039 -->

* Apenas uma mensagem pop-up é exibida quando um usuário adiciona um novo ativo em [!DNL Content]. <!-- GS-5020 -->

* Aprimoramento do desempenho da Tela de desenho durante a edição de texto.  <!-- GS-5118 -->

* Adicionados espaços ausentes entre cadeias de caracteres no Email ou na Meta ad Canvas do [!DNL Create]. <!-- GS-5019 -->

* Os editores agora podem salvar um arquivo com nomes que contêm caracteres especiais após a edição no Express. <!-- GS-6131 -->

### Localização

Esta versão inclui melhorias de localização em toda a interface do produto, incluindo estas áreas de interface:

* A URL para o destino de opção **[!UICONTROL Saiba mais]** no menu de prompts [!DNL Create]. <!-- GS-5029 -->

* Formatos de número adjacentes aos campos de entrada de pesquisa [!DNL Insights] > [!DNL Experience]. <!-- GS-4494 -->

## Problema conhecido

* Fragmentos de email regenerados não aparecem na variante após a seleção. (No entanto, as variantes aparecem depois que o rascunho é reaberto.) <!-- GS-5913 -->
