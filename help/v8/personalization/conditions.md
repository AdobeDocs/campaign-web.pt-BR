---
title: Criação de conteúdo condicional
description: Saiba como definir condições para personalizar seu conteúdo no Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 6%

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

Além do editor de expressão, você pode aproveitar uma **construtor de conteúdo condicional** ao criar um email que permite criar várias variantes para um elemento do corpo do email. [Saiba como criar conteúdo condicional em emails](#condition-condition-builder)

## Criar condições no editor de expressão {#condition-perso-editor}

Para definir o conteúdo condicional para um delivery usando o editor de expressão, siga as etapas abaixo. Neste exemplo, queremos criar conteúdo condicional com base no idioma dos recipients (francês ou inglês).

1. Abra um delivery e navegue até a seção de edição de conteúdo.

1. Localize o campo ao qual deseja adicionar conteúdo condicional. Por exemplo, você pode adicionar conteúdo condicional a uma mensagem SMS.

1. Clique em **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone ao lado do campo para abrir o editor de expressão.

   ![](assets/open-perso-editor-sms.png){zoom=&quot;yes&quot;}

1. No editor de personalização, navegue até o **[!UICONTROL Funções auxiliares]** à esquerda.

1. Para começar a criar sua condição, clique no ícone &quot;+&quot; ao lado da **Se** função. A seguinte linha é adicionada à tela central:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Substituir `<FIELD>` com um campo de personalização, como o idioma do recipient: `recipient.language`.
   * Substituir `<VALUE>` com o valor a satisfazer. Por exemplo, `'French'`.
   * Substituir `Ìnsert content here` com o conteúdo que deseja exibir para os perfis que atendem à condição especificada.

     ![](assets/condition-sample1.png){zoom=&quot;yes&quot;}{width="800" align="center"}

1. Especifique o conteúdo que deve ser exibido se os recipients não atenderem à condição. Para fazer isso, use um **else** função auxiliar:

   1. Coloque o cursor antes da tag de fechamento da expressão `%>` e clique no link `+` ao lado da **Mais** função.

   1. Substituir `Ìnsert content here` com o conteúdo que você deseja exibir para os perfis que não atendem à condição da função if.

   ![](assets/condition-sample2.png){zoom=&quot;yes&quot;}{width="800" align="center"}

   Você também pode usar a variável **else if** função auxiliar para criar condições com várias variantes de conteúdo. Por exemplo, a expressão abaixo exibe três variantes de uma mensagem dependendo do idioma dos recipients:

   ![](assets/condition-sample3.png){zoom=&quot;yes&quot;}{width="800" align="center"}

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

## Criar conteúdo condicional em emails {#condition-condition-builder}

O conteúdo condicional em emails pode ser criado de duas maneiras:
* No editor de expressão, criando uma condição com funções auxiliares,
* Em um construtor de conteúdo condicional dedicado que pode ser acessado ao criar um email.

A seção a seguir fornece instruções passo a passo sobre como criar condições usando o recurso de conteúdo condicional do designer de email. Informações detalhadas sobre como criar condições usando o editor de expressão estão disponíveis [aqui](#condition-perso-editor).

Neste exemplo, queremos criar uma mensagem de email com várias variantes com base no idioma dos recipients. Siga estas etapas:

1. Crie ou abra um delivery de email, edite seu conteúdo e clique no link **[!UICONTROL Editar corpo do email]** botão para abrir o espaço de trabalho de design de email.

1. Selecione um componente de conteúdo e clique no botão **[!UICONTROL Ativar conteúdo condicional]** ícone.

   ![](assets/condition-email-enable.png){zoom=&quot;yes&quot;}{width="800" align="center"}

1. A variável **[!UICONTROL Conteúdo condicional]** no lado esquerdo da tela. Nesse painel, você pode criar várias variantes do componente de conteúdo selecionado usando condições.

1. Configure sua primeira variante. Focalizar **[!UICONTROL Variante - 1]** no **[!UICONTROL Conteúdo condicional]** e clique no botão **[!UICONTROL Adicionar condição]** botão.

   ![](assets/condition-add-condition.png){zoom=&quot;yes&quot;}{width="800" align="center"}

1. Um construtor de regras é exibido. Ele fornece **Perfil**, **Mensagem**, e **Entrega** atributos que você pode utilizar para criar sua condição.

   Além disso, a **Condições** O menu fornece condições pré-criadas que você pode adicionar à tela para criar facilmente sua variante. Para usá-las, clique no link **Adicionar** e substitua os elementos entre `<` e `>`símbolos pelos elementos desejados. Certifique-se de que o valor especificado para o `<value>` objeto está entre aspas.

   ![](assets/condition-syntax.png){zoom=&quot;yes&quot;}{width="800" align="center"}

1. Quando a condição da primeira variante da mensagem estiver pronta, clique em **[!UICONTROL Confirmar o]**. Neste exemplo, estamos criando uma regra direcionada a recipients cujo idioma é &quot;francês&quot;.

   ![](assets/condition-example.png){zoom=&quot;yes&quot;}{width="800" align="center"}

1. A regra agora está associada à variante. Para melhorar a compreensão, recomendamos renomear a variante clicando no menu de reticências.

1. Configure como o componente deve ser exibido se a regra for atendida ao enviar a mensagem. Neste exemplo, queremos exibir o texto em francês se for o idioma preferencial do recipient.

   ![](assets/condition-email-variant1.png){zoom=&quot;yes&quot;}{width="800" align="center"}

1. Adicione quantas variantes forem necessárias para o componente de conteúdo. Você pode alternar entre as variantes a qualquer momento para verificar como o componente de conteúdo será exibido com base em suas regras condicionais.

   >[!NOTE]
   >Se nenhuma das regras definidas nas variantes for atendida ao enviar a mensagem, o componente de conteúdo exibirá o conteúdo definido na variável **[!UICONTROL Variante padrão]** do **[!UICONTROL Conteúdo condicional]** painel.
