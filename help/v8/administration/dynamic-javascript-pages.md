---
title: Trabalhar com páginas dinâmicas do JavaScript
description: Saiba como trabalhar com páginas dinâmicas do JavaScript.
exl-id: b7de9f55-2aef-4ba9-a2a1-e9ca15deacfb
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2df9759bb21eae0630bcbe9130a1a20b165e8cca
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 1%

---

# Trabalhar com páginas dinâmicas do JavaScript {#dynamic-javascript-pages}

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="Páginas JavaScript dinâmicas"
>abstract="As páginas dinâmicas do JavaScript (JSSP) permitem construir páginas do lado do servidor que geram conteúdo dinâmico quando acessados por meio de um URL, como APIs personalizadas, exportações ou lógica de aplicativo da Web. Nessa lista, você pode criar, modificar, duplicar ou excluir uma página dinâmica do JavaScript."

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="Criar página JavaScript dinâmica"
>abstract="Defina um namespace, nome e rótulo para sua página dinâmica do JavaScript e grave o conteúdo usando o código JavaScript. Depois de criado, o namespace e o nome não podem ser modificados."

## Sobre páginas dinâmicas do JavaScript {#about}

As páginas dinâmicas do JavaScript (JSSP) permitem construir páginas do lado do servidor que geram conteúdo dinâmico quando acessados por meio de um URL, como APIs personalizadas, exportações ou lógica de aplicativo da Web. Essas páginas são armazenadas no menu **[!UICONTROL Administração]** > **[!UICONTROL Páginas do Dynamic JavaScript]**, no painel de navegação esquerdo.

![Interface de lista de páginas do Dynamic JavaScript mostrando as opções disponíveis](assets/dynamic-javascript-pages.png)

Na lista de páginas dinâmicas do JavaScript, é possível:

* **Duplicar ou excluir uma página**: clique no botão de reticências e selecione a ação desejada.
* **Modificar uma página**: clique no nome de uma página para abrir suas propriedades, fazer suas alterações e salvar.
* **Criar uma nova página dinâmica do JavaScript**: clique no botão **[!UICONTROL Criar página dinâmica do JavaScript]**.

<!--
>[!NOTE]
>
>In the Campaign console, dynamic JavaScript pages are available under **[!UICONTROL Administration]** > **[!UICONTROL Configuration]** > **[!UICONTROL Dynamic JavaScript pages]**. Although the menu location differs from the Web user interface, the list is identical and operates like a mirror.
-->

## Criar uma página dinâmica do JavaScript {#create}

Para criar uma página dinâmica do JavaScript, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Páginas do Dynamic JavaScript]** e clique no botão **[!UICONTROL Criar página do Dynamic JavaScript]**.

1. Defina as propriedades da página:

   * **[!UICONTROL Namespace]**: especifique o namespace relevante para seus recursos personalizados. Por padrão, o namespace é &quot;cus&quot;, mas pode variar dependendo da implementação.
   * **[!UICONTROL Nome]**: o identificador exclusivo usado para fazer referência à página.
   * **[!UICONTROL Rótulo]**: o rótulo descritivo exibido na lista de páginas dinâmicas do JavaScript.

   ![Interface de criação de página do Dynamic JavaScript mostrando os campos de namespace, nome e rótulo](assets/dynamic-javascript-pages2.png)

   >[!NOTE]
   >
   >Depois de criados, os campos **[!UICONTROL Namespace]** e **[!UICONTROL Nome]** não podem ser modificados. Para fazer alterações, duplique a página e atualize conforme necessário.

1. Clique no botão **[!UICONTROL Criar código]** para definir o conteúdo da página e, em seguida, escreva o código JSSP usando diretivas `<%@ page %>` e chamadas `NL.require()` para carregar as bibliotecas principais.

   ![Editor de código de página do Dynamic JavaScript](assets/dynamic-javascript-pages4.png)

1. Clique em **[!UICONTROL Confirmar]** para salvar seu código.

1. Quando a sua página dinâmica do JavaScript estiver pronta, clique em **[!UICONTROL Criar]**. A página agora está acessível em uma URL criada a partir de seu namespace e nome, no formato `https://<your-instance>/<namespace>/<name>`. Por exemplo, uma página chamada `recipientAPI.jssp` no namespace `cus` está acessível em `https://<your-instance>/cus/recipientAPI.jssp`.

Para obter mais informações sobre funções JavaScript reutilizáveis, consulte [Trabalhar com códigos JavaScript](javascript-codes.md).
