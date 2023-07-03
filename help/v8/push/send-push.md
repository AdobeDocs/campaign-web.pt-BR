---
audience: end-user
title: Enviar uma entrega de notificação por push
description: Saiba como enviar um delivery de notificação por push com o Adobe Campaign Web
badge: label="Alpha"
source-git-commit: 8bb189837a2d9c7134188e39efa47ce2ccbe12db
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 2%

---

# Visualizar e enviar uma entrega de notificação por push {#send-push-delivery}

## Pré-visualizar o delivery de notificação por push {#preview-push}

Depois de definir o conteúdo da mensagem, você pode utilizar assinantes de teste para visualizar e testar a mensagem. Se você incluiu conteúdo personalizado, poderá examinar como esse conteúdo é exibido na mensagem usando os dados do perfil de teste. Isso permite garantir que a mensagem esteja sendo renderizada corretamente e que os elementos personalizados estejam sendo incorporados adequadamente.

As principais etapas para visualizar sua notificação por push são as seguintes. Mais detalhes sobre como visualizar deliveries estão disponíveis em [nesta seção](../preview-test/preview-content.md).

1. Na página de conteúdo do delivery, use **[!UICONTROL Simular conteúdo]** para visualizar seu conteúdo personalizado.

   ![](assets/push_send_1.png)

1. Clique em **[!UICONTROL Adicionar assinante(s)]** para selecionar um ou vários perfis para visualizar seus dados no conteúdo da notificação por push.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. No painel direito, você encontrará uma pré-visualização da notificação por push, em que os elementos personalizados são substituídos dinamicamente por dados do perfil selecionado.

   ![](assets/push_send_7.png)

Agora você pode revisar e enviar a notificação por push para o público-alvo.

## Testar sua entrega de notificação por push {#test-push}

Usar **Adobe Campaign**, você terá a capacidade de testar notificações por push antes de enviá-las para o público-alvo principal. Essa etapa é importante para validar o delivery e identificar quaisquer problemas.
Os recipients de teste podem revisar elementos como links, imagens e configurações de personalização, garantindo o desempenho ideal e detectando erros. Esse processo ajuda a refinar e otimizar as notificações por push antes de atingir o público principal.

![](../assets/do-not-localize/book.png) Saiba como enviar notificações por push de teste no [nesta seção](../preview-test/test-deliveries.md#subscribers).

![](assets/push_send_6.png)

## Enviar a entrega de notificação por push {#send-push}

1. Após personalizar o conteúdo da notificação por push, clique em **[!UICONTROL Revisar e enviar]** do seu **[!UICONTROL Entrega]** página.

   ![](assets/push_send_2.png)

1. Clique em **[!UICONTROL Preparar]** acompanhamento dos progressos e das estatísticas fornecidos.

   Se ocorrer algum erro, consulte o menu Logs para obter informações detalhadas sobre a falha.

   ![](assets/push_send_3.png)

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para continuar com o processo final de envio.

1. Confirme a ação de envio clicando no ícone **[!UICONTROL Enviar]** ou **[!UICONTROL Enviar conforme agendado]** botão.

   ![](assets/push_send_4.png)

Depois que o delivery for enviado, você poderá rastrear os KPIs (indicadores principais de desempenho) na página do delivery e os dados na **[!UICONTROL Logs]** menu.

Agora você pode começar a medir o impacto de sua mensagem com relatórios integrados. [Saiba mais](../reporting/push-report.md)
