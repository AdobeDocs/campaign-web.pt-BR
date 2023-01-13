---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do usuário da Web do Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 2d23b04b81ab625de0936fdf058f6ac8bd1017c3
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# Personalizar seu conteúdo{#add-personalization}

![](../assets/do-not-localize/badge.png)

Você pode personalizar o conteúdo da mensagem ao:

* Inserção dinâmica **campos de personalização**

   Os campos de personalização são usados para personalização de primeiro nível das mensagens. Você pode selecionar qualquer campo disponível no banco de dados no editor de personalização. Para um delivery, é possível selecionar qualquer campo relacionado ao recipient, à mensagem ou ao delivery. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo de suas mensagens.

   ![](assets/perso-subject-line.png)

   A sintaxe acima insere a cidade do recipient no conteúdo: &lt;%= recipient.location.city %>.

* Inserção de predefinido **blocos de conteúdo**

   O Campaign vem com um conjunto de blocos de personalização que contêm uma renderização específica que você pode inserir nos deliveries. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para a mirror page da mensagem. Os blocos de conteúdo estão disponíveis em uma entrada dedicada no editor de personalização.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personalizar a linha de assunto do email {#personalize-subject-line}

Para adicionar personalização na **[!UICONTROL Linha de assunto]** siga as etapas abaixo:

1. Clique no botão **Abrir caixa de diálogo de personalização** ícone à direita do **Linha de assunto** campo.
1. Insira o conteúdo da linha de assunto e selecione os atributos de personalização a serem adicionados.
1. Clique em Confirm para validar. Os atributos de personalização são adicionados à linha de assunto.

![](assets/perso-subject.png)

## Personalizar seu conteúdo de email {#personalize-emails}

Para personalizar o conteúdo do email, abra a mensagem no Designer de email e:

1. Clique dentro de um bloco de texto.
1. Na barra de ferramentas contextual, selecione **Adicionar personalização**.

   ![](assets/perso-add-to-content.png)

1. Insira o nome do recipient no editor de personalização e confirme.

   ![](assets/perso-add-name.png)

   O atributo de personalização é adicionado ao conteúdo do email.

   Você pode simular o conteúdo para verificar a renderização. [Saiba mais](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)


## Personalizar links em seus emails {#personalize-links}

Para personalizar um **link**:

1. Selecione um bloco de texto ou uma imagem.
1. Na barra de ferramentas contextual, selecione **Adicionar personalização**.

   ![](assets/perso-link.png)

1. Use o editor de personalização para definir e personalizar o link.

## Personalize suas ofertas {#personalize-offers}

Também é possível acessar o editor de personalização ao adicionar conteúdo do tipo texto às representações das ofertas.
