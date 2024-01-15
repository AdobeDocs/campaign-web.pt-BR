---
audience: end-user
title: Gerenciar os assinantes
description: Saiba como gerenciar e fornecer aos assinantes de um serviço no Adobe Campaign Web
badge: label="Beta"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Gerenciar os assinantes {#manage-subscribers}

Uma vez que [criou um serviço](manage-services.md#create-service), você pode adicionar assinantes, cancelar a assinatura de destinatários e enviar mensagens aos assinantes desse serviço.

O gerenciamento de assinantes é detalhado nesta página. Para saber como enviar mensagens para seus assinantes, consulte [nesta seção](../msg/send-to-subscribers.md).

## Adicionar assinantes ao seu serviço {#add-subscribers}

Para adicionar assinantes manualmente, siga as etapas abaixo.

1. Selecione um serviço existente na **[!UICONTROL Serviços de assinatura]** lista.

1. Selecione o **[!UICONTROL Assinantes]** e clique em **[!UICONTROL Adicionar perfis]**.

   ![](assets/service-subscribers-tab.png)

1. Selecione os perfis que deseja adicionar na lista e clique em **[!UICONTROL Confirmar o]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Clique em **[!UICONTROL Enviar]**.<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)--> Os destinatários selecionados receberão a assinatura [mensagem de confirmação](manage-services.md#create-confirmation-message) que você selecionou quando [criação do serviço](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

Os perfis adicionados são exibidos no **[!UICONTROL Assinantes]** lista. Agora eles estão subscritos no seu serviço.

## Remover assinantes do seu serviço {#remove-subscribers}

### Cancelar inscrição de destinatários manualmente {#manual-unsubscription}

Uma vez que [assinantes adicionados](#add-subscribers) ao seu serviço, você pode cancelar manualmente a assinatura de cada um deles. Siga as etapas abaixo.

1. Selecione um serviço existente na **[!UICONTROL Serviços de assinatura]** lista.

1. Clique no ícone de três pontos ao lado do nome do recipient desejado e selecione **[!UICONTROL Excluir]**.

   ![](assets/service-subscribers-delete.png)

1. Confirme a exclusão e clique **[!UICONTROL Enviar]**. O recipient selecionado receberá o cancelamento de subscrição [mensagem de confirmação](manage-services.md#create-confirmation-message) que você selecionou quando [criação do serviço](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

O recipient é removido do **[!UICONTROL Assinantes]** e não está mais inscrito no seu serviço.

### Cancelar automaticamente a inscrição de destinatários {#automatic-unsubscription}

Um serviço de assinatura pode ter uma duração limitada. Os recipients são automaticamente cancelados quando o período de validade expira.

Este período é especificado quando [criação do serviço](manage-services.md#create-service). No **[!UICONTROL Opções adicionais]**, desative o **[!UICONTROL Período de validade ilimitado]** e definir um período de validade do serviço.

![](assets/service-create-validity-period.png)

Após a expiração da duração especificada, todos os assinantes terão a subscrição cancelada automaticamente desse serviço.
