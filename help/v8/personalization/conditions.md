---
title: Criação de conteúdo condicional
description: Saiba como definir condições para personalizar seu conteúdo no Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: c54f56620570ba9520dc9fc11410d3628641d0a5
workflow-type: tm+mt
source-wordcount: '1069'
ht-degree: 6%

---

# Criar conteúdo condicional {#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Adicionar conteúdo condicional"
>abstract="Configure campos de conteúdo condicional para criar personalizações dinâmicas avançadas com base nos dados do perfil do destinatário. Blocos de texto, links, linha de assunto e/ou imagens são substituídos no conteúdo da mensagem quando uma determinada condição é atendida."

## Introdução ao conteúdo condicional {#gs}

O conteúdo condicional é um recurso poderoso que permite a personalização dinâmica com base nos dados de perfil do recipient. Ele substitui automaticamente blocos de texto e imagens quando condições específicas são atendidas. Esse recurso melhora as campanhas e fornece experiências personalizadas e altamente direcionadas para o seu público-alvo.

Ao configurar campos de conteúdo condicional, você pode criar personalização dinâmica avançada com base no perfil do recipient. Por exemplo, blocos de texto, links, linhas de assunto e imagens são substituídos no conteúdo da mensagem quando uma determinada condição é atendida. Por exemplo, você pode exibir &quot;Sr.&quot; ou &quot;Sra.&quot; de acordo com o valor do campo Sexo no banco de dados do Adobe Campaign ou incluir um link diferente com base no idioma preferencial do recipient.

Para criar conteúdo condicional, configure as condições no **editor de expressão** usando funções auxiliares específicas. Esse método está disponível para todos os canais de entrega, em qualquer campo no qual você pode acessar o editor de expressão, como a linha de assunto, links de email e componentes de conteúdo de texto/botão. [Saiba como acessar o editor de expressão](gs-personalization.md#access).

Além disso, use o **criador de conteúdo condicional** dedicado ao criar um email para criar várias variantes para um elemento do seu corpo de email. [Saiba como criar conteúdo condicional em emails](#condition-condition-builder).

## Criar condições no editor de expressão {#condition-perso-editor}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_conditions"
>title="Condições"
>abstract="Esse menu permite aproveitar as funções auxiliares para definir o conteúdo condicional."

Para definir o conteúdo condicional para um delivery usando o editor de expressão, siga essas etapas. Neste exemplo, o conteúdo condicional é criado com base no idioma dos recipients (francês ou inglês).

1. Abra um delivery e navegue até a seção de edição de conteúdo.

1. Localize o campo ao qual deseja adicionar conteúdo condicional. Por exemplo, adicione conteúdo condicional a uma mensagem SMS.

1. Clique no ícone **[!UICONTROL Abrir caixa de diálogo de personalização]** ao lado do campo para abrir o editor de expressão.

   ![Captura de tela mostrando o ícone Abrir caixa de diálogo de personalização ao lado do campo no editor de mensagens SMS.](assets/open-perso-editor-sms.png){zoomable="yes"}

1. No editor de personalização, navegue até o menu **[!UICONTROL Condições]** à esquerda.

1. Para começar a criar sua condição, clique no ícone &quot;+&quot; ao lado da função **If**. A seguinte linha foi adicionada à tela central: `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Substitua `<FIELD>` por um campo de personalização, como o idioma do destinatário: `recipient.language`.
   * Substitua `<VALUE>` pelo valor a ser satisfeito, como `'French'`.
   * Substitua `Insert content here` pelo conteúdo a ser exibido para perfis que atendam à condição especificada.

     ![Captura de tela mostrando uma condição de exemplo no editor de expressão com espaços reservados para campo, valor e conteúdo.](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. Especifique o conteúdo a ser exibido se os recipients não atenderem à condição. Usar uma função auxiliar **else**:

   1. Coloque o cursor antes da marca de fechamento de expressão `%>` e clique no `+` ao lado da função **Else**.

   1. Substitua `Insert content here` com o conteúdo a ser exibido para perfis que não atendem à condição da função if.

   ![Captura de tela mostrando a função Else adicionada à condição no editor de expressão.](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   Use a função auxiliar **else if** para criar condições com várias variantes de conteúdo. Por exemplo, a expressão abaixo exibe três variantes de uma mensagem dependendo do idioma dos recipients:

   ![Captura de tela mostrando uma condição com várias variantes com base no idioma dos destinatários.](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >Cada vez que uma função auxiliar é adicionada, as marcas de abertura (`<%`) e fechamento (`%>`) são adicionadas automaticamente antes e depois da função.
   >
   >Exemplo após adicionar uma função auxiliar &quot;Else&quot; dentro de uma expressão:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Remova essas tags para evitar erros de sintaxe. Neste exemplo, a expressão corrigida após a remoção das marcas de função **else** é:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Salve o conteúdo e verifique a renderização simulando o conteúdo.

## Criar conteúdo condicional em emails {#condition-condition-builder}

O conteúdo condicional em emails pode ser criado de duas maneiras:
* No editor de expressão, criando uma condição com funções auxiliares.
* Em um construtor de conteúdo condicional dedicado acessível ao criar um email.

A seção a seguir fornece instruções passo a passo sobre como criar condições usando o recurso de conteúdo condicional do Designer de email. Informações detalhadas sobre como criar condições usando o editor de expressão estão disponíveis [aqui](#condition-perso-editor).

Neste exemplo, uma mensagem de email com várias variantes é criada com base no idioma dos recipients. Siga estas etapas:

1. Crie ou abra um delivery de email, edite seu conteúdo e clique no botão **[!UICONTROL Editar corpo do email]** para abrir o espaço de trabalho de design de email.

1. Selecione um componente de conteúdo e clique no ícone **[!UICONTROL Habilitar conteúdo condicional]**.

   ![Captura de tela mostrando o ícone Habilitar conteúdo condicional no designer de email.](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. O painel **[!UICONTROL Conteúdo Condicional]** é aberto no lado esquerdo da tela. Nesse painel, crie várias variantes do componente de conteúdo selecionado usando condições.

1. Configure sua primeira variante. Passe o mouse sobre a **[!UICONTROL Variante - 1]** no painel **[!UICONTROL Conteúdo Condicional]** e clique no botão **[!UICONTROL Adicionar condição]**.

   ![Captura de tela mostrando o botão Adicionar condição no painel Conteúdo Condicional.](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. O modelador de query é aberto, permitindo criar uma condição filtrando os dados do perfil do recipient. [Saiba como trabalhar com o modelador de consultas](../query/query-modeler-overview.md).

   Quando a condição da primeira variante da mensagem estiver pronta, clique em **[!UICONTROL Confirmar]**. Neste exemplo, uma regra direcionada a recipients cujo idioma é &quot;francês&quot; é criada.

   ![Captura de tela mostrando uma condição que direciona destinatários cujo idioma é francês.](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. A regra agora está associada à variante. Para melhorar a compreensão, renomeie a variante clicando no menu de reticências.

1. Configure como o componente deve ser exibido se a regra for atendida ao enviar a mensagem. Neste exemplo, exiba o texto em francês se for o idioma preferencial do recipient.

   ![Captura de tela mostrando a variante de texto em francês no designer de email.](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. Adicione quantas variantes forem necessárias para o componente de conteúdo. Alterne entre as variantes a qualquer momento para verificar como o componente de conteúdo será exibido com base em suas regras condicionais.

   >[!NOTE]
   >Se nenhuma das regras definidas nas variantes for atendida ao enviar a mensagem, o componente de conteúdo exibirá o conteúdo definido na **[!UICONTROL Variante padrão]** do painel **[!UICONTROL Conteúdo condicional]**.

## Usar variáveis para conteúdo condicional {#variables-conditional}

As variáveis podem ser usadas para conteúdo condicional no seu delivery.

Saiba mais sobre [adição de variáveis a uma entrega](../advanced-settings/delivery-settings.md#variables-delivery).

Escolha o elemento onde deseja colocar o conteúdo condicional.

![Captura de tela mostrando o uso de variáveis para conteúdo condicional.](assets/variables-conditional.png){zoomable="yes"}

Para usar sua variável, configure a condição usando o botão **[!UICONTROL Editar expressão]**, conforme mostrado abaixo. Neste exemplo, esta imagem é exibida quando o valor da variável é `launch`.

![Captura de tela mostrando uma condição usando uma variável com o valor &#39;launch&#39;.](assets/variables-condition.png){zoomable="yes"}

Crie outra variante com o valor `reminder`, por exemplo, onde uma imagem diferente é exibida.