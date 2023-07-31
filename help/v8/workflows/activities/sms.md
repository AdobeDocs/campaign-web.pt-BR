---
audience: end-user
title: Usar a atividade de workflow de SMS
description: Saiba como usar a atividade de workflow de SMS
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 3%

---


# SMS {#sms}

A variável **SMS** A atividade fornece a funcionalidade para enviar mensagens SMS em um workflow. Ela permite a automação do envio de SMS para um target específico determinado no mesmo workflow.

Para definir os recipients do SMS, você pode configurá-los antes da atividade de delivery do SMS no workflow usando a atividade Build audience. Saiba mais.

1. Depois de criar e configurar um novo fluxo de trabalho, adicione uma atividade Criar público-alvo para selecionar um público-alvo existente ou use o construtor de regras para definir sua própria consulta.

1. Adicione uma atividade de canal SMS no seu fluxo de trabalho.

   ![](../assets/activity-sms-1.png)
<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the SMS to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the SMS to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the SMS to be sent at regular intervals.
-->

1. Selecione a atividade. No menu do delivery, selecione os Templates que deseja usar para esse delivery. Saiba mais sobre templates

1. Clique em Criar entrega para configurar a entrega de SMS. Para obter mais informações sobre delivery de SMS, consulte esta página.

1. Quando o delivery estiver pronto para ser enviado, navegue de volta para o workflow e clique em Start para iniciar o workflow.

1. Por padrão, iniciar um workflow de delivery aciona o estágio de preparação da mensagem, sem enviar imediatamente a mensagem.

   Clique em Revisar e enviar no menu avançado da atividade de SMS para confirmar o envio.

1. No painel do delivery de SMS, clique em Send.
