---
audience: end-user
title: Preparar e enviar um email
description: Documentação da Web do Campaign v8
source-git-commit: fe06419e429f48dbcc71802c372130be22e68d52
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 13%

---

# Preparar e enviar seu email {#prepare-send}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Preparar e enviar seu email"
>abstract="Saiba como preparar seu email e saber mais sobre como enviar KPIs."

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## Preparar o envio

Durante a preparação, a população do target é calculada e o conteúdo da mensagem gerado para cada perfil é incluído no target. Quando a preparação for concluída, as mensagens estarão prontas para serem enviadas, imediatamente ou na data e hora programadas. As regras de validação usadas durante a análise são descritas nesta [seção](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html?lang=en#validation-process-with-typologies).

1. Clique no botão **Preparar** no canto superior direito.

1. O progresso da preparação é exibido. Dependendo do tamanho do público alvo, essa operação pode levar algum tempo.

   >[!NOTE]
   >
   >Você pode interromper a preparação a qualquer momento usando a variável **Parar preparação** botão. Durante a fase de preparação, nenhuma mensagem é enviada. Portanto, você pode iniciar ou parar isso sem correr o risco de afetar nada.

1. Quando a preparação for concluída, verifique a **Direcionado**, **Para entregar** e **Para excluir** KPIs. Se o número de mensagens para enviar não corresponder às suas expectativas, modifique seu público-alvo e reinicie a preparação.

1. Clique no botão **Logs** e verifique se não há erro. Todas as etapas de validação, avisos e erros são listados. Os ícones coloridos mostram o tipo de mensagem:

   * O ícone cinza indica uma mensagem informativa.
   * O ícone amarelo indica um erro de processamento não crítico.
   * O ícone vermelho indica um erro crítico que impede o envio do delivery.

1. Depois de fazer as alterações, reinicie a preparação.

Uma vez concluída a preparação, sua mensagem estará pronta para ser enviada. Para obter mais informações, consulte Confirmação do envio.


## Enviar a mensagem

Quando a preparação estiver concluída, siga as etapas abaixo para enviar sua mensagem.

1. Clique no botão **Botão Enviar** no canto superior direito e confirme.

1. O progresso do envio é exibido junto com três KPIs: Entregue, Aberturas, Cliques.

1. Finalize o envio clicando no botão OK .

LOGS

>[!NOTE]
>
>Se a mensagem estiver programada, ela será enviada quando o horário de envio for atingido. Para saber mais sobre como programar mensagens, consulte esta seção.

