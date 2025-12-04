---
title: Validação de marca no Adobe GenStudio for Performance Marketing
description: Saiba mais sobre o sistema integrado de validação de marca na GenStudio for Performance Marketing.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 6a33f7e3a769eda459f70e6ab4e8559064ede2b4
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 0%

---

# Validação da marca

Na GenStudio for Performance Marketing, a validação da marca é um componente essencial que funciona em colaboração com a funcionalidade e as diretrizes da IA gerativa—[[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) e [[!DNL Personas]](/help/user-guide/guidelines/personas.md). Ele garante que todo o seu conteúdo esteja alinhado à identidade da sua marca, aos padrões ADA e à orientação individual da plataforma de canal.

A GenStudio for Performance Marketing realiza a validação da marca e outras verificações de conteúdo em vários aspectos, incluindo:

* Diretrizes [!DNL Brand] definidas ou padrão
* Diretrizes da plataforma
* [Suporte para acessibilidade](/help/user-guide/guidelines/brand-validation.md#supporting-your-accessibility-strategy)
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->


## Resumo da verificação de conteúdo

Um resumo da validação de marca e outras informações de verificação de conteúdo para cada item de conteúdo gerado podem ser acessadas por meio do ícone de resumo _Verificação de conteúdo_ para cada variante na Tela.

O resumo de _Verificação de conteúdo_ exibe:

* Porcentagem de conformidade com suas [[!DNL Brand]](brands.md) calculada como o número de [diretrizes](overview.md) que passaram na validação em comparação ao número de diretrizes testadas
* `Pass` ou `Fail` resultado das diretrizes da plataforma, como Meta ou LinkedIn
* `Pass` ou `Fail` resultado para padrões de acessibilidade ADA

![Resumo da verificação de conteúdo](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Clique na porcentagem para ver a compatibilidade da variante. As pontuações são atualizadas automaticamente à medida que você edita as variantes ou outro conteúdo. Você pode clicar em _Exibir e corrigir problemas_ para garantir mais conformidade.

Consulte [Melhorar o alinhamento da marca](#improve-brand-alignment).

## Painel de verificação de conteúdo

O painel _Verificação de conteúdo_ é aberto no lado direito da Tela quando clicado na barra de ação direita _ou_ a partir do ícone de resumo [_Verificação de conteúdo_](#content-check-summary). Este painel oferece validação detalhada da marca, diretrizes da plataforma e informações sobre os padrões de acessibilidade, além de apontar oportunidades para melhorias.

![Painel de verificação de conteúdo](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

O painel _Verificação de conteúdo_ exibe as [informações de conformidade](/help/user-guide/guidelines/overview.md#compliance) e validação para imagens e seções de variantes:

* Representação das informações de resumo da _Verificação de conteúdo_ para [!DNL Brand], diretrizes da plataforma e padrões de acessibilidade
* A seção _Precisa de revisão_ exibindo o número de diretrizes com falha e informações detalhadas sobre cada diretriz que precisa de revisão
* Seção _Aprovadas_ exibindo o número de diretrizes aprovadas e informações detalhadas sobre cada diretriz aprovada

Consulte [Melhorar o alinhamento da marca](#improve-brand-alignment) para saber como melhorar as pontuações do painel _Verificação de conteúdo_.

### Tipo de conteúdo

No painel _Verificação de conteúdo_, é possível alternar quais verificações de diretrizes e padrões de acessibilidade são executadas. Clique no ícone _Tipo de conteúdo_ (ícone de níveis) na parte superior do painel para ativar ou desativar:

* **[!DNL Brand]** — Executa as verificações associadas a [!DNL Brand] diretrizes
* **Diretrizes da plataforma**—Executa as verificações associadas à plataforma específica do canal, como o Meta
* **Acessibilidade** — Executa as verificações associadas aos padrões de acessibilidade ADA

Para **definir o tipo de conteúdo** para as verificações que deseja executar, clique para desativar ou nos tipos disponíveis e clique em **Aplicar**.

## Melhorar o alinhamento da marca

Para maximizar a eficácia do conteúdo gerado e manter a identidade de marca consistente, use o resumo da [_Verificação de conteúdo_](#content-check-summary) e o painel [_Verificação de conteúdo_](#content-check-panel). Você pode modificar manualmente seções específicas para alinhar-se às suas [[!DNL Brand] diretrizes](brands.md), verificações de diretrizes da plataforma e verificações de padrões de acessibilidade.

**Para melhorar o alinhamento da marca para variantes geradas**:

1. Clique no ícone do painel _Verificação de conteúdo_, na barra de ação direita, para ver informações sobre validação e acessibilidade.

   Você pode ver um resumo das _Verificações de necessidades_ e _Aprovadas_ para ver o que precisa ser melhorado.

   >[!NOTE]
   >
   > A diretriz _Voz da marca_ anotada no painel _Verificação de conteúdo_ aplica-se a toda a variante, não a uma seção individual. Toda a variante de conteúdo é destacada para melhoria sugerida.

1. Clique para corrigir as diretrizes que não estão em conformidade no momento.
1. Clique para expandir e inspecionar cada verificação que precisa de revisão em seções disponíveis, como _Título_, _Cor_ e _Voz da marca_.

   Use o raciocínio fornecido para cada verificação para orientá-lo na revisão de imagens e variantes.

1. Depois de fazer as revisões necessárias, clique em **[!UICONTROL Verificar novamente a pontuação]** para verificar novamente e validar suas alterações para garantir que elas estejam alinhadas à identidade da sua marca, às diretrizes da plataforma e aos padrões de acessibilidade.

   O processo de verificação de conteúdo é executado novamente. Se os itens revisados passarem na validação, um banner verde será exibido na parte inferior da Tela para confirmar se a pontuação foi atualizada. Se não houve alteração após uma nova verificação, o banner confirma que não houve alteração na pontuação. A porcentagem no ícone de resumo _Verificação de conteúdo_ para a variante revisada também mostra seu progresso.

1. Continue revisando as seções para garantir que toda a variante seja aprovada nas verificações de validação e acessibilidade. Navegue por cada variante usando as setas adjacentes a uma variante individual na Tela de Pintura.

## Suporte à sua estratégia de acessibilidade

O GenStudio for Performance Marketing inclui verificações de conteúdo projetadas para ajudar os clientes a oferecer suporte a suas próprias práticas recomendadas de acessibilidade.

Esse recurso inclui as seguintes verificações de conteúdo:

* As imagens fornecem um atributo `<alt>`.
* O texto gerado tem 4,5:1 de contraste com seu plano de fundo.
* Palavras ou frases usadas de forma incomum ou restrita, incluindo expressões idiomáticas e jargões, são evitadas.
* Formas expandidas ou significado de abreviações estão disponíveis.
* O conteúdo é legível em um nível de ensino médio inferior.

Os clientes são incentivados a usar esses recursos como parte de sua estratégia de acessibilidade mais ampla, embora permaneçam responsáveis por sua própria conformidade legal e de acessibilidade.
