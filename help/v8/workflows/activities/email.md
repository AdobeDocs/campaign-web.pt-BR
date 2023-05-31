---
audience: end-user
title: Usar a atividade de fluxo de trabalho Email
description: Saiba como usar a atividade de workflow de email
badge: label="Alpha" type="Positive"
source-git-commit: 6af0b460a3c81f063a855b2fabba221b43e4ebb9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Email {#email}

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow

-->


A atividade Email delivery permite configurar o envio de um email em um workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Os destinatários de email são definidos no sentido upstream da atividade, no mesmo fluxo de trabalho, por meio de uma atividade de direcionamento de Público-alvo.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
