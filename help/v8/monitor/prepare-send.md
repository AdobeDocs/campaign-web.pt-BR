---
audience: end-user
title: Preparar e enviar um email
description: Saiba como preparar e enviar um email com a interface do usuário da Web do Campaign
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 9%

---


# Preparar e enviar seu email {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Preparar e enviar seu email"
>abstract="Veja como preparar seu email e saiba mais sobre KPIs de envio."

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

Após definir seu conteúdo, público-alvo e programação, você estará pronto para preparar sua mensagem. Durante a preparação, a população do target é calculada e o conteúdo da mensagem gerado para cada perfil é incluído no target. Quando a preparação for concluída, as mensagens estarão prontas para serem enviadas, imediatamente ou na data e hora programadas. As regras de validação usadas durante a análise são descritas na seção [Documentação do Campaign Classic v7](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies){target="_blank"}.

Siga as etapas abaixo:

1. No painel do delivery, clique em **Preparar** no canto superior direito e confirme.

   ![](assets/prepare.png)

   O progresso da preparação é exibido. Dependendo do tamanho do público alvo, essa operação pode levar algum tempo.

   >[!NOTE]
   >
   >Você pode interromper a preparação a qualquer momento usando a variável **Parar preparação** botão. Durante a fase de preparação, nenhuma mensagem é enviada. Portanto, você pode iniciar ou parar isso sem correr o risco de afetar nada.

1. Quando a preparação for concluída, verifique os KPIs. Se o número de mensagens para enviar não corresponder às suas expectativas, modifique seu público-alvo e reinicie a preparação.

   ![](assets/prepare2.png)

   Estes são os diferentes KPIs exibidos:

   * **Direcionado**: o número de recipients alvos
   * **Para entregar**: o número de mensagens que serão enviadas
   * **Para excluir**: o número de mensagens excluídas por uma regra de tipologia

1. Clique no botão **Logs** e verifique se não há erro. A última mensagem de log exibe mensagens de erro e o número de erros. Para obter mais informações, consulte esta [seção](delivery-logs.md).

   ![](assets/prepare-logs.png)

Se a preparação detectar um erro crítico que impede o envio do delivery, o status da preparação aparecerá como defeituoso no painel do delivery.

![](assets/prepare-error.png)

Se precisar fazer alterações no delivery após a preparação, será necessário reiniciar a preparação para que essas alterações sejam consideradas.

Quando a preparação estiver concluída sem erro, sua mensagem estará pronta para ser enviada. Para obter mais informações, consulte esta [seção](#send).

## Enviar a mensagem{#send}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Entregue"
>abstract="O número de mensagens entregues com êxito. Este indicador é atualizado a cada 5 minutos. A porcentagem exibida se baseia no número total de mensagens enviadas."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Aberturas"
>abstract="O número de mensagens abertas. Este indicador é atualizado a cada 5 minutos. A porcentagem exibida é a proporção do número de aberturas distintas em comparação ao número de mensagens entregues."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Cliques"
>abstract="O número de recipients que clicaram pelo menos uma vez no email. Este indicador é atualizado a cada 5 minutos. A porcentagem exibida é a proporção do número de cliques distintos em comparação ao número de mensagens entregues."


Depois que a preparação for concluída, você poderá enviar a mensagem. Essa etapa só é necessária para mensagens enviadas imediatamente. Se a mensagem estiver programada, ela será enviada na data definida.

Siga estas etapas:

1. No painel do delivery, clique em **Enviar** no canto superior direito e confirme.

   ![](assets/send.png)

1. O progresso do envio é exibido. Verifique os KPIs exibidos. Você também pode verificar os logs. Para obter mais informações, consulte esta [seção](delivery-logs.md).

   ![](assets/send2.png)

   Estes são os diferentes KPIs exibidos:

   * **Entregue**: o número de mensagens entregues com êxito. A porcentagem exibida se baseia no número total de mensagens enviadas.
   * **Abre**: o número de mensagens abertas. A porcentagem exibida é a proporção do número de aberturas distintas em comparação ao número de mensagens entregues.
   * **Cliques**: o número de recipients que clicaram pelo menos uma vez no email. A porcentagem exibida é a proporção do número de cliques distintos em comparação ao número de mensagens entregues.

   >[!NOTE]
   >
   >Todos os indicadores são atualizados a cada 5 minutos após o início do delivery. Os indicadores de preparação do delivery são em tempo real.

   Você pode pausar o envio a qualquer momento e, em seguida, retomar. Se você interromper o delivery enquanto ele estiver sendo enviado, não será possível retomar.
