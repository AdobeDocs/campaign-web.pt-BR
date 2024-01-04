---
title: Criação de conteúdo condicional
description: Saiba como definir condições para personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Beta"
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: d3afb758e11faf9c39fb14f0b30f1b9edc913ec3
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 14%

---

# Criar conteúdo condicional{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Adicionar conteúdo condicional"
>abstract="Configure campos de conteúdo condicional para criar personalizações dinâmicas avançadas com base nos dados do perfil do destinatário. Blocos de texto, links, linha de assunto e/ou imagens são substituídos no conteúdo da mensagem quando uma determinada condição é atendida."

## Introdução ao conteúdo condicional {#gs}

O conteúdo condicional é um recurso poderoso que permite criar personalização dinâmica com base no perfil do recipient, substituindo automaticamente blocos de texto e imagens quando determinadas condições são atendidas. Esse recurso pode elevar suas campanhas a novos patamares e fornecer experiências personalizadas e altamente direcionadas ao seu público-alvo.

Ao configurar campos de conteúdo condicional, você pode criar personalização dinâmica avançada com base no perfil do recipient, por exemplo. Blocos de texto, links, linha de assunto e/ou imagens são substituídos no conteúdo da mensagem quando uma determinada condição é atendida. Por exemplo, você pode exibir &quot;Sr.&quot; ou &quot;Sra.&quot; de acordo com o valor do campo Gênero no banco de dados do Adobe Campaign ou incluir um link diferente com base no idioma preferencial do recipient.

Para criar conteúdo condicional, você precisa criar condições no **editor de expressão** usando funções auxiliares específicas. Esse método está disponível para todos os canais de entrega, em qualquer campo em que você possa acessar o editor de expressão, como a linha de assunto ou links de email e componentes de conteúdo de texto/botão. [Saiba como acessar o editor de expressão](gs-personalization.md/#access)

<!--In addition to the expression editor, you can leverage a dedicated **conditional content builder** when designing an email that allows you to build conditions using profile attributes only. [Learn how to create conditional content in emails](#condition-condition-builder)-->

## Criar condições no editor de expressão {#condition-perso-editor}

Para definir o conteúdo condicional para um delivery usando o editor de expressão, siga as etapas abaixo. Neste exemplo, queremos criar conteúdo condicional com base no idioma dos recipients (francês ou inglês).

1. Abra um delivery e navegue até a seção de edição de conteúdo.

1. Localize o campo ao qual deseja adicionar conteúdo condicional. Por exemplo, você pode adicionar conteúdo condicional a uma mensagem SMS.

1. Clique em **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone ao lado do campo para abrir o editor de expressão.

   ![](assets/open-perso-editor-sms.png)

1. No editor de personalização, navegue até o **[!UICONTROL Funções auxiliares]** à esquerda.

1. Para começar a criar sua condição, clique no ícone &quot;+&quot; ao lado da **Se** função. A seguinte linha é adicionada à tela central:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Substituir `<FIELD>` com um campo de personalização, como o idioma do recipient: `recipient.language`.
   * Substituir `<VALUE>` com o valor a satisfazer. Por exemplo, `'French'`.
   * Substituir `Ìnsert content here` com o conteúdo que deseja exibir para os perfis que atendem à condição especificada.

     ![](assets/condition-sample1.png){width="800" align="center"}

1. Especifique o conteúdo que deve ser exibido se os recipients não atenderem à condição. Para fazer isso, use um **else** função auxiliar:

   1. Coloque o cursor antes da tag de fechamento da expressão `%>` e clique no link `+` ao lado da **Mais** função.

   1. Substituir `Ìnsert content here` com o conteúdo que você deseja exibir para os perfis que não atendem à condição da função if.

   ![](assets/condition-sample2.png){width="800" align="center"}

   Você também pode usar a variável **else if** função auxiliar para criar condições com várias variantes de conteúdo. Por exemplo, a expressão abaixo exibe três variantes de uma mensagem dependendo do idioma dos recipients:

   ![](assets/condition-sample3.png){width="800" align="center"}

   >[!NOTE]
   >
   >Cada vez que uma função auxiliar é adicionada, abrindo (`<%`) e fechamento (`%>`) são adicionadas automaticamente antes e depois da função.
   >
   >Exemplo após adicionar uma função auxiliar &quot;Else&quot; dentro de uma expressão: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Remova essas tags para evitar erros de sintaxe. Neste exemplo, a expressão corrigida após a remoção de **else** as tags de função são:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Quando a condição estiver pronta, você poderá salvar o conteúdo e verificar a renderização simulando o conteúdo.

<!--SECTION REMOVED FOR LA > CONDITIONAL CONTENT NOT AVAILABLE ANYMORE FROM THE DEDICATED MENU IN THE EMAIL DESIGNER. ONLY THE EXPRESSION EDITOR IS AVAILABLE FOR NOW

## Create conditional content in emails {#condition-condition-builder}

Conditional content in emails can be created in two ways:
* In the expression editor by building a condition with helper functions,
* In a dedicated conditional content builder that is accessible when designing an email.

Detailed information on how to create conditions using the expression editor is available [here](#condition-perso-editor). The following section provides step-by-step instructions on how to create conditions using the email designer's conditional content capability. In this example, we want to create an email message with multiple variants based on the recipients' language. Follow these steps:

1. Create or open an email delivery, edit its content, and click the **[!UICONTROL Edit email body]** button to open the email designing workspace.

1. Select a content component and click the **[!UICONTROL Enable conditional content]** icon.

    ![](assets/condition-email-enable.png){width="800" align="center"}

1. The **[!UICONTROL Conditional Content]** pane opens on the left-hand side of the screen. In this pane, you can create multiple variants of the selected content component using conditions.

1. Configure your first variant. Hover over **[!UICONTROL Variant - 1]** in the **[!UICONTROL Conditional Content]** pane and click the **[!UICONTROL Add condition]** icon.

1. A rule builder appears. Use profile attributes to create the condition for the first variant of the message and click **[!UICONTROL Confirm]**. In this example, we are creating a rule targeting recipients whose language is 'French'.

    ![](assets/condition-email-rule.png){width="800" align="center"}

1. The rule is now associated to the variant. For better readability, we recommend renaming the variant by clicking the ellipsis menu.

1. Configure how the component should display if the rule is met when sending the message. In this example, we want to display the text in French if it is the recipient's preferred language.

    ![](assets/condition-email-variant1.png){width="800" align="center"}

1. Add as many variants as needed for the content component. You can switch between the variants at any time to check how the content component will display based on their conditional rules.

    >[!NOTE]
    >If none of the rules defined in the variants are met when sending the message, the content component will display the content defined in the **[!UICONTROL Default variant]** from the **[!UICONTROL Conditional Content]** pane.
-->