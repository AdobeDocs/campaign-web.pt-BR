---
audience: end-user
title: Agendar o envio de um delivery
description: Saiba como agendar uma entrega
source-git-commit: 7bee82ea7286fca3398bef9f84f3c5aa1e3d9959
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

1. No **[!UICONTROL Agendar]** das suas propriedades de delivery, ative a variável **[!UICONTROL Ativar agendamento]** alternar

1. Defina a data e a hora desejadas para envio e clique em **[!UICONTROL Revisar e enviar]** botão.

   ![](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>Por padrão, a opção **[!UICONTROL Ativar confirmação antes de enviar]** está habilitada. Essa opção exige que você confirme o envio antes que a entrega seja enviada na data e hora programadas. Se você precisar **enviar o delivery automaticamente** na data e hora programadas, é necessário desativar essa opção.
>

1. Verifique se a programação está correta e clique em **[!UICONTROL Preparar]** botão.

![](assets/schedule-email-standalone-prepare.png){zoomable="yes"}

1. Quando a preparação estiver concluída, as mensagens estarão prontas para serem enviadas. As métricas principais para o delivery são exibidas: população total do target, número de mensagens a serem entregues, número de recipients excluídos. Clique em **[!UICONTROL Enviar conforme agendado]** botão para confirmar que você permite que o delivery seja enviado na data e hora agendadas para o target principal.

![](assets/schedule-email-standalone-send.png){zoomable="yes"}


### SMS

Para agendar o delivery de SMS para uma data e hora específicas, as etapas são as mesmas dos deliveries de email, [veja acima](#schedule-email-standalone).

![](assets/schedule-sms-standalone.png){zoomable="yes"}

Você também pode verificar se a programação é levada em conta:

![](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### Notificações por push

Para agendar um delivery por push independente para uma data e hora específicas, as etapas são as mesmas dos deliveries de email, [veja acima](#schedule-email-standalone).

![](assets/schedule-push-standalone.png){zoomable="yes"}

Você também pode verificar se a programação é levada em conta:

![](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### Entrega independente em uma campanha

Você pode criar um delivery independente em uma campanha sem usar um fluxo de trabalho. Você pode configurar a data e a hora dessa entrega conforme explicado acima.
A campanha pode ter sua programação, com uma data de início e uma data de término. Este cronograma não interferirá no seu cronograma de delivery.

![](assets/schedule-delivery-standalone.png){zoomable="yes"}

## Programar um delivery em um workflow de campanha

No contexto de um workflow de campanha, a variável **prática recomendada** é usar o **[!UICONTROL Scheduler]** atividade para aplicar uma data e hora que iniciará o workflow, envolvendo o envio do delivery. [Saiba mais sobre o Scheduler](../workflows/activities/scheduler.md)

![](assets/schedule-workflow.png){zoomable="yes"}


É necessário configurar a data e a hora no campo **[!UICONTROL Scheduler]** atividade.

![](assets/schedule-workflow-scheduler.png){zoomable="yes"}


>[!NOTE]
>
>Quando você usa o **[!UICONTROL Scheduler]** atividade para agendar o envio do delivery em um workflow, **não ativar** o **[!UICONTROL Ativar agendamento]** alternar no **[!UICONTROL Entrega]** configurações de atividade. Seu delivery será enviado automaticamente.
>

Caso ative a opção **[!UICONTROL Ativar agendamento]** alternar no **[!UICONTROL Entrega]** configurações de atividade e definir uma data e hora, o delivery aguardará para ser enviado nessa data e hora. Isso significa que, se houver um atraso entre a data de lançamento do workflow e a data de envio, o público-alvo pode não estar atualizado.

