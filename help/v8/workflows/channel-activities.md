---
audience: end-user
title: Trabalhar com atividades de canal de fluxos de trabalho
description: Saiba como usar as atividades de canal nos fluxos de trabalho do Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 26%

---

# Atividades de canal {#channel}

O Adobe Campaign Web permite que você automatize e execute campanhas de marketing em vários canais, como email, SMS ou push. Com os fluxos de trabalho do Adobe Campaign, é possível combinar atividades de canal na tela para criar fluxos de trabalho entre canais que podem acionar ações com base no comportamento do cliente.

Por exemplo, você pode criar uma campanha de email de boas-vindas que inclui uma série de mensagens em diferentes canais, como email, SMS e push. Você também pode enviar um email de acompanhamento depois que um cliente concluir uma compra ou enviar uma mensagem de aniversário personalizada para um cliente por SMS.

Ao usar atividades de canal, você pode criar campanhas abrangentes e personalizadas que envolvam clientes em vários pontos de contato e gerar conversões.

As atividades de Canal estão disponíveis na paleta, no lado esquerdo da tela, na seção Canais .

## Email {#email}

descrição, que caso de uso você pode executar (comum a outras atividades que você pode vincular antes ou depois da atividade)

como adicionar e configurar a atividade

exemplo de uma atividade configurada em um fluxo de trabalho


A atividade Email delivery permite configurar o envio de um email em um workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

Os recipients do email são definidos no sentido upstream da atividade, no mesmo workflow, por meio de uma atividade de direcionamento de público-alvo.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->