---
audience: end-user
title: Agendar o envio de um delivery
description: Saiba como agendar uma entrega
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: 89633454bb3de1ac05d37d767df45d9d143c80b5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 6%

---

# Agendar o envio de um delivery {#schedule-sending}

Você pode agendar o envio de um delivery. As etapas para isso dependerão se é um delivery independente (one-shot) ou se você está trabalhando no contexto de um workflow da campanha.

## Entrega independente

Para deliveries independentes, você pode agendar diretamente a data e a hora no delivery.
Veja abaixo exemplos para cada tipo de delivery : email, sms, notificação por push.

### Email {#schedule-email-standalone}

Para agendar o envio de um delivery de email, siga as etapas abaixo:

1. Na seção **[!UICONTROL Agendamento]** das suas propriedades de entrega, ative a opção **[!UICONTROL Habilitar agendamento]**

1. Defina a data e a hora desejadas para envio e clique no botão **[!UICONTROL Revisar e enviar]**.

   ![](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>Por padrão, a opção **[!UICONTROL Ativar confirmação antes de enviar]** está habilitada. Essa opção exige que você confirme o envio antes que a entrega seja enviada na data e hora programadas. Se você precisar **enviar a entrega automaticamente** na data e hora agendadas, desabilite esta opção.
>

1. Verifique se a programação está correta e clique no botão **[!UICONTROL Preparar]**.

![](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. Quando a preparação estiver concluída, as mensagens estarão prontas para serem enviadas. As métricas principais para o delivery são exibidas: população total do target, número de mensagens a serem entregues, número de recipients excluídos. Clique no botão **[!UICONTROL Enviar como agendado]** para confirmar se você permite que o delivery seja enviado na data e hora agendadas para o público-alvo principal.

![](assets/schedule-email-standalone-send.png){zoomable="yes"}


### SMS

Para agendar sua entrega de SMS para uma data e hora específicas, as etapas são as mesmas das entregas de email, [veja acima](#schedule-email-standalone).

![](assets/schedule-sms-standalone.png){zoomable="yes"}

Você também pode verificar se a programação é levada em conta:

![](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### Notificações por push

Para agendar uma entrega por push autônoma para uma data e hora específicas, as etapas são as mesmas das entregas por email, [veja acima](#schedule-email-standalone).

![](assets/schedule-push-standalone.png){zoomable="yes"}

Você também pode verificar se a programação é levada em conta:

![](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### Entrega independente em uma campanha

Você pode criar um delivery independente em uma campanha sem usar um fluxo de trabalho. Você pode configurar a data e a hora dessa entrega conforme explicado acima.
A campanha pode ter sua programação, com uma data de início e uma data de término. Este cronograma não interferirá no seu cronograma de delivery.

![](assets/schedule-delivery-standalone.png){zoomable="yes"}

## Programar um delivery em um workflow de campanha

No contexto de um fluxo de trabalho de campanha, a **prática recomendada** é usar a atividade **[!UICONTROL Scheduler]** para aplicar uma data e hora em que o fluxo de trabalho será iniciado, envolvendo o envio da entrega. [Saiba mais sobre o Agendador](../workflows/activities/scheduler.md)

![](assets/schedule-workflow.png){zoomable="yes"}


Você precisa configurar a data e a hora na atividade **[!UICONTROL Scheduler]**.

![](assets/schedule-workflow-scheduler.png){zoomable="yes"}


>[!NOTE]
>
>Ao usar a atividade **[!UICONTROL Agendador]** para agendar o envio da sua entrega em um fluxo de trabalho, **não ative** a opção **[!UICONTROL Habilitar agendamento]** nas configurações de atividade de **[!UICONTROL Entrega]**. Seu delivery será enviado automaticamente.
>

Caso você ative a opção **[!UICONTROL Habilitar agendamento]** nas configurações de atividade de **[!UICONTROL Entrega]** e configure uma data e hora lá, a entrega aguardará para ser enviada nesta data e hora. Isso significa que, se houver um atraso entre a data de lançamento do workflow e a data de envio, o público-alvo pode não estar atualizado.
