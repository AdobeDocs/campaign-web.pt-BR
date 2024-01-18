---
audience: end-user
title: Enviar mensagens aos assinantes de um serviço
description: Saiba como enviar mensagens aos assinantes de um serviço
badge: label="Disponibilidade limitada"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 2%

---

# Enviar mensagens aos assinantes de um serviço {#send-to-subscribers}

Você pode criar serviços de assinatura no Adobe Campaign e enviar mensagens aos assinantes. Saiba como criar serviços de subscrições no [esta página](../audience//manage-services.md#create-service).

Para enviar mensagens aos assinantes, crie um público-alvo específico para identificá-los e, em seguida, crie o delivery conforme detalhado abaixo.

1. Criar um público-alvo. Saiba mais sobre públicos-alvo na [esta página](../audience/create-audience.md).

1. No **[!UICONTROL Criar público-alvo]** atividade, exibir os atributos avançados e selecionar **[!UICONTROL Recipient]** > **[!UICONTROL Assinaturas]** > **[!UICONTROL Serviço]**.

   Neste exemplo, selecione os usuários que assinaram o serviço que tem a **Informativo da Luma** rótulo.

   ![](assets/service-audience-subscribers.png)

1. Salve o público.
1. Criar um delivery. As etapas para criar um delivery estão detalhadas em [esta página](../msg/gs-messages.md#create-delivery).
1. Navegue até as configurações de entrega e altere o target mapping padrão para **Assinaturas (nms:subscriptions)**.

   ![](assets/service-delivery-change-mapping.png)

1. Na seção principal do target do delivery, selecione o público-alvo criado acima.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Crie o conteúdo da mensagem, teste e envie o delivery, conforme detalhado em [nesta seção](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Seu delivery é enviado somente aos assinantes desse serviço.
