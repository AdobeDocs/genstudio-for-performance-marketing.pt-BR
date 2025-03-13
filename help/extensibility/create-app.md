---
title: Criar um aplicativo do App Builder para estender o GenStudio for Performance Marketing
description: Comece a criar um aplicativo ou complemento.
source-git-commit: cd53f566981a005b24ef1f1951aa2e55c6dd46c1
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Desenvolver um aplicativo do App Builder

Os desenvolvedores que estendem os recursos nativos do GenStudio for Performance Marketing usam o [Adobe App Builder](https://developer.adobe.com/app-builder/) para criar, enviar e implantar seus aplicativos extensíveis ou complementos.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

* Node.js (versão 20.x ou superior)

* npm (empacotado com Node.js)

* Interface de linha de comando (CLI) do Adobe Developer. Para instalar: `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Estrutura do aplicativo

Os complementos do GenStudio for Performance Marketing são aplicativos App Builder e contêm os mesmos componentes básicos que outros aplicativos App Builder.

### Arquivos de build e configuração

Os principais componentes dos aplicativos App Builder incluem esses arquivos de build e configuração. Essa lista não inclui todos os arquivos de build e configuração.

* `README.md`: Inclui informações gerais sobre o aplicativo.

* Arquivos do aplicativo TS:

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* Arquivos de configuração do App Builder:

   * `app.config.yaml`
   * `ext.config.yaml`: arquivo de configuração para o Complemento
   * `app.config.yaml`: arquivo de configuração para o Complemento (inclui definir seu aplicativo como um Complemento do GenStudio for Performance Marketing)
   * `.aio`
   * `.env`: não confirmar o arquivo `.env` no controle de origem

### código Source

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Componentes de código do Source

* `ExtensionRegistration.tsx`: Define as APIs necessárias que o aplicativo host (GenStudio for Performance Marketing) precisa para carregar e exibir o Complemento.

* `App.tsx`: Componente do aplicativo principal que define o roteamento para outros componentes.

* `AdditionalContextDialog.tsx`: Componente da caixa de diálogo para exibir complementos de contexto adicionais.

* `RightPanel.tsx`: Componente da caixa de diálogo para um complemento de validação.

* `Helper` componentes: Inclui `ClaimsChecker`.

## Criar um aplicativo App Builder a partir de um aplicativo existente

Você pode usar um aplicativo de exemplo para iniciar a criação do complemento.

**Para criar um aplicativo App Builder a partir de um aplicativo existente**:

1. Baixe um aplicativo de exemplo do repositório [Exemplos do GenStudio UNIX](https://github.com/adobe/genstudio-uix-examples).

1. No espaço de trabalho Projeto do App Builder em [Adobe Developer Console](https://developer.adobe.com/console/), selecione **[!UICONTROL Baixar tudo]** para baixar os detalhes do Projeto.

1. Abra o aplicativo de exemplo localmente no IDE (Ambiente de desenvolvimento integrado) de sua preferência.

1. Autentique com a interface de linha de comando do Adobe Developer:

   ```bash
   aio login
   ```

1. Baixe o arquivo JSON e crie o aplicativo:

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Adicionar código personalizado ao seu complemento

Você define o código do complemento em arquivos `AdditionalContextDialog.tsx` e `RightPanel.tsx`. Esses dois arquivos definem a aparência e o comportamento do pop-up quando os usuários acessam o complemento.

* `AdditionalContextDialog.tsx`: defina este componente se você planeja usar o Complemento _Adicionar Contexto_. Os usuários interagem com esse componente ao clicar em _Complementos_ na gaveta de prompts em [!DNL Create].

* `RightPanel.tsx`: defina este componente se você planeja usar o Complemento _Painel Direito_ (validação da experiência). Os usuários interagem com esse componente ao clicar no Complemento de validação no painel direito em um rascunho de experiência [!DNL Create].

Agora você está pronto para [Implantar seu aplicativo](deploy-app.md)

## Práticas recomendadas para desenvolvimento de aplicativos

A manutenção de seu ambiente de desenvolvimento pode ajudar você a evitar erros de desenvolvimento e implantação de aplicativos:

* Se você estiver usando uma versão mais antiga de um aplicativo de amostra, atualize as dependências reinstalando-as:

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Atualize o GenStudio UIX SDK. Confirme se você está usando a versão mais recente do [GenStudio UNIX SDK](https://github.com/adobe/genstudio-uix-sdk). Consulte o [Repositório de exemplo do GenStudio UIX](https://github.com/adobe/genstudio-uix-examples) para saber como usar as alterações mais recentes do SDK.
