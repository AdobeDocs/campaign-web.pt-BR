---
audience: end-user
title: Usar a atividade de workflow de notificação por push
description: Saiba como usar a atividade de workflow de notificação por push
badge: label="Alpha" type="Positive"
source-git-commit: c0e5902d3ee504aa5aa4e55f18416facfe4020b1
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 3%

---


# Notificações por push {#push-activity}

A variável **Notificação por push** a atividade de delivery permite configurar o envio de uma notificação por push em um workflow.

>[!BEGINTABS]

>[!TAB Notificação por push (Android)]

1. Depois de criar e configurar um novo fluxo de trabalho, adicione uma atividade Criar público-alvo para selecionar um público-alvo existente ou use o construtor de regras para definir sua própria consulta.

1. Adicione uma atividade de canal de notificação por push (Android) no fluxo de trabalho.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Selecione a atividade. No menu do delivery, selecione os Templates que deseja usar para esse delivery. Saiba mais sobre modelos

1. Clique em Criar entrega para configurar a entrega de notificação por push. Para obter mais informações sobre delivery de notificação por push (Android), consulte esta página.

1. Quando o delivery estiver pronto para ser enviado, navegue de volta para o workflow e clique em Start para iniciar o workflow.

1. Por padrão, iniciar um workflow de delivery aciona o estágio de preparação da mensagem, sem enviar imediatamente a mensagem.

   Clique em Revisar e enviar no menu avançado da atividade de canal de notificação por push (Android) para confirmar o envio.

1. No painel do delivery de notificação por push, clique em Enviar.

>[!TAB Notificação por push (iOS)]

1. Depois de criar e configurar um novo fluxo de trabalho, adicione uma atividade Criar público-alvo para selecionar um público-alvo existente ou use o construtor de regras para definir sua própria consulta.

1. Adicione uma atividade de canal de notificação por push (iOS) no fluxo de trabalho.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Selecione a atividade. No menu do delivery, selecione os Templates que deseja usar para esse delivery. Saiba mais sobre modelos

1. Clique em Criar entrega para configurar a entrega de notificação por push. Para obter mais informações sobre delivery de notificação por push (iOS), consulte esta página.

1. Quando o delivery estiver pronto para ser enviado, navegue de volta para o workflow e clique em Start para iniciar o workflow.

1. Por padrão, iniciar um workflow de delivery aciona o estágio de preparação da mensagem, sem enviar imediatamente a mensagem.

   Clique em Revisar e enviar no menu avançado da atividade de canal de notificação por push (iOS) para confirmar o envio.

1. No painel do delivery de notificação por push, clique em Enviar.

>[!ENDTABS]