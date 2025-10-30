---
audience: end-user
title: Enviar mensagens aos assinantes de um serviço
description: Saiba como enviar mensagens aos assinantes de um serviço
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Enviar mensagens aos assinantes de um serviço {#send-to-subscribers}

Você pode criar serviços de subscrição no Adobe Campaign e enviar mensagens aos seus assinantes. Saiba como criar serviços de assinatura [nesta página](../audience//manage-services.md#create-service).

Para enviar mensagens aos assinantes, crie um público-alvo específico para identificá-los e, em seguida, crie o delivery conforme detalhado abaixo.

1. Criar um público-alvo. Um novo workflow é criado automaticamente. [Saiba mais sobre públicos](../audience/create-audience.md).

1. Para melhorar a compreensão, altere o nome do fluxo de trabalho no campo **Rótulo** das configurações do fluxo de trabalho. [Saiba como definir configurações de fluxo de trabalho](../workflows/workflow-settings.md).

1. Abra a atividade **[!UICONTROL Criar público-alvo]** e selecione **[!UICONTROL Criar público-alvo]**. [Saiba como configurar uma atividade Criar público-alvo](../workflows/activities/build-audience.md).

   ![Captura de tela mostrando a configuração da atividade de criação de público no Adobe Campaign.](assets/service-create-audience.png){zoomable="yes"}

1. No fluxo de criação de público, selecione as seguintes condições personalizadas: **[!UICONTROL Existem assinaturas]**, como **[!UICONTROL Serviço]**, que é igual ao serviço definido. Neste exemplo, selecione seu **informativo sobre a Luma yoga**.

   ![Captura de tela mostrando o fluxo de criação de público-alvo com condições personalizadas para assinaturas no Adobe Campaign.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Selecione **[!UICONTROL Confirmar]** e clique em **[!UICONTROL Iniciar]** para executar o fluxo de trabalho.

1. Criar um delivery. As etapas para criar uma entrega estão detalhadas em [esta página](../msg/gs-messages.md#create-delivery).

1. Navegue até as configurações de entrega e altere o target mapping padrão para **Assinaturas (nms:subscriptions)**.

   ![Captura de tela mostrando as configurações de entrega com o target mapping alterado para Assinaturas no Adobe Campaign.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Na seção principal do target do delivery, selecione o público-alvo criado acima.

   ![Captura de tela mostrando a seção principal do público-alvo da entrega com o público selecionado no Adobe Campaign.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Crie o conteúdo da mensagem, teste-o e envie a entrega, conforme detalhado em [esta seção](../preview-test/preview-test.md).

   ![Captura de tela mostrando a entrega pronta para ser enviada no Adobe Campaign.](assets/service-delivery-ready.png){zoomable="yes"}

Seu delivery é enviado somente aos assinantes desse serviço.