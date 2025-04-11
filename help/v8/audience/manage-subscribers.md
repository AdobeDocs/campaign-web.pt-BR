---
audience: end-user
title: Gerenciar os assinantes
description: Saiba como gerenciar e fornecer aos assinantes de um serviço no Adobe Campaign Web
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 0%

---

# Gerenciar os assinantes {#manage-subscribers}

Depois que você [criou um serviço](manage-services.md#create-service), poderá adicionar assinantes, cancelar a assinatura de destinatários e enviar mensagens aos assinantes desse serviço.

O gerenciamento de assinantes é detalhado nesta página. Para saber como enviar mensagens aos seus assinantes, consulte [esta seção](../msg/send-to-subscribers.md).

## Adicionar assinantes ao seu serviço {#add-subscribers}

Para adicionar assinantes manualmente, siga as etapas abaixo.

1. Selecione um serviço existente na lista **[!UICONTROL Subscription services]**.

1. Vá para a guia **[!UICONTROL Assinantes]** e clique em **[!UICONTROL Adicionar assinantes]**.

   ![Captura de tela mostrando a guia Assinantes na interface dos Serviços de assinatura.](assets/service-subscribers-tab.png){zoomable="yes"}

1. Selecione os perfis que deseja adicionar na lista e clique em **[!UICONTROL Confirmar]**.

   ![Captura de tela mostrando a interface de seleção de perfil para adicionar assinantes.](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Clique em **[!UICONTROL Enviar]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> para que os destinatários selecionados recebam a [mensagem de confirmação](manage-services.md#create-confirmation-message) da assinatura definida ao [criar o serviço](manage-services.md#create-service).

   ![Captura de tela mostrando a interface da mensagem de confirmação para adicionar assinantes.](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se você selecionar **[!UICONTROL Cancelar]**, nenhuma mensagem de confirmação será enviada aos perfis selecionados, mas eles são assinantes.

Os perfis adicionados são exibidos na guia **[!UICONTROL Assinantes]**. Agora eles estão subscritos no seu serviço.

## Remover assinantes do seu serviço {#remove-subscribers}

### Cancelar inscrição manual de perfis {#manual-unsubscription}

Depois de [adicionar assinantes](#add-subscribers) ao seu serviço, você pode cancelar manualmente a assinatura de cada um deles. Siga as etapas abaixo.

1. Selecione um serviço existente na lista **[!UICONTROL Subscription services]**.

1. Clique no ícone de três pontos ao lado do nome do destinatário desejado e selecione **[!UICONTROL Excluir]**.

   ![Captura de tela mostrando a opção de exclusão para cancelar a assinatura de perfis.](assets/service-subscribers-delete.png){zoomable="yes"}

1. Confirmar exclusão.

1. Clique em **[!UICONTROL Enviar]** para que o destinatário selecionado receba a [mensagem de confirmação](manage-services.md#create-confirmation-message) de cancelamento de assinatura que você definiu ao [criar o serviço](manage-services.md#create-service).

   ![Captura de tela mostrando a interface da mensagem de confirmação para cancelar a assinatura de perfis.](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

O destinatário foi removido da guia **[!UICONTROL Assinantes]** e não está mais inscrito no seu serviço.

### Cancelar automaticamente a inscrição de destinatários {#automatic-unsubscription}

Um serviço de assinatura pode ter uma duração limitada. A subscrição dos perfis é automaticamente cancelada quando o período de validade expira.

Este período é especificado ao [criar o serviço](manage-services.md#create-service). Nas **[!UICONTROL Opções adicionais]**, desabilite a opção **[!UICONTROL Período de validade ilimitado]** e defina um período de validade para o serviço.

![Captura de tela mostrando a configuração do período de validade de um serviço de assinatura.](assets/service-create-validity-period.png){zoomable="yes"}

Após a expiração da duração especificada, todos os assinantes terão a subscrição cancelada automaticamente desse serviço.