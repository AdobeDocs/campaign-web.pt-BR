---
audience: end-user
title: Enviar uma entrega de notificação por push
description: Saiba como enviar um delivery de notificação por push com o Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---

# Visualizar e enviar uma entrega por push {#send-push-delivery}

## Pré-visualizar o delivery de notificação por push {#preview-push}

Depois de definir o conteúdo da mensagem, use assinantes de teste para pré-visualizar e testar a mensagem. Se o conteúdo personalizado estiver incluído, examine como esse conteúdo é exibido na mensagem usando os dados do perfil de teste. Isso garante que a mensagem seja renderizada corretamente e que os elementos personalizados sejam incorporados adequadamente.

As principais etapas para visualizar sua notificação por push são as seguintes. Mais detalhes sobre como visualizar entregas estão disponíveis em [esta seção](../preview-test/preview-content.md).

1. Na sua página de conteúdo de entrega, use **[!UICONTROL Simular conteúdo]** para pré-visualizar seu conteúdo personalizado.

   ![Visualização de conteúdo personalizado na página de conteúdo da entrega](assets/push_send_1.png){zoomable="yes"}

1. Clique em **[!UICONTROL Adicionar assinante(s)]** para selecionar um ou vários perfis para visualizar seus dados no conteúdo da notificação por push.

   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. No painel direito, localize uma pré-visualização da notificação por push, em que os elementos personalizados são substituídos dinamicamente por dados do perfil selecionado.

   ![Painel de visualização que mostra elementos personalizados substituídos por dados de perfil](assets/push_send_7.png){zoomable="yes"}

Revise e envie sua notificação por push para o público-alvo.

## Testar sua entrega de notificação por push {#test-push}

Usando o **Adobe Campaign**, envie provas antes de entregá-las ao seu público principal. Esta etapa valida o delivery e identifica quaisquer problemas.

Perfis de teste atuam como recipients de prova. Eles revisam e validam componentes e configurações como links, imagens e personalização, garantindo um desempenho ideal e detectando erros. Esse processo refina e otimiza as notificações por push antes de atingir o público principal. [Saiba como enviar provas](../preview-test/test-deliveries.md#subscribers).

![Testando a entrega de notificação por push com destinatários de prova](assets/push_send_6.png){zoomable="yes"}

## Enviar a entrega de notificação por push {#send-push}

1. Após personalizar o conteúdo da sua notificação por push, clique em **[!UICONTROL Revisar e enviar]** na sua página **[!UICONTROL Entrega]**.

   ![Botão Revisar e enviar na página de entrega](assets/push_send_2.png){zoomable="yes"}

1. Clique em **[!UICONTROL Preparar]** e monitore o progresso e as estatísticas fornecidas.

   Se ocorrerem erros, consulte o menu Logs para obter informações detalhadas sobre a falha.

   ![Monitorando o progresso da preparação e as estatísticas](assets/push_send_3.png){zoomable="yes"}

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para prosseguir com o processo de envio final.

1. Confirme a ação de envio clicando em **[!UICONTROL Enviar]**.

   Se a entrega por push estiver agendada, clique no botão **[!UICONTROL Enviar como agendado]**. Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![Botão Enviar como agendado para entrega por push agendada](assets/push_send_4.png){zoomable="yes"}

Depois que a entrega for enviada, rastreie os dados do KPI (Indicador Chave de Desempenho) na página de entrega e os dados no menu **[!UICONTROL Logs]**.

Comece a medir o impacto da sua mensagem com relatórios integrados. [Saiba mais](../reporting/push-report.md).