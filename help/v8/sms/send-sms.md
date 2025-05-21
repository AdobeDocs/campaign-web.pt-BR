---
audience: end-user
title: Enviar uma entrega de SMS
description: Saiba como enviar SMS com o Adobe Campaign Web
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 12%

---

# Visualizar e enviar uma entrega de SMS {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nova métrica de quarentenas"
>abstract="Número total de endereços colocados em quarentena após falha em uma entrega (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues."

## Pré-visualizar seu delivery de SMS {#preview-sms}

Depois de definir o conteúdo da mensagem, use perfis de teste para pré-visualizá-la e testá-la. Se o conteúdo personalizado estiver incluído, examine como esse conteúdo aparece na mensagem usando os dados do perfil de teste. Isso garante que a mensagem seja exibida conforme o esperado e que as informações personalizadas sejam apresentadas corretamente.

As principais etapas para visualizar seu delivery de SMS são as seguintes. Mais detalhes sobre como visualizar entregas estão disponíveis em [esta seção](../preview-test/preview-content.md).

1. Na sua página de conteúdo de entrega, use **[!UICONTROL Simular conteúdo]** para pré-visualizar seu conteúdo personalizado.

   ![Pré-visualização de conteúdo de SMS personalizado](assets/sms_send_1.png){zoomable="yes"}

1. Clique em **[!UICONTROL Adicionar perfil(s) de teste]** para selecionar um ou vários perfis de teste ou perfis.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![Selecting test profiles for SMS preview](assets/sms_send_2.png){zoomable="yes"}
    -->

1. No painel direito, visualize uma pré-visualização do delivery de SMS, em que os elementos personalizados são substituídos dinamicamente por dados do perfil selecionado.

   ![Painel de visualização mostrando a entrega personalizada de SMS](assets/sms_send_3.png){zoomable="yes"}

Revise e envie sua mensagem SMS para o público-alvo.

## Testar sua entrega de SMS {#test-sms}

Com o **Adobe Campaign**, teste uma mensagem antes de enviá-la para o público principal. Esta etapa valida sua campanha de email e identifica possíveis problemas.

O envio de provas é crucial para garantir a qualidade e a eficácia do delivery. Os recipients de prova revisam vários elementos, como links, links para opção de não participação e imagens, e identificam erros na renderização, conteúdo, configurações de personalização e configuração de SMS. Esse processo avalia e otimiza completamente o SMS antes de alcançar seu público principal.

![Ícone de livro para enviar provas](../assets/do-not-localize/book.png) Saiba como enviar provas em [esta seção](../preview-test/test-deliveries.md).

![Testando entrega de SMS](assets/sms_send_6.png){zoomable="yes"}

## Enviar a entrega de SMS {#send-sms}

1. Depois de personalizar seu conteúdo de SMS, clique em **[!UICONTROL Revisar e enviar]** na sua página **[!UICONTROL Entrega]**.

   ![Revisar e enviar a entrega de SMS](assets/sms_send_4.png){zoomable="yes"}

1. Clique em **[!UICONTROL Preparar]** e monitore o progresso e as estatísticas fornecidas.

   Se ocorrerem erros, consulte o menu Logs para obter informações detalhadas sobre a falha.

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para prosseguir com o processo de envio final.

   ![Enviando entrega de SMS](assets/sms_send_5.png){zoomable="yes"}

   Se a entrega do SMS estiver agendada, clique no botão **[!UICONTROL Enviar como agendado]**. Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-messages.md#schedule-the-delivery-sending).

1. Confirme a ação de envio clicando no botão **[!UICONTROL Enviar]**.

Depois que a entrega for enviada, rastreie os dados dos KPIs (indicadores principais de desempenho) na página de entrega e os dados no menu **[!UICONTROL Logs]**.

Comece a medir o impacto da sua mensagem com relatórios integrados. [Saiba mais](../reporting/sms-report.md)