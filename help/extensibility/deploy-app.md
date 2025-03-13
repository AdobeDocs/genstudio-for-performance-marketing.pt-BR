---
title: Implante seu aplicativo App Builder
description: Implante seu aplicativo ou complemento do App Builder para o GenStudio for Performance Marketing.
source-git-commit: acc54215d980f1f7392401cca9d90ed0ce41b2ec
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---


# Implante seu aplicativo

A execução do aplicativo fornece um instantâneo preliminar do comportamento do complemento antes de implantá-lo. Essas informações podem facilitar a depuração. Você pode forçar a criação e a implantação de um aplicativo implantado sem reenviá-lo para aprovação.


**Para executar o aplicativo**:

Executar o aplicativo em `https://localhost:9080`:

```bash
aio app run
```

**Para implantar o aplicativo**:

1. Navegue até o espaço de trabalho Implantação. Por exemplo, para navegar até o espaço de trabalho Produção:

   ```bash
   aio app use -w Production
   ```

1. Implante o aplicativo:

   ```bash
   aio app deploy
   ```

**Para forçar a reimplantação**:

>[!NOTE]
>
>Forçar a criação e a implantação substitui a implantação existente. Primeiro, teste completamente seu aplicativo em um ambiente de teste.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**Para compilar e implantar ao mesmo tempo**:

```bash
aio app deploy --force-build --force-deploy
```

**Para exibir o aplicativo**:

Após a implantação, é possível exibir o aplicativo no GenStudio for Performance Marketing adicionando um parâmetro `query` à URL do GenStudio for Performance Marketing:

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Se você estiver satisfeito com o Complemento, estará pronto para distribuí-lo sem o parâmetro `query`.

Agora você pode [distribuir seu aplicativo](distribute-app.md).
