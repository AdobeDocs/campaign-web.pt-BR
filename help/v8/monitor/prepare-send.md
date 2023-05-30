---
audience: end-user
title: Preparar e enviar um email
description: Saiba como preparar e enviar um email com a interface do Campaign Web
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Alpha" type="Positive"
source-git-commit: 598caf335db5b46036c8b6da92f4a9591089a0f4
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 100%

---


# Preparar e enviar seu email {#prepare-send}


<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Preparar o envio{#prepare}

Após definir o conteúdo, público e programação, você estará pronto para preparar sua mensagem. Durante a preparação, a população do público-alvo é calculada, e o conteúdo da mensagem gerado para cada perfil é incluído no público-alvo. Quando a preparação for concluída, as mensagens estarão prontas para serem enviadas, imediatamente ou na data e hora programadas. As regras de validação usadas durante a análise são descritas na seção [Documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=pt-BR#validation-process-with-typologies){target="_blank"}.

Siga as etapas abaixo:

1. No painel de entrega, clique no botão **Preparar** localizado no canto superior direito e confirme.

   ![](assets/prepare.png)

   O progresso da preparação é exibido. Dependendo do tamanho do público-alvo, essa operação pode levar algum tempo.

   >[!NOTE]
   >
   >Você pode interromper a preparação a qualquer momento usando o botão **Parar preparação**. Durante a fase de preparação, nenhuma mensagem é enviada. Portanto, você pode iniciar ou parar isso sem o risco de afetar nada.

1. Quando a preparação for concluída, verifique os KPIs. Se o número de mensagens para enviar não corresponder às suas expectativas, modifique o público e reinicie a preparação.

   ![](assets/prepare2.png)

   Estes são os diferentes KPIs exibidos:

   * **Direcionado**: o número de recipients visados
   * **Para entregar**: o número de mensagens que serão enviadas
   * **Para excluir**: o número de mensagens excluídas por uma regra de tipologia

1. Clique no botão **Logs** e verifique se não há erro. A última mensagem de log exibe mensagens de erro e o número de erros. Para obter mais informações, consulte esta [seção](delivery-logs.md).

   ![](assets/prepare-logs.png)

Se a preparação detectar um erro crítico que impede o envio da entrega, o status da preparação aparece como falha no painel de entrega.

![](assets/prepare-error.png)

Se precisar fazer alterações na entrega após a preparação, será necessário reiniciar a preparação para que essas alterações sejam consideradas.

Assim que a preparação estiver concluída sem erros, sua mensagem estará pronta para ser enviada. Para obter mais informações, consulte esta [seção](#send).

## Enviar a mensagem{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Entregue"
>abstract="O número de mensagens entregues com sucesso. Esse indicador é atualizado a cada 5 minutos. A porcentagem exibida se baseia no número total de mensagens enviadas."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aberturas"
>abstract="O número de mensagens abertas. Esse indicador é atualizado a cada 5 minutos. A porcentagem exibida é a proporção do número de aberturas distintas em comparação com o número de mensagens entregues."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Cliques"
>abstract="O número de recipients que clicaram pelo menos uma vez no email. Esse indicador é atualizado a cada 5 minutos. A porcentagem exibida é a proporção do número de cliques distintos em comparação com o número de mensagens entregues."


Depois que a preparação for concluída, você poderá enviar a mensagem. Essa etapa é necessária apenas para mensagens enviadas imediatamente. Se a mensagem estiver programada, ela será enviada na data definida.

Siga estas etapas:

1. No painel de entrega, clique no botão **Enviar** no canto superior direito e confirme.

   ![](assets/send.png)

1. O progresso do envio é exibido. Verifique os KPIs exibidos. Você também pode verificar os logs. Para obter mais informações, consulte esta [seção](delivery-logs.md).

   ![](assets/send2.png)

   Estes são os diferentes KPIs exibidos:

   * **Entregues**: o número de mensagens entregues com sucesso. A porcentagem exibida se baseia no número total de mensagens enviadas.
   * **Aberturas**: o número de mensagens abertas. A porcentagem exibida é a proporção do número de aberturas distintas em comparação com o número de mensagens entregues.
   * **Cliques**: o número de recipients que clicaram pelo menos uma vez no email. A porcentagem exibida é a proporção do número de cliques distintos em comparação com o número de mensagens entregues.

   >[!NOTE]
   >
   >Todos os indicadores são atualizados a cada 5 minutos após o início da entrega. Os indicadores de preparação da entrega estão em tempo real.

   Você pode pausar o envio a qualquer momento e, em seguida, retomar. Se você interromper a entrega enquanto estiver sendo enviada, não será possível retomar.
