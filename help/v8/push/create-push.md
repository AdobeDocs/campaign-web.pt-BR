---
audience: end-user
title: Criar uma entrega de notificação por push
description: Saiba como criar um delivery de notificação por push com o Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 933cfcdfb9ff9a176f4942e349b882c404c4e2a8
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 31%

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
>abstract="Defina as propriedades da entrega por push. Insira o rótulo do push e use as **Opções adicionais** para configurar o nome interno, a pasta de entrega e o código. Você também pode inserir uma descrição personalizada."

Você pode criar um delivery de notificação por push independente ou criar uma notificação por push no contexto de um workflow da campanha. As etapas abaixo detalham o procedimento para um delivery push independente (único). Se estiver trabalhando no contexto de um workflow da campanha, as etapas de criação serão detalhadas em [nesta seção](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Criar uma entrega por push {#create-push-delivery}

Para criar um novo delivery por push independente, siga estas etapas:

1. Navegue até o **[!UICONTROL Entregas]** no painel à esquerda e clique no botão  **[!UICONTROL Criar entrega]** botão.

1. No **[!UICONTROL Canal]** escolha **Notificação por push** como canal e selecione um modelo, dependendo do sistema operacional do dispositivo escolhido: Android ou iOS. [Saiba mais sobre modelos](../msg/delivery-template.md)

1. Clique no botão **[!UICONTROL Criar entrega]** para confirmar.

   ![](assets/push_create_1.png){zoomable=&quot;yes&quot;}

## Definir as configurações de entrega {#configure-push-settings}

Defina as configurações de delivery conforme detalhado abaixo:

1. Insira um **[!UICONTROL Rótulo]** para o delivery. Por padrão, o rótulo é definido com o rótulo do template selecionado. Deve ser atualizado.

1. Navegue pelo **[!UICONTROL Opções adicionais]** para personalizar as opções, se necessário. Se o seu delivery for baseado em um schema estendido, **Opções personalizadas** campos estão disponíveis.

   +++Defina as seguintes configurações com base nos seus requisitos.
   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazene a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: organize suas entregas usando sua própria convenção de nomeação.
   * **[!UICONTROL Descrição]**: forneça uma descrição da entrega.
   * **[!UICONTROL Natureza]**: especifique a natureza do delivery para fins de classificação.
+++


## Selecionar o público-alvo da entrega por push {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Definir o público-alvo da notificação por push"
>abstract="Para definir o público-alvo da mensagem, primeiro selecione o aplicativo associado à entrega por push. Por padrão, sua notificação por push é enviada a todos os assinantes do aplicativo. É possível definir um público-alvo específico clicando em **Selecionar público-alvo**. Se necessário, adicione um grupo de controle para medir o impacto da sua entrega."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=pt-BR" text="Definir um grupo de controle"


Primeiro, selecione o aplicativo e, depois, refine o público-alvo de notificação por push, conforme detalhado abaixo:

1. No **[!UICONTROL Público]** selecione o aplicativo que deseja usar para esse delivery. Por padrão, sua notificação por push é enviada a todos os assinantes do aplicativo. É possível refinar para um público-alvo específico clicando no link **[!UICONTROL Selecionar público]** botão.

   ![](assets/push_create_2.png){zoomable=&quot;yes&quot;}

1. Selecione um público existente ou crie seu próprio público para refinar a população do target para o delivery de push. Para Notificações por push, o padrão é [dimensão de destino](../audience/about-recipients.md#targeting-dimensions) é **Aplicativo do assinante** (nms:appSubscriptionRcp), que está vinculado à tabela de recipients.

   Saiba como selecionar um público existente no [esta página](../audience/add-audience.md)

   Saiba como criar um novo público-alvo no [esta página](../audience/one-time-audience.md)

1. Ligue o **[!UICONTROL Ativar grupo de controle]** opção para definir um grupo de controle para medir o impacto do delivery. As mensagens não são enviadas para esse grupo de controle, para que você possa comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não receberam. [Saiba mais](../audience/control-group.md)

## Definir o conteúdo da notificação por push {#create-content-push}

Para definir o conteúdo de sua notificação, clique em **[!UICONTROL Editar conteúdo]**. [Saiba mais](content-push.md)

![](assets/push_create_5.png){zoomable=&quot;yes&quot;}

Nessa tela, também é possível [simular seu conteúdo](../preview-test/preview-test.md) e [configurar ofertas](../msg/offers.md).

## Agendar o envio do delivery {#schedule-push}

Quando um delivery é enviado no contexto de um workflow, você deve usar o **Scheduler** atividade. Saiba mais em [esta página](../workflows/activities/scheduler.md). As etapas abaixo se aplicam apenas aos deliveries independentes.

Para programar uma entrega por push independente para uma data e hora específicas, siga estas etapas:

1. Navegue até o **[!UICONTROL Agendar]** seção das propriedades de delivery.

1. Use o **[!UICONTROL Ativar agendamento]** para ativá-la.

1. Defina a data e a hora desejadas para envio.

Após iniciar o delivery, a mensagem será enviada automaticamente na data e hora exatas definidas para o recipient.

![](assets/push_create_3.png){zoomable=&quot;yes&quot;}

Saiba mais sobre a programação de delivery em [nesta seção](../msg/gs-messages.md#gs-schedule)

## Configurações avançadas de entrega {#adv-push}

Clique em **[!UICONTROL Definir configurações de entrega]** para acessar opções avançadas relacionadas ao seu template do delivery. [Saiba mais](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png){zoomable=&quot;yes&quot;}
