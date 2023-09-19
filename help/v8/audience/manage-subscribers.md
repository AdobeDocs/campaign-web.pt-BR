---
audience: end-user
title: Gerenciar os assinantes de um serviço
description: Saiba como gerenciar e fornecer aos assinantes de um serviço no Adobe Campaign Web
badge: label="Beta"
source-git-commit: 5125de258edd4e3eda9a8507228156ee40215532
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 2%

---


# Gerenciar os assinantes de um serviço {#manage-subscribers}

Uma vez que [criou um serviço](manage-services.md#create-service), você pode adicionar assinantes, cancelar a assinatura de destinatários e entregar aos assinantes desse serviço.

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

## Entregar aos assinantes de um serviço

Uma vez que [criou um serviço de assinatura](manage-services.md#create-service), o pode direcionar os assinantes em um delivery. Siga as etapas abaixo.

1. [Criar um público](../audience/create-audience.md) incluindo os assinantes do serviço criado:

   * No **[!UICONTROL Criar público-alvo]** atividade, exibir os atributos avançados e selecionar **[!UICONTROL Recipient]** > **[!UICONTROL Assinaturas]** > **[!UICONTROL Serviço]**.

   * Neste exemplo, selecione os usuários que assinaram o serviço que tem a **Informativo da Luma** rótulo.

   ![](assets/service-audience-subscribers.png)

1. [Criar um delivery](../msg/gs-messages.md#create-delivery) e selecione o público criado acima.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Edite o conteúdo da mensagem conforme desejado e envie o delivery.

   ![](assets/service-delivery-ready.png)

Seu delivery é enviado somente aos assinantes desse serviço.
