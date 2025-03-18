---
title: Editor de código de modelo
description: Saiba como usar o editor de código de modelo no GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Editor de código de modelo

O editor de código de modelo foi projetado para ajudar você a verificar e refinar seu modelo para uso ideal ao gerar novas experiências com o GenStudio for Performance Marketing. O editor é compatível com a sintaxe Handlebars, que usa espaços reservados dentro do modelo para indicar onde o GenStudio for Performance Marketing deve gerar conteúdo para você.

>[!TIP]
>
>Antes de carregar o código HTML do modelo na exibição [!DNL Content] _Modelos_, prepare o modelo inserindo os espaços reservados para conteúdo definidos na orientação [Personalizar modelos](customize-template.md).

## Verificar campos detectados

O painel _[!UICONTROL Verificar campos detectados]_ mostra uma lista de campos que a GenStudio for Performance Marketing reconhece no modelo. Revise a lista e você pode rolar pelo código HTML para observar a formação do seu template.

![Modo de exibição do editor de código](/help/assets/template-detected-fields.png "Verificar campos detectados"){width="600" zoomable="yes"}

Se você observar que um campo está ausente na lista, pesquise o código do modelo e localize o local do campo ausente. Insira o espaço reservado correto usando a sintaxe Handlebars e um [nome de campo reconhecido](/help/user-guide/content/customize-template.md#recognized-field-names). Use o formulário Localizar e substituir, exibido na parte inferior do editor de código, para procurar strings específicas no código. (Windows `CTRL`+`F` ou macOS `CMD`+`F`)

### Fazer uma correção

Se houver erros no modelo, você poderá ver uma mensagem `Template is invalid` que inclui uma breve explicação do problema. No exemplo a seguir, a mensagem indica que o campo `_image` não está em conformidade com a convenção de nomenclatura de campos estabelecida no modelo de vários pods. A mensagem informa ainda que é necessário atualizar o nome do campo com o prefixo correto. Localize o campo `_image` no editor de código de modelo e atualize o nome conforme recomendado.

![Corrigir modelo inválido](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

O painel _[!UICONTROL Verificar campos detectados]_ atualiza para refletir as alterações feitas. Quando estiver satisfeito com o preenchimento e os campos corretos, clique em **[!UICONTROL Avançar]** para continuar [carregando seu modelo](/help/user-guide/content/use-templates.md#add-a-template).
