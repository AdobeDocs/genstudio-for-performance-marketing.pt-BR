---
title: Validação da marca no Adobe GenStudio for Performance Marketing
description: Saiba como o sistema integrado de validação de marca funciona no GenStudio for Performance Marketing.
feature: Brands Service, Guidelines
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: e4f552016fe17d2d7eb61792b62859475f107094
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 0%

---

# Validação da marca

Na GenStudio for Performance Marketing, a validação da marca é um componente essencial que funciona em colaboração com a funcionalidade e as diretrizes da IA gerativa—[[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) e [[!DNL Personas]](/help/user-guide/guidelines/personas.md). Ele garante que todo o seu conteúdo esteja alinhado à identidade da sua marca, aos padrões ADA e à orientação individual da plataforma de canal.

A GenStudio for Performance Marketing realiza a validação da marca e outras verificações de conteúdo em vários aspectos, incluindo:

* Diretrizes [!DNL Brand], [!DNL Persona] e [!DNL Product] definidas ou padrão
* Diretrizes da plataforma
* Considerações éticas relacionadas a gênero, etnia, raça, status de deficiência e idade no conteúdo gerado por IA
* Padrões da Lei Americana com Deficiência (ADA)

## Resumo da verificação de conteúdo

Um resumo da validação de marca e outras informações de verificação de conteúdo para cada variante de conteúdo gerada podem ser acessadas por meio do ícone de resumo _Verificação de conteúdo_ para cada variante na Tela.

O resumo de _Verificação de conteúdo_ exibe:

* Porcentagem de conformidade com suas [[!DNL Brand]](brands.md) calculada como o número de [diretrizes](overview.md) que passaram na validação em comparação ao número de diretrizes testadas
* `Pass` ou `Fail` resultado para as diretrizes da plataforma, como Meta ou LinkedIn
* `Pass` ou `Fail` resultado para padrões de acessibilidade ADA

![Resumo da verificação de conteúdo](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Clique na porcentagem para ver a compatibilidade da variante. As pontuações são atualizadas automaticamente à medida que você edita as variantes. Você pode clicar em _Exibir e corrigir problemas_ para garantir mais conformidade.

Consulte [Melhorar o alinhamento da marca](#improve-brand-alignment).

## Painel de verificação de conteúdo

O painel _Verificação de conteúdo_ é aberto no lado direito da Tela quando clicado na barra de ação direita _ou_ no ícone de resumo [_Verificação de conteúdo_](#content-check-summary) de uma variante. Esse painel oferece validação detalhada da marca. diretrizes da plataforma e informações sobre padrões de acessibilidade iluminam oportunidades de melhoria para cada seção de variante.

![Painel de verificação de conteúdo](/help/assets/content-check-panel.png){height="250" zoomable="yes"}

O painel _Verificação de conteúdo_ exibe as [informações de conformidade](/help/user-guide/guidelines/overview.md#compliance) e validação para cada seção da variante:

* Representação das informações de resumo da _Verificação de conteúdo_ para [!DNL Brand], diretrizes da plataforma e padrões de acessibilidade
* A seção _Precisa de revisão_ exibindo o número de diretrizes com falha e informações detalhadas sobre cada diretriz que precisa de revisão
* Seção _Aprovadas_ exibindo o número de diretrizes aprovadas e informações detalhadas sobre cada diretriz aprovada

Consulte [Melhorar o alinhamento da marca](#improve-brand-alignment) para saber como melhorar as pontuações do painel _Verificação de conteúdo_.

### Tipo de conteúdo

No painel _Verificação de conteúdo_, é possível alternar quais verificações de diretrizes e padrões de acessibilidade são executadas. Clique no ícone _Tipo de conteúdo_ (ícone de níveis) na parte superior do painel para ativar ou desativar:

* **[!DNL Brand]** — Executa as verificações associadas a [!DNL Brand] diretrizes
* **Diretrizes da plataforma** — Executa as verificações associadas à plataforma específica do canal, como Meta
* **Acessibilidade** — Executa as verificações associadas aos padrões de acessibilidade ADA

Para **definir o tipo de conteúdo** para as verificações que deseja executar, clique para desativar ou nos tipos disponíveis e clique em **Aplicar**.

## Melhorar o alinhamento da marca

Para maximizar a eficácia do conteúdo gerado e manter a identidade de marca consistente, use o resumo da [_Verificação de conteúdo_](#content-check-summary) e o painel [_Verificação de conteúdo_](#content-check-panel). Você pode modificar manualmente seções específicas para alinhar-se às suas [[!DNL Brand] diretrizes](brands.md), verificações de diretrizes da plataforma e verificações de padrões de acessibilidade.

**Para melhorar o alinhamento da marca para variantes geradas**:

1. Clique no ícone do painel _Verificação de conteúdo_, na barra de ação à direita, para ver as informações de validação e acessibilidade de uma única variante.

   Você pode ver um resumo das verificações de _Precisa de revisão_ e _Aprovado_ para ver quais seções e diretrizes precisam ser aprimoradas.

   >[!NOTE]
   >
   > A diretriz _Voz da marca_ anotada no painel _Verificação de conteúdo_ aplica-se a toda a variante, não a uma seção individual. Toda a variante de conteúdo é destacada para melhoria sugerida.

1. Clique para corrigir as diretrizes que não estão em conformidade no momento.
1. Clique para expandir e inspecionar cada verificação que precisa de revisão em seções disponíveis, como _Título_ e _Voz da marca_.

   Use o raciocínio fornecido para cada verificação para orientá-lo na revisão das variantes.

1. Depois de fazer as revisões necessárias, clique em **[!UICONTROL Verificar novamente a pontuação]** para verificar novamente e validar suas alterações para garantir que elas estejam mais alinhadas à identidade da sua marca, às diretrizes da plataforma e aos padrões de acessibilidade.

   O processo de verificação de conteúdo é executado novamente. Se os itens revisados passarem na validação, um banner verde será exibido na parte inferior da Tela para confirmar se a pontuação foi atualizada. Se não houve alteração após uma nova verificação, o banner confirma que não houve alteração na pontuação. A porcentagem no ícone de resumo _Verificação de conteúdo_ para a variante revisada também mostra seu progresso.

1. Continue revisando as seções para garantir que toda a variante seja aprovada nas verificações de validação e acessibilidade. Navegue por cada variante usando as setas adjacentes a uma variante individual na Tela de Pintura.

