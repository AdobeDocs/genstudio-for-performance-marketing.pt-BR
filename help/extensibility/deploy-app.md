---
title: Implantar o aplicativo App Builder
description: Implante seu aplicativo ou complemento do App Builder para o GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 7fdd3f54a0a031bfe26b48983de9cd24baad2f62
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 0%

---

# Implante seu aplicativo

A execução do aplicativo oferece um instantâneo preliminar do comportamento do complemento antes de implantá-lo. Essas informações podem facilitar a depuração.

**Para executar o aplicativo**:

Executar o aplicativo em `https://localhost:9080`:

```bash
aio app run
```

**Para implantar o aplicativo**:

1. Navegue até o espaço de trabalho Implantação:

   ```bash
   aio app use -w [deployment_workspace]
   ```

2. Implante o aplicativo:

   ```bash
   aio app deploy
   ```

**Para forçar a reimplantação**:

Você pode forçar uma criação e implantação do seu aplicativo sem reenviá-lo para aprovação.

>[!NOTE]
>
>Forçar uma criação e implantação substitui a implantação existente. **Primeiro teste completamente seu aplicativo** em um ambiente de teste.

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

```txt
https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create
```

Se estiver satisfeito com o Complemento, você estará pronto para distribuí-lo sem o parâmetro `query`.

Agora você pode [distribuir seu aplicativo](distribute-app.md).
