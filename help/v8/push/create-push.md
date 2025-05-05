---
audience: end-user
title: Criar uma entrega de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 24%

---

# Criar uma entrega de notificação por push {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Modelo de notificação por push"
>abstract="Selecione um modelo de notificação por push para iniciar a entrega por push. Os modelos de entrega permitem reutilizar facilmente o conteúdo e as configurações personalizadas em suas campanhas e entregas."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=pt-BR" text="Usar modelos de entrega"

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Propriedades da entrega por push"
>abstract="Defina as propriedades da entrega por push. Insira o rótulo do push e use as **Opções Adicionais** para configurar o nome interno, a pasta de entrega e o código. Você também pode inserir uma descrição personalizada."

Você pode criar um delivery de notificação por push independente ou criar uma notificação por push no contexto de um workflow da campanha. As etapas abaixo detalham o procedimento para um delivery push independente (único). Se você estiver trabalhando no contexto de um fluxo de trabalho de campanha, as etapas de criação serão detalhadas em [esta seção](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Criar uma entrega por push {#create-push-delivery}

Para criar um novo delivery por push independente, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Entregas]** no painel esquerdo e clique no botão **[!UICONTROL Criar entrega]**.

1. Na seção **[!UICONTROL Canal]**, escolha **Notificação por push** como canal e selecione um modelo, dependendo do sistema operacional do dispositivo escolhido: Android ou iOS. [Saiba mais sobre modelos](../msg/delivery-template.md)

1. Clique no botão **[!UICONTROL Criar entrega]** para confirmar.

   ![Captura de tela mostrando a criação de uma entrega por push](assets/push_create_1.png){zoomable="yes"}

## Definir as configurações de entrega {#configure-push-settings}

Defina as configurações de delivery conforme detalhado abaixo:

1. Insira um **[!UICONTROL Rótulo]** para a entrega. Por padrão, o rótulo é definido com o rótulo do template selecionado. Deve ser atualizado.

1. Navegue pelo menu suspenso **[!UICONTROL Opções adicionais]** para personalizar as opções, se necessário. Se a sua entrega for baseada em um esquema estendido, campos específicos de **Opções personalizadas** estarão disponíveis.

   +++Defina as seguintes configurações com base nos seus requisitos.
   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazene a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: organize suas entregas usando sua própria convenção de nomeação.
   * **[!UICONTROL Descrição]**: forneça uma descrição da entrega.
   * **[!UICONTROL Natureza]**: especifique a natureza da entrega para fins de classificação.

   +++

## Selecionar o público-alvo da entrega por push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definir o público-alvo da notificação por push"
>abstract="Para definir o público-alvo da mensagem, primeiro selecione o aplicativo associado à entrega por push. Por padrão, sua notificação por push é enviada a todos os assinantes do aplicativo. É possível definir um público-alvo específico clicando em **Selecionar público-alvo**. Se necessário, adicione um grupo de controle para medir o impacto da sua entrega."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=pt-BR" text="Definir um grupo de controle"

Primeiro, selecione o aplicativo e, depois, refine o público-alvo de notificação por push, conforme detalhado abaixo:

1. Na seção **[!UICONTROL Público-alvo]**, selecione o aplicativo que deseja usar para esta entrega. Por padrão, sua notificação por push é enviada a todos os assinantes do aplicativo. Você pode refinar para um público-alvo específico clicando no botão **[!UICONTROL Selecionar público-alvo]**.

   ![Captura de tela mostrando a seleção de público para entrega por push](assets/push_create_2.png){zoomable="yes"}

1. Selecione um público existente ou crie seu próprio público para refinar a população do target para o delivery de push. Para notificação por push, a [dimensão de destino](../audience/about-recipients.md#targeting-dimensions) padrão é o **Aplicativo do assinante** (nms:appSubscriptionRcp), que está vinculado à tabela de destinatários.

   Saiba como selecionar um público existente [nesta página](../audience/add-audience.md).

   Saiba como criar um novo público-alvo [nesta página](../audience/one-time-audience.md).

1. Ative a opção **[!UICONTROL Habilitar grupo de controle]** para definir um grupo de controle e medir o impacto da sua entrega. As mensagens não são enviadas para esse grupo de controle, portanto, você pode comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não receberam. [Saiba mais](../audience/control-group.md).

## Definir o conteúdo da notificação por push {#create-content-push}

Para definir o conteúdo de sua notificação, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](content-push.md).

![Captura de tela mostrando a edição de conteúdo para entrega por push](assets/push_create_5.png){zoomable="yes"}

Nesta tela, você também pode [simular seu conteúdo](../preview-test/preview-test.md) e [configurar ofertas](../msg/offers.md).

## Agendar o envio do delivery {#schedule-push}

Quando uma entrega é enviada no contexto de um fluxo de trabalho, você deve usar a atividade **Scheduler**. Saiba mais em [esta página](../workflows/activities/scheduler.md). As etapas abaixo se aplicam apenas aos deliveries independentes.

Para programar uma entrega por push independente para uma data e hora específicas, siga estas etapas:

1. Navegue até a seção **[!UICONTROL Agendamento]** das propriedades de entrega.

1. Use o botão de alternância **[!UICONTROL Habilitar agendamento]** para ativá-lo.

1. Defina a data e a hora desejadas para envio.

Após iniciar o delivery, a mensagem será enviada automaticamente na data e hora exatas definidas para o recipient.

![Captura de tela mostrando as opções de agendamento para entrega por push](assets/push_create_3.png){zoomable="yes"}

Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-deliveries.md#gs-schedule).

## Configurações avançadas de entrega {#adv-push}

Clique em **[!UICONTROL Definir configurações de entrega]** para acessar opções avançadas relacionadas ao seu modelo de entrega. [Saiba mais](../advanced-settings/delivery-settings.md).

![Captura de tela mostrando as configurações avançadas para entrega por push](assets/push_create_4.png){zoomable="yes"}