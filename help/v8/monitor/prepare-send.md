---
audience: end-user
title: Preparar e enviar um email
description: Saiba como preparar e enviar um email com a interface da Web do Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 10f8768b244b0138d055330d8d23f42076c83c49
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 38%

---


# Preparar e enviar seu email {#prepare-send}

## Preparar o envio {#prepare}

Depois de definir seu [conteúdo](../email/edit-content.md), [público-alvo](../audience/add-audience.md) e [agendamento](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule), você estará pronto para preparar sua entrega de email.

Durante a preparação do delivery, a população do target é calculada e o conteúdo da mensagem é gerado para cada perfil incluído no target. Quando a preparação for concluída, as mensagens estarão prontas para serem enviadas, imediatamente ou na data e hora programadas.

As regras de validação usadas durante a preparação da entrega são descritas na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/validate/delivery-analysis.html){target="_blank"}.

As principais etapas para preparar o envio estão listadas abaixo.

1. No painel de entrega, clique em **[!UICONTROL Revisar e enviar]**.

   ![](assets/email-review-and-send.png){zoomable="yes"}


1. Clique no botão **[!UICONTROL Preparar]**, localizado no canto superior direito, e confirme.

   ![](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se você tiver agendado a entrega e desabilitado a opção **[!UICONTROL Habilitar confirmação antes de enviar]**, as etapas de preparação e envio serão agrupadas no botão **[!UICONTROL Preparar e enviar]**. [Saiba mais sobre agendamento](../msg/gs-deliveries.md#gs-schedule)

1. O progresso da preparação é exibido. Dependendo do tamanho do público-alvo, essa operação pode levar algum tempo.

   Você pode interromper a preparação a qualquer momento usando o botão **[!UICONTROL Parar preparação]**.

   ![](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >Durante a fase de preparação, nenhuma mensagem é enviada. Portanto, você pode iniciar ou parar isso sem o risco de afetar nada.

1. Quando a preparação for concluída, verifique os KPIs. Se o número de mensagens para enviar não corresponder às suas expectativas, modifique o público-alvo e reinicie a preparação.

   ![](assets/email-preparation-complete.png){zoomable="yes"}

   Estes são os diferentes KPIs exibidos:

   * **[!UICONTROL Direcionado]**: o número de destinatários direcionados.
   * **[!UICONTROL Para entregar]**: o número de mensagens que serão enviadas.
   * **[!UICONTROL A excluir]**: o número de mensagens excluídas por uma [regra de tipologia](../advanced-settings/delivery-settings.md#typology).

1. Clique no botão **[!UICONTROL Logs]** e verifique se não há erro. A última mensagem de log exibe mensagens de erro e o número de erros. [Saiba mais](delivery-logs.md)

   ![](assets/email-prepare-logs.png){zoomable="yes"}

1. Se a preparação detectar um erro crítico que impede o envio da entrega, o status da preparação aparece como falha no painel de entrega.

   ![](assets/email-prepare-error.png){zoomable="yes"}

1. Se você fizer alterações no delivery após a preparação, deverá reiniciar a preparação para que essas alterações sejam consideradas.

Quando a preparação for concluída sem erros, a mensagem estará pronta para ser enviada.

## Enviar a mensagem {#send}


Após a conclusão da [preparação](#prepare), você poderá enviar seu email.

Se a mensagem estiver programada, ela será enviada na data e hora definidas. [Saiba mais](../msg/gs-deliveries.md#gs-schedule)

### Enviar imediatamente {#send-immediately}

Para enviar um email imediatamente, siga as etapas abaixo.

1. No painel de entrega, clique no botão **[!UICONTROL Enviar]**, no canto superior direito.

   ![](assets/email-send.png){zoomable="yes"}

1. Confirme essa ação para enviar imediatamente a mensagem ao público-alvo principal.

1. O progresso do envio é exibido.

### Agendar o envio {#schedule-the-send}

Se você programou seu email para enviá-lo em data e hora posteriores, siga as etapas abaixo.

1. Antes de clicar no botão **[!UICONTROL Revisar e enviar]**, verifique se você definiu um agendamento para o seu email. [Saiba mais](../msg/gs-deliveries.md#gs-schedule)

1. No painel de entrega, clique no botão **[!UICONTROL Enviar como agendado]**, no canto superior direito.

   ![](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Clique em **[!UICONTROL Confirmar envio]**. O delivery será enviado na data agendada para o target principal.

   >[!NOTE]
   >
   >Se você desabilitou a opção **[!UICONTROL Habilitar confirmação antes de enviar]**, as etapas de preparação e envio serão agrupadas sob o botão **[!UICONTROL Preparar e enviar]**. [Saiba mais sobre agendamento](../msg/gs-deliveries.md#gs-schedule)

## Pausar ou parar o envio {#pause-stop-sending}

Se a sua entrega estiver agendada ou não<!--TBC-->, duas ações podem ser executadas a qualquer momento durante o processo de envio:

* Clique em **[!UICONTROL Pausar envio]** para interromper o envio das mensagens. Você pode retomar o envio a qualquer momento.

* Clique em **[!UICONTROL Parar envio]** para interromper imediatamente o envio. Nem a preparação nem o envio podem ser retomados depois de interrompidos.

![](assets/email-send-pause-or-stop.png){zoomable="yes"}

## Verifique os KPIs {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Entregue"
>abstract="O número de mensagens entregues com sucesso. Esse indicador é atualizado a cada 5 minutos. A porcentagem exibida se baseia no número total de mensagens enviadas."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Entenda os KPIs"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aberturas"
>abstract="O número de mensagens abertas. Esse indicador é atualizado a cada 5 minutos. A porcentagem exibida é a proporção do número de aberturas distintas em comparação com o número de mensagens entregues."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Entenda os KPIs"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Cliques"
>abstract="O número de recipients que clicaram pelo menos uma vez no email. Esse indicador é atualizado a cada 5 minutos. A porcentagem exibida é a proporção do número de cliques distintos em comparação com o número de mensagens entregues."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Entenda os KPIs"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Métricas enviadas"
>abstract="Número total de mensagens processadas durante a análise de entrega."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Entenda os KPIs"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Métricas de erros"
>abstract="Total de erros acumulados durante o processamento de entrega e retorno automático em relação ao número total de mensagens enviadas."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="Entenda os KPIs"


Quando o envio estiver concluído, você poderá verificar os KPIs exibidos:

![](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Enviado]**: o número de mensagens entregues. A porcentagem exibida tem como base o número total de mensagens a serem entregues.

* **[!UICONTROL Entregues]**: o número de mensagens entregues com sucesso. A porcentagem exibida se baseia no número total de mensagens enviadas.

* **[!UICONTROL Aberturas]**: o número de mensagens abertas. A porcentagem exibida é o número de aberturas distintas em comparação ao número de mensagens entregues.

* **[!UICONTROL Cliques]**: o número de destinatários que clicaram pelo menos uma vez no email. A porcentagem exibida é o número de cliques distintos em comparação ao número de mensagens entregues.

* **[!UICONTROL Erros]**: o número de emails com o status de erro. A porcentagem exibida se baseia no número total de mensagens enviadas.

>[!NOTE]
>
>Todos os indicadores são atualizados a cada 5 minutos após o início da entrega. Os indicadores de preparação do delivery são em tempo real.

Saiba mais sobre KPIs em [esta página](../reporting/kpis.md).

Você também pode verificar os logs. [Saiba mais](delivery-logs.md)