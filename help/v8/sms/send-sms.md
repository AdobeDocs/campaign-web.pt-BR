---
audience: end-user
title: Enviar uma entrega de SMS
description: Saiba como enviar SMS com o Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 14%

---

# Visualizar e enviar uma entrega de SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nova métrica de quarentenas"
>abstract="Número total de endereços colocados em quarentena após falha em uma entrega (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues."

## Pré-visualizar seu delivery de SMS{#preview-sms}

Depois de definir o conteúdo da mensagem, você pode utilizar perfis de teste para pré-visualizá-la e testá-la. Se você incluiu conteúdo personalizado, poderá examinar como esse conteúdo é exibido na mensagem usando os dados do perfil de teste. Isso permite garantir que a mensagem apareça conforme esperado e que qualquer informação personalizada seja apresentada corretamente.

As principais etapas para visualizar seu delivery de SMS são as seguintes. Mais detalhes sobre como visualizar entregas estão disponíveis em [esta seção](../preview-test/preview-content.md).

1. Na sua página de conteúdo de entrega, use **[!UICONTROL Simular conteúdo]** para pré-visualizar seu conteúdo personalizado.

   ![](assets/sms_send_1.png){zoomable="yes"}

1. Clique em **[!UICONTROL Adicionar perfil(s) de teste]** para selecionar um ou vários perfis de teste ou perfis.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png){zoomable="yes"}
    -->

1. No painel direito, você encontrará uma pré-visualização do delivery de SMS, em que os elementos personalizados são substituídos dinamicamente pelos dados do perfil selecionado.

   ![](assets/sms_send_3.png){zoomable="yes"}

Agora é possível revisar e enviar uma mensagem de SMS para o público-alvo.

## Testar sua entrega de SMS {#test-sms}

Com o **Adobe Campaign**, você pode testar uma mensagem antes de enviá-la para o público principal, o que é uma etapa essencial para validar sua campanha de email e identificar possíveis problemas.

O envio de provas é uma etapa importante para garantir a qualidade e a eficácia do delivery. Os recipients de prova podem revisar vários elementos, como links, links para opção de não participação e imagens, bem como identificar erros na renderização, conteúdo, configurações de personalização e configuração de SMS. Esse processo ajuda a avaliar e otimizar completamente o SMS antes de alcançar seu público principal.

![](../assets/do-not-localize/book.png) Saiba como enviar provas em [esta seção](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png){zoomable="yes"}

## Enviar a entrega de SMS {#send-sms}

1. Depois de personalizar seu conteúdo de SMS, clique em **[!UICONTROL Revisar e enviar]** na sua página **[!UICONTROL Entrega]**.

   ![](assets/sms_send_4.png){zoomable="yes"}

1. Clique em **[!UICONTROL Preparar]** e monitore o progresso e as estatísticas fornecidas.

   Se ocorrer algum erro, consulte o menu Logs para obter informações detalhadas sobre a falha.

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para prosseguir com o processo de envio final.

   ![](assets/sms_send_5.png){zoomable="yes"}

   Se a entrega de SMS tiver sido agendada, clique no botão **[!UICONTROL Enviar como agendado]**. Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-messages.md#schedule-the-delivery-sending).


1. Confirme a ação de envio clicando no botão **[!UICONTROL Enviar]**.

Depois que a entrega for enviada, você poderá acompanhar seus KPIs (indicadores principais de desempenho) por meio da página de entrega e dados pelo menu **[!UICONTROL Logs]**.

Agora você pode começar a medir o impacto de sua mensagem com relatórios integrados. [Saiba mais](../reporting/sms-report.md)
