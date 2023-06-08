---
title: Criação de conteúdo condicional
description: Saiba como definir condições para personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 1dfd557b22de9888ab8d3a1f0479b45d59a86f93
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 3%

---

# Criar conteúdo condicional{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Criação de conteúdo condicional"
>abstract="Crie conteúdo condicional para definir a personalização dinâmica com base no perfil do recipient, substituindo automaticamente blocos de texto e imagens quando determinadas condições forem atendidas. Esse recurso pode levar suas campanhas a novos patamares e fornecer experiências personalizadas e altamente direcionadas ao seu público-alvo."

O conteúdo condicional é um recurso poderoso que permite criar personalização dinâmica com base no perfil do recipient, substituindo automaticamente blocos de texto e imagens quando determinadas condições são atendidas. Esse recurso pode levar suas campanhas a novos patamares e fornecer experiências personalizadas e altamente direcionadas ao seu público-alvo.

Ao configurar campos de conteúdo condicional, você pode criar personalização dinâmica avançada com base no perfil do recipient, por exemplo. Blocos de texto, links, linha de assunto e/ou imagens são substituídos no conteúdo da mensagem quando uma determinada condição é atendida. Por exemplo, você pode exibir &quot;Sr.&quot; ou &quot;Sra.&quot; de acordo com o valor do campo Gênero no banco de dados do Adobe Campaign ou incluir um link diferente com base no idioma preferencial do recipient.

## Como criar conteúdo condicional

Para criar conteúdo condicional, você precisa criar condições no editor de expressão usando uma função auxiliar específica. Esse método está disponível para todos os canais de entrega, em qualquer campo em que você possa acessar o editor de expressão, como o campo de linha de assunto ou links de email e componentes de conteúdo de texto/botão. [Saiba onde adicionar conteúdo dinâmico](gs-personalization.md/#access)

Além do editor de expressão, você pode aproveitar um construtor de conteúdo condicional dedicado ao criar um email que permite criar condições usando atributos de perfil.

## Criar condições no editor de expressão {#condition-perso-editor}

Para definir um conteúdo condicional para um delivery, siga as etapas abaixo. Neste exemplo, queremos criar conteúdo condicional com base no idioma dos recipients (francês ou inglês).

1. Abra um delivery e edite o conteúdo.

1. Localize o campo ao qual deseja adicionar conteúdo condicional e clique no **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone para abrir o editor de expressão. Neste exemplo, queremos adicionar conteúdo condicional a uma mensagem SMS:

   ![](assets/open-perso-editor-sms.png)

1. No editor de personalização, navegue até o **[!UICONTROL Funções auxiliares]** menu esquerdo.

1. Clique no ícone &quot;+&quot; ao lado da guia **Se** para iniciar sua condição. A seguinte linha é adicionada à tela central:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Substituir `<FIELD>` por um campo de personalização Por exemplo, o idioma do recipient: `recipient.language`.
   * Substituir `<VALUE>` pelo valor a satisfazer. Por exemplo, `'French'`.
   * Substituir `Ìnsert content here` pelo conteúdo que você deseja exibir para os perfis que atendem à condição especificada acima.

     ![](assets/condition-sample1.png)

1. Especifique o conteúdo que deve ser exibido se os recipients não atenderem à condição. Para fazer isso:

   1. Adicionar um **else** função auxiliar: coloque o cursor antes da tag de fechamento da expressão `%>` e clique no link `+` ao lado da **Mais** função.

      >[!NOTE]
      >
      >Cada vez que uma função auxiliar é adicionada, abrindo (`<%`) e fechamento (`%>`) são adicionadas automaticamente antes e depois da função. Exemplo após adicionar uma função auxiliar &quot;Else&quot; dentro de uma expressão:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
      >
      >Remova essas tags para evitar qualquer erro de sintaxe. Neste exemplo, a expressão corrigida após a remoção de **Mais** as tags de função são:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

   1. Substituir `Ìnsert content here` pelo conteúdo que você deseja exibir para os perfis que não atendem à condição.

      ![](assets/condition-sample2.png)

   Você também pode usar a variável **else if** função auxiliar para criar condições com várias variantes de conteúdo. Por exemplo, a expressão abaixo exibe três variantes de uma mensagem dependendo do idioma dos recipients:

   ![](assets/condition-sample3.png)

1. Quando a condição estiver pronta, você poderá salvar o conteúdo e verificar a renderização simulando o conteúdo.

## Criar conteúdo condicional em emails  {#condition-condition-builder}

O conteúdo condicional em emails pode ser criado de duas maneiras:
* No editor de expressão, criando uma condição usando funções auxiliares,
* Em um construtor de conteúdo condicional dedicado que pode ser acessado ao criar um email.

Informações detalhadas sobre como criar condições usando o editor de expressão estão disponíveis [aqui](#condition-perso-editor).

A seção abaixo guiará você pelas etapas para criar condições usando o construtor de conteúdo condicional do designer de email. Neste exemplo, criaremos uma mensagem de email com várias variantes, dependendo do idioma dos recipients. Para fazer isso, siga estes passos:

1. Crie ou abra um delivery de email, edite seu conteúdo e clique no link **[!UICONTROL Editar corpo do email]** botão para abrir o espaço de trabalho de design de email.

1. Selecione um componente de conteúdo e clique em **[!UICONTROL Ativar conteúdo condicional]**.

   ![](assets/condition-email-enable.png)

1. A variável **[!UICONTROL Conteúdo condicional]** no lado esquerdo da tela. Nesse painel, você pode criar várias variantes do componente de conteúdo selecionado usando condições.

1. Configure sua primeira variante. Para fazer isso, passe o mouse sobre **[!UICONTROL Variante - 1]** no **[!UICONTROL Conteúdo condicional]** e clique no botão **[!UICONTROL Adicionar condição]** ícone.

1. Um construtor de regras é exibido. Use os atributos de perfil para criar a condição para a primeira variante da mensagem e clique em **[!UICONTROL Confirmar o]**. Neste exemplo, estamos criando uma regra direcionada a recipients cujo idioma é &quot;francês&quot;.

   ![](assets/condition-email-rule.png)

1. A regra agora está associada à variante. Para melhorar a compreensão, recomendamos renomear a variante clicando no menu de reticências.

   Agora, configure como o componente deve ser exibido se a regra for atendida ao enviar a mensagem. Neste exemplo, queremos exibir o texto em francês se for o idioma preferencial do recipient.

   ![](assets/condition-email-variant1.png)

1. Adicione quantas variantes forem necessárias para o componente de conteúdo. Você pode alternar a qualquer momento entre as diferentes variantes para verificar como o componente de conteúdo será exibido, dependendo das regras condicionais.

   >[!NOTE]
   >Se nenhuma das regras definidas nas variantes for atendida ao enviar a mensagem, o componente de conteúdo exibirá o conteúdo definido na variável **[!UICONTROL Variante padrão]** do **[!UICONTROL Conteúdo condicional]** painel.
