---
title: Seletor de experiência MFE no Salesforce
description: Saiba como implantar e configurar o MFE do Seletor de experiência no Salesforce Lightning, incluindo CSP, autenticação do Adobe, modelos de email Apex e validação.
feature: Extensibility, Extensions, Experiences
source-git-commit: 99a2b657560d20642b7b92aefb976ba2373ebc7f
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---

# Seletor de experiência MFE no Salesforce

Este tópico explica como clientes e implementadores podem implantar e executar o MFE (micro front-end do Seletor de Experiência) do [!DNL GenStudio for Performance Marketing] em uma organização da Salesforce. Ele abrange etapas do administrador (sem código), etapas do desenvolvedor (implantar e configurar) e configurações relacionadas à segurança, como a Política de segurança de conteúdo (CSP).

Para obter opções de integração MFE genérica, propriedades de configuração e exemplos de estrutura, consulte [MFE do Seletor de Experiência GenStudio](experience-selector.md).

## O que essa integração faz

>[!VIDEO](https://video.tv.adobe.com/v/3491084?captions=por_br&learn=on)

O LWC (Componente Web Lightning) `sfgsmfe` carrega o pacote UMD do Seletor de Experiência da Adobe e o renderiza em `<dialog>` para que os usuários possam escolher uma experiência de [!DNL GenStudio for Performance Marketing].

A integração também pode:

* **Visualizar e decodificar:** mostra a carga selecionada como JSON, HTML decodificado e uma visualização limpa do HTML dentro do LWC.
* **Modelos de email (opcional):** Um fluxo **[!UICONTROL Criar Modelo de Email]** no Salesforce pode chamar o Apex (`EmailTemplateController.createEmailTemplate`) para inserir um registro `EmailTemplate` (HTML, assunto e pasta).

O script do Seletor de Experiência para [!DNL GenStudio for Performance Marketing] é carregado da URL hospedada da Adobe em `experience.adobe.com`, não de um Recurso Estático do Salesforce na implementação típica.

## Pré-requisitos

* **Organização do Salesforce:** Uma sandbox ou organização de produção onde você pode implantar metadados e usar o **[!UICONTROL Lightning App Builder]**.
* **CLI do Salesforce:** A CLI do Salesforce (`sf`) está instalada e autenticada, por exemplo:

  ```bash
  sf org login web --alias <your-org-alias>
  ```

* **Permissões:** os usuários que criam modelos de email precisam de acesso à pasta de modelo de email de destino e de direitos para criar modelos de acordo com suas políticas da organização. O Apex executa `with sharing`.
* **Adobe / GenStudio:** a ID de organização do Adobe IMS e a SUSI `clientId` devem corresponder à configuração do Adobe (consulte [Configurar valores de integração](#configure-integration-values-developer--implementation)).
* **O Navegador/CSP:** o Salesforce deve permitir o carregamento de scripts de `https://experience.adobe.com` (consulte [Configurar política de segurança de conteúdo e URL do Adobe](#configure-content-security-policy-and-adobe-url)).

## Implantar o pacote (desenvolvedor)

O projeto usa o layout Salesforce DX; o diretório de pacote padrão é `force-app`.

1. Na raiz do projeto, implante o código-fonte na organização de destino:

   ```bash
   sf project deploy start --source-dir force-app --target-org <your-org-alias>
   ```

2. Confirme se a implantação é concluída sem erros.

* `force-app/main/default/lwc/sfgsmfe` — Pacote LWC (HTML, JS, CSS, meta).
* `force-app/main/default/classes/EmailTemplateController.cls` — Apêndice para criação de modelo.

O repositório também pode conter Recursos Estáticos (`reactApp`, `sfgsmfe_react`). O carregador [!DNL GenStudio for Performance Marketing] atual em `sfgsmfe.js` usa a URL CDN da Adobe para `standalone.js`; esses Recursos Estáticos não são necessários para esse caminho de carregamento, a menos que você altere a implementação.

## Adicionar o componente a uma página Lightning (admin)

O componente `sfgsmfe` é exposto por:

* Páginas do aplicativo Lightning
* Home pages
* Gravar páginas
* Guias (em uma página Lightning em uma guia personalizada)

Para adicionar o componente:

1. Em **[!UICONTROL Configuração]**, abra o **[!UICONTROL Gerenciador de Aplicativos]**.
1. Crie um **[!UICONTROL Novo Aplicativo Lightning]** (ou abra um aplicativo existente que deseja estender).
   ![O modal do Novo Aplicativo Lightning](./mfe-new-lighting-app.png){width="80%" zoomable="yes"}
1. Abra o aplicativo e selecione **[!UICONTROL Editar]**.
   ![O modal Editar Aplicativo Lightning](./mfe-lightning-edit.png){width="80%" zoomable="yes"}
1. Criar uma **[!UICONTROL Nova Página]** (ou editar uma página Lightning existente).
   ![O modal Nova página](./mfe-lightning-new-page.png){width="60%" zoomable="yes"}
1. No **[!UICONTROL Lightning App Builder]**, arraste o componente **sfgsmfe** para o layout.
1. **[!UICONTROL Salve]**, **[!UICONTROL Ative]** e atribua a página ao aplicativo Lightning correto, aos perfis e à visibilidade do aplicativo para que os usuários desejados possam abri-la.

## Configurar a política de segurança de conteúdo e o URL do Adobe

O LWC injeta uma tag `<script>` cujo `src` aponta para o pacote UMD da Adobe, por exemplo:

`https://experience.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js`

Você deve configurar o Salesforce para que essa origem seja permitida para o carregamento de scripts de acordo com as configurações de segurança da CSP e do Lightning de sua organização.

Se o script não carregar:

1. Abra as ferramentas do desenvolvedor do navegador.
1. Verifique as guias **[!UICONTROL Console]** e **[!UICONTROL Rede]** em busca de solicitações bloqueadas ou violações de CSP.
1. Adicione ou ajuste as **[!UICONTROL URLs confiáveis]** (e qualquer configuração relacionada à sua versão do Salesforce) para `https://experience.adobe.com`, seguindo a documentação atual do Salesforce para Lightning.
   ![Sites Confiáveis do Salesforce CSP](./sf-trusted-urls.png){width="80%" zoomable="yes"}

## Configurar valores de integração (desenvolvedor/implementação)

Vários valores estão definidos no JavaScript LWC para `sfgsmfe`. Normalmente, os clientes os substituem por ambiente.

| Valor | Descrição |
| --- | --- |
| `folderId` | ID da pasta do Salesforce (`00l...`) para modelos de email onde novos modelos são criados. Necessário para Apex; a pasta deve existir e estar acessível ao usuário em execução. |
| `imsOrg` | Identificador da organização IMS da Adobe passado para `GenStudioExperienceSelector.renderExperienceSelectorWithSUSI`. |
| `susiConfig.clientId` | ID do cliente Adobe SUSI para o registro do aplicativo Seletor de experiência. |
| GenStudio `script.src` | URL do pacote UMD `standalone.js`; atualize se o Adobe publicar um novo caminho. |

A criação do modelo de email mapeia campos do GenStudio para o modelo (por exemplo, assunto de `experienceFields`). Ajuste os mapeamentos no LWC se o modelo de conteúdo for diferente.

Para obter detalhes sobre `renderExperienceSelectorWithSUSI` e opções relacionadas, consulte [Propriedades de configuração](experience-selector.md#configuration-properties) no tópico MFE do Seletor de Experiência.

## Apêndice: EmailTemplateController

`EmailTemplateController.createEmailTemplate` normalmente:

* Valida o nome do modelo, a ID da pasta e o HTML não vazio.
* Cria um `EmailTemplate` com `TemplateType = 'custom'`, `HtmlValue`, `Subject`, `Body` e atribuição de pasta.
* Erros de superfície para o LWC até `AuraHandledException`.

Dicas operacionais:

* Respeite as regras de exclusividade e nomenclatura do DeveloperName na organização.
* Confirme a ID da pasta e se o usuário pode criar `EmailTemplate` registros nessa pasta.
* Use os logs de depuração do Salesforce quando o DML não conseguir capturar o erro exato.

## Lista de verificação de validação

Confirme os itens nesta lista após a implantação e a configuração para obter uma validação confiável da integração:

1. A implantação é concluída sem erros.
1. Os usuários podem abrir a página Lightning que contém `sfgsmfe` e ver a interface do usuário do Seletor de Experiência.
1. O componente não mostra um erro de carregamento; a guia Rede retorna HTTP 200 para `standalone.js`.
1. **[!UICONTROL Selecionar uma Experiência GenStudio]** abre o seletor e executa retornos de chamada de seleção.
1. **[!UICONTROL Criar Modelo de Email]** é bem-sucedido quando você usa esse fluxo e o modelo aparece na pasta configurada em **[!UICONTROL Configuração]**.

## Consulte também

* [MFE do GenStudio Experience Seletor](experience-selector.md)
