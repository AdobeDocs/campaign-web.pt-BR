---
audience: end-user
title: Criar um delivery de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
badge: label="Alpha"
source-git-commit: 4f7cedc4197a983d4d13294744e30836a0263d3a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 65%

---

# Criar um delivery de notificação por push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Defina o público-alvo do push"
>abstract="Selecione o melhor público-alvo para a sua mensagem por push"

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modelo de notificação por push"
>abstract="Selecione um modelo de notificação por push para iniciar a entrega por push."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propriedades da entrega por push"
>abstract="Gerencie as propriedades da entrega por push."

1. Na página inicial **[!UICONTROL Entregas]**, clique em **[!UICONTROL Criar entrega]**.

1. No **[!UICONTROL Canal]** escolha Notificação por push como canal e selecione um modelo dependendo do sistema operacional escolhido: Android ou iOS. [Saiba mais sobre templates](../msg/delivery-template.md)

1. Clique no botão **[!UICONTROL Criar entrega]** para confirmar.

   ![](assets/push_create_1.png)

1. Insira um **[!UICONTROL Rótulo]** para a entrega e acesse o menu suspenso **[!UICONTROL Opções adicionais]**.

   +++Defina as seguintes configurações com base nos seus requisitos.
   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazene a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: organize suas entregas usando sua própria convenção de nomeação.
   * **[!UICONTROL Descrição]**: forneça uma descrição da entrega.
   * **[!UICONTROL Natureza]**: especifique a natureza do email para fins de classificação.
+++

1. No **[!UICONTROL Público]** selecione o aplicativo que deseja usar para esse delivery.

1. Clique no botão **[!UICONTROL Selecionar público-alvo]** para direcionar um público já existente ou criar o seu próprio. [Saiba mais](../audience/about-audiences.md)

   Observe que, por padrão, sua notificação por push será enviada a todos os assinantes do aplicativo.

   ![](assets/push_create_2.png)

1. Ative a opção **[!UICONTROL Habilitar grupo de controle]** e defina um grupo de controle para medir o impacto da entrega, permitindo comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não receberam. [Saiba mais](../audience/control-group.md)

1. Clique em **[!UICONTROL Editar conteúdo]** para começar a projetar o conteúdo da sua notificação por push. [Saiba mais](content-push.md)

   ![](assets/push_create_5.png)

   Nessa tela, também é possível [simular seu conteúdo](../preview-test/preview-test.md) e [configurar ofertas](../content/offers.md).

1. Para programar sua entrega para uma data e hora específicas, ative a opção **[!UICONTROL Habilitar agendamento]**. Depois de iniciar a entrega, a mensagem será enviada automaticamente na data e hora exatas definidas para o destinatário.

   ![](assets/push_create_3.png)

1. Clique em **[!UICONTROL Definir configurações de entrega]** para acessar opções avançadas relacionadas ao seu template do delivery. [Saiba mais](../advanced-settings/delivery-settings.md)

   ![](assets/push_create_4.png)
