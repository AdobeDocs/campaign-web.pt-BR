---
audience: end-user
title: Enriquecimento de perfil em mensagens transacionais
description: Saiba como criar uma mensagem transacional na interface da Web do Campaign
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 11%

---


# Enriquecer mensagens transacionais com dados de perfil{#profile-enrichment}

Esse recurso permite personalizar mensagens transacionais vinculando campos do banco de dados do Adobe Campaign ao conteúdo da mensagem. Você pode selecionar target mappings, colunas de enriquecimento e uma chave de reconciliação para garantir uma personalização em tempo real e precisa, mantendo os limites de desempenho.

* As mensagens transacionais baseadas em evento usam dados contidos no próprio evento.
* As mensagens transacionais baseadas em perfil usam dados contidos no banco de dados do Adobe Campaign.

Para configurar o enriquecimento de perfil, siga estas etapas principais:

1. Criar a mensagem transacional, [leia mais](#create-enrichment)
1. Definir o tipo de evento, [leia mais](#event-enrichment)
1. Defina as configurações de enriquecimento, [leia mais](#settings-enrichment)
1. Defina o conteúdo, [leia mais](#content-enrichment)
1. Validar e enviar, [leia mais](#send-enrichment)

>[!NOTE]
>
>Seu servidor deve ser atualizado para a versão 8.8.2 ou posterior.
>
>No momento, esse recurso só está disponível para emails, SMS e notificações por push.

## Criar a mensagem transacional{#create-enrichment}

Primeiro, é necessário criar uma nova mensagem transacional.

1. Na seção **[!UICONTROL Mensagens acionadas]**, vá para **[!UICONTROL Mensagens transacionais]** e crie uma nova mensagem transacional.

   ![](assets/transactional-browse.png){zoomable="yes"}

1. Escolha um modelo e defina as propriedades. Para obter mais informações, consulte esta [página](create-transactional.md#transactional-message).

## Definir o tipo de evento{#event-enrichment}

Em seguida, é necessário definir o evento como baseado em perfil para direcionar dados contidos no banco de dados do Adobe Campaign.

1. Na seção **Tipo de evento**, selecione **Selecionar tipo de evento** e escolha se deseja usar um tipo de evento existente ou criar o seu próprio.

   >[!NOTE]
   >
   >Não é possível escolher um tipo de evento já usado em outro modelo de mensagem transacional.

   ![](assets/profile-enrich.png){zoomable="yes"}

1. Insira as informações do tipo de evento:

   * Para um tipo de evento existente, selecione na lista.
   * Para um novo, adicione um rótulo e um nome.

1. Em seguida, escolha **Perfil RT** no menu suspenso **Tipo de evento**.

   ![](assets/profile-enrich1.png){zoomable="yes"}

## Definir as configurações de enriquecimento{#settings-enrichment}

Agora, vamos adicionar campos ao evento que permitirão personalizar a mensagem transacional.

1. Na seção **Data**, clique em **Enrichment settings**.

   ![](assets/profile-enrich2.png){zoomable="yes"}

   >[!NOTE]
   >
   >Esse botão está disponível somente quando você define um evento baseado em perfil.

1. Na seção **Atributos adicionais**, clique em **adicionar atributo** e selecione os campos necessários.

   ![](assets/profile-enrich3.png){zoomable="yes"}

1. Defina qual atributo será usado como chave de reconciliação.

1. Escolha o que deve acontecer se a chave não estiver disponível na carga.

   * A mensagem é enviada sem personalização
   * Mensagem não enviada

## Definição do conteúdo{#content-enrichment}

Em seguida, é necessário definir o conteúdo da mensagem transacional.

1. Na seção **Conteúdo**, clique no botão **Editar conteúdo** e defina o conteúdo da mensagem. Consulte esta [página](create-transactional.md#transactional-content).

   ![](assets/template-content.png){zoomable="yes"}

1. Ao usar a personalização, na linha de assunto, por exemplo, use o menu **Enriquecimento de perfil** para adicionar os campos baseados em perfil definidos anteriormente.

   ![](assets/profile-enrich4.png){zoomable="yes"}


## Validar e enviar{#send-enrichment}

Por fim, você precisa validar e enviar o delivery.

1. Valide o delivery simulando o conteúdo e enviando provas. Consulte esta [página](validate-transactional.md).

1. Clique no botão **[!UICONTROL Revisar e publicar]** para criar e publicar a mensagem. Os acionadores agora podem iniciar o envio da mensagem transacional.


<!--
When creating the event configuration, select the Profile event targeting dimension (see Creating an event).

Add fields to the event, in order to be able to personalize the transactional message (see Defining the event attributes). You must add at least one field to create an enrichment. You do not need to create other fields such as First name and Last name as you will be able to use personalization fields from the Adobe Campaign database.

Create an enrichment in order to link the event to the Profile resource (see Enriching the event) and select this enrichment as the Targeting enrichment.


IMPORTANT
This step is mandatory for profile-based events.
Preview and publish the event (see Previewing and publishing the event).

When previewing the event, the REST API does not contain an attribute specifying the email address, mobile phone, or push notification specific attributes, as it will be retrieved from the Profile resource.

Once the event has been published, a transactional message linked to the new event is automatically created. In order for the event to trigger sending a transactional message, you must modify and publish the message that was just created…

Integrate the event into your website (see Integrate the event triggering).
-->

