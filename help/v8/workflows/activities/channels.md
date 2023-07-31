---
audience: end-user
title: Usar uma atividade de fluxo de trabalho de entrega
description: Saiba como adicionar uma atividade de fluxo de trabalho de entrega (Email, Push, SMS)
badge: label="Alfa"
source-git-commit: d70c671e558613a27acc5252091e1e2836b675c7
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 100%

---


# Email, SMS, push {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em canais de email, SMS e push. Você pode combinar atividades do canal na tela do fluxo de trabalho para criar fluxos de trabalho entre canais que podem iniciar ações com base no comportamento e nos dados do cliente.

Por exemplo, você pode criar uma campanha de email de boas-vindas que inclui uma série de mensagens em diferentes canais, como email, SMS e push. Também é possível enviar um email de acompanhamento depois que alguém concluir uma compra ou enviar uma mensagem de aniversário personalizada para um cliente por SMS.

Usando atividades do canal, você pode criar campanhas abrangentes e personalizadas que envolvem clientes em vários pontos de contato e impulsionam conversões.

Estas são as etapas para adicionar uma atividade do **Canal** em um fluxo de trabalho:

1. Verifique se você adicionou uma atividade **Criar público-alvo**. O público-alvo é o principal foco da sua entrega: os destinatários que receberão as mensagens Ao enviar mensagens no contexto de um fluxo de trabalho de campanha, o público-alvo da mensagem não é definido na atividade de canal, mas na atividade **Criar público-alvo**. Consulte [esta seção](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Selecione uma atividade de entrega: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificação por push (Android)]** ou **[!UICONTROL Notificação por push (iOS)]**.

1. Selecione um **Modelo** da entrega. Os modelos são configurações de entrega pré-definidas, específicas para um canal. Um modelo integrado está disponível para cada canal e é preenchido previamente por padrão. [Saiba mais](../../msg/delivery-template.md)

   ![](../assets/delivery-activity-in-wf.png)


   Você pode selecionar outro modelo no painel esquerdo de configuração das atividades do canal. Se o público-alvo selecionado anteriormente não for compatível com o canal, não será possível selecionar um modelo. Para resolver isso, atualize a atividade **Criar público-alvo** para selecionar um público-alvo com o target mapping correto. Saiba mais sobre os target mappings na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=pt-BR){target="_blank"}.

1. Clique em **Criar entrega**. Defina as configurações e o conteúdo da mensagem da mesma maneira que você cria uma entrega independente. Também é possível agendar e simular o conteúdo. [Saiba mais](../../msg/gs-messages.md).

1. Volte para o fluxo de trabalho e salve as alterações.

1. Clique em **Iniciar** para iniciar o fluxo de trabalho.

   Por padrão, iniciar um fluxo de trabalho aciona a etapa de preparação da mensagem, sem enviar imediatamente a mensagem.

1. Abra a atividade de entrega para confirmar o envio no botão **Revisar e enviar**.

1. No painel de entrega, clique em **Enviar**.

## Exemplo

Este é um exemplo de fluxo de trabalho entre canais com uma segmentação e duas entregas. O fluxo de trabalho tem como público-alvo todos os clientes que vivem em Paris e que estão interessados em máquinas de café. Entre essa população, um email é enviado aos clientes regulares e um SMS é enviado aos clientes VIP.

![](../assets/workflow-channel-example.png)
<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.
Email recipients are defined upstream of the activity in the same workflow, via an Audience targeting activity.

-->


<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
