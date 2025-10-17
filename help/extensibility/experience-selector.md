---
title: GenStudio Experience Seletor MFE
description: Entenda e implemente o Experience Seletor Micro FrontEnd para seus aplicativos e complementos do GenStudio.
feature: Extensibility, Extensions, Experiences
source-git-commit: d6e580763d85df6d9d295d4e87501af4b022f57b
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# GenStudio Experience Seletor MFE

O Seletor de experiência é um Micro Frontend (MFE) que fornece um componente `ExperienceSelectorDialog` para selecionar experiências do GenStudio. Use o componente em seu aplicativo importando a função `renderExperienceSelectorWithSUSI` do pacote JavaScript independente, que carrega automaticamente o Micro Frontend implantado mais recente e apresenta uma interface de componente natural.

O GenStudio Experience Seletor MFE permite aos usuários:

- Procurar e selecionar experiências do GenStudio
- Filtrar experiências por vários critérios
- Suporta os modos de seleção única e múltipla
- Gerenciar autenticação por meio da integração SUSI (Logon de inscrição)
- Fornecer uma interface consistente em diferentes estruturas

## Opções de integração

A MFE pode ser integrada através de duas abordagens diferentes:

### ESM (Módulos ES) - recomendado

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Definição de módulo universal)

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Propriedades de configuração

A função `renderExperienceSelectorWithSUSI` aceita um objeto de configuração com as seguintes propriedades:

| Propriedade | Tipo | Obrigatório | Descrição |
|----------|------|----------|-------------|
| `apiKey` | string | Sim | Chave de API para serviços da GenStudio |
| `imsOrg` | string | Sim | IMS Organization ID |
| `env` | string | Sim | Ambiente (`stage`, `prod`) |
| `susiConfig` | objeto | Sim | [Configuração de autenticação SUSI](#susi-configuration) |
| `onSelectionConfirmed` | função | Sim | Retorno de chamada quando a seleção é confirmada |
| `onDismiss` | função | Sim | Retorno de chamada quando a caixa de diálogo é descartada |
| `locale` | string | Não | Localidade do idioma (por exemplo, `en-US`) |
| `isOpen` | booleano | Não | Estado inicial da caixa de diálogo |
| `selectionType` | string | Não | O modo de seleção (`single` ou `multiple`) |
| `customFilters` | matriz | Não | Critérios de filtro personalizados |
| `dialogTitle` | string | Não | Título da caixa de diálogo personalizada |

### Configuração do SUSI

O objeto `susiConfig` pode incluir:

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## Início rápido

1. **Escolha sua estrutura** dentre os exemplos disponíveis abaixo
1. **Navegue até o diretório de exemplo**
1. **Instalar dependências** (para exemplos de React/Vue)
1. **Atualize a configuração** com suas chaves de API e organização IMS:

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Executar o servidor de desenvolvimento**

### Exemplos de implementações

Este repositório inclui exemplos de trabalho para estruturas diferentes:

- [Um aplicativo React completo demonstrando integração com o sistema de compilação Vite](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [Um aplicativo do Vue 3 com integração de API de composição](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Duas implementações básicas do JavaScript](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js):

- [Esta versão do Vanilla ESM usa módulos ES6 e o JavaScript moderno](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

- [Esta versão de UMD Vanilla usa o pacote UMD carregado pela marca de script &#x200B;](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Fluxo de autenticação

O Seletor de experiência lida com autenticação automaticamente por meio do SUSI:

1. Quando a caixa de diálogo for aberta, ela verificará a autenticação existente.
1. Se não estiver autenticado, ele abre um fluxo de logon SUSI.
1. Após a autenticação bem-sucedida, o seletor de experiência é exibido.
1. Os usuários podem procurar e selecionar experiências.
1. As experiências selecionadas são retornadas por meio do retorno de chamada `onSelectionConfirmed`.
