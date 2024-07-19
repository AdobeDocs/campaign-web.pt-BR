---
audience: end-user
title: Enviar uma entrega de notificação por push
description: Saiba como enviar um delivery de notificação por push com o Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 2%

---

# Visualizar e enviar uma entrega por push {#send-push-delivery}

## Pré-visualizar o delivery de notificação por push {#preview-push}

Depois de definir o conteúdo da mensagem, você pode utilizar assinantes de teste para visualizar e testar a mensagem. Se você incluiu conteúdo personalizado, poderá examinar como esse conteúdo é exibido na mensagem usando os dados do perfil de teste. Isso permite garantir que a mensagem esteja sendo renderizada corretamente e que os elementos personalizados estejam sendo incorporados adequadamente.

As principais etapas para visualizar sua notificação por push são as seguintes. Mais detalhes sobre como visualizar entregas estão disponíveis em [esta seção](../preview-test/preview-content.md).

1. Na sua página de conteúdo de entrega, use **[!UICONTROL Simular conteúdo]** para pré-visualizar seu conteúdo personalizado.

   ![](assets/push_send_1.png){zoomable="yes"}

1. Clique em **[!UICONTROL Adicionar assinante(s)]** para selecionar um ou vários perfis para visualizar seus dados no conteúdo da notificação por push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. No painel direito, você encontrará uma pré-visualização da notificação por push, em que os elementos personalizados são substituídos dinamicamente por dados do perfil selecionado.

   ![](assets/push_send_7.png){zoomable="yes"}

Agora você pode revisar e enviar a notificação por push para o público-alvo.

## Testar sua entrega de notificação por push {#test-push}

Usando o **Adobe Campaign**, você pode enviar provas antes de enviá-las para o seu público principal. Essa etapa é importante para validar o delivery e identificar quaisquer problemas.

Os perfis de teste são os recipients de prova. Eles podem revisar e validar componentes e configurações como links, imagens e personalização, garantindo um desempenho ideal e detectando erros. Esse processo ajuda a refinar e otimizar as notificações por push antes de atingir o público principal. [Saiba como enviar provas](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable="yes"}

## Enviar a entrega de notificação por push {#send-push}

1. Após personalizar o conteúdo da sua notificação por push, clique em **[!UICONTROL Revisar e enviar]** na sua página **[!UICONTROL Entrega]**.

   ![](assets/push_send_2.png){zoomable="yes"}

1. Clique em **[!UICONTROL Preparar]** e monitore o progresso e as estatísticas fornecidas.

   Se ocorrer algum erro, consulte o menu Logs para obter informações detalhadas sobre a falha.

   ![](assets/push_send_3.png){zoomable="yes"}

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para prosseguir com o processo de envio final.

1. Confirme a ação de envio clicando em **[!UICONTROL Enviar]**.

   Se a entrega por push tiver sido agendada, clique no botão **[!UICONTROL Enviar como agendado]**. Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png){zoomable="yes"}

Depois que a entrega for enviada, você poderá acompanhar seus KPIs (indicadores principais de desempenho) por meio da página de entrega e dados pelo menu **[!UICONTROL Logs]**.

Agora você pode começar a medir o impacto de sua mensagem com relatórios integrados. [Saiba mais](../reporting/push-report.md)
