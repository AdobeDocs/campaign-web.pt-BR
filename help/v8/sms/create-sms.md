---
audience: end-user
title: Criar uma entrega de SMS
description: Saiba como criar e enviar SMS com o Adobe Campaign Web
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 43%

---

# Criar uma entrega de SMS {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Propriedades de entrega de SMS"
>abstract="As propriedades abrangem os parâmetros de entrega comuns que ajudam a nomear e classificar sua entrega. Se a entrega for baseada em um schema estendido, campos de opções personalizadas específicos estarão disponíveis."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Defina o público-alvo do SMS"
>abstract="Você pode criar um novo público-alvo ou selecionar um existente clicando em **Selecionar público-alvo**. Se necessário, adicione um grupo de controle para medir o impacto da sua entrega."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=pt-BR" text="Definir um grupo de controle"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Seleção de modelo de SMS"
>abstract="Selecione um modelo predefinido para iniciar a entrega do SMS. Os modelos de entrega permitem reutilizar facilmente o conteúdo e as configurações personalizadas em suas campanhas e entregas."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html?lang=pt-BR" text="Usar modelos de entrega"


Você pode criar um delivery de SMS independente ou criar um SMS no contexto de um workflow da campanha. As etapas abaixo detalham o procedimento para um delivery de SMS independente (único). Se você estiver trabalhando no contexto de um fluxo de trabalho de campanha, as etapas de criação serão os detalhes em [esta seção](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Para criar um novo delivery de SMS independente, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Entregas]** no painel esquerdo e clique no botão **[!UICONTROL Criar entrega]**.

1. Na seção **[!UICONTROL Canal]**, escolha SMS como canal e selecione um modelo. [Saiba mais sobre modelos](../msg/delivery-template.md)

1. Clique no botão **[!UICONTROL Criar entrega]** para confirmar.

   ![](assets/sms_create_1.png){zoomable="yes"}

1. Insira um **[!UICONTROL Rótulo]** para a entrega e acesse o menu suspenso **[!UICONTROL Opções adicionais]**. Se a sua entrega for baseada em um esquema estendido, campos específicos de **Opções personalizadas** estarão disponíveis.

   +++Defina as seguintes configurações com base nos seus requisitos.
   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazene a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: organize suas entregas usando sua própria convenção de nomeação.
   * **[!UICONTROL Descrição]**: forneça uma descrição da entrega.
   * **[!UICONTROL Natureza]**: especifique a natureza da entrega para fins de classificação.
+++

1. Clique no botão **[!UICONTROL Selecionar público-alvo]** para direcionar um público já existente ou criar o seu próprio. [Saiba mais sobre públicos](../audience/about-recipients.md).

   ![](assets/sms_create_2.png){zoomable="yes"}

   Saiba como selecionar um público existente [nesta página](../audience/add-audience.md)

   Saiba como criar um novo público-alvo [nesta página](../audience/one-time-audience.md)

1. Ative a opção **[!UICONTROL Habilitar grupo de controle]** para definir um grupo de controle e medir o impacto da sua entrega. As mensagens não são enviadas para esse grupo de controle, para que você possa comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não receberam. [Saiba mais](../audience/control-group.md)

1. Clique em **[!UICONTROL Editar conteúdo]** para começar a criar o conteúdo da sua mensagem SMS. [Saiba mais](content-sms.md)

   ![](assets/sms_create_4.png){zoomable="yes"}

   Nesta tela, você também pode [simular seu conteúdo](../preview-test/preview-test.md) e [configurar ofertas](../msg/offers.md).

1. Para programar sua entrega para uma data e hora específicas, ative a opção **[!UICONTROL Habilitar agendamento]**. Depois de iniciar o delivery, a mensagem será enviada automaticamente na data e hora exatas definidas para o recipient. Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Quando uma entrega é enviada no contexto de um fluxo de trabalho, você deve usar a atividade **Scheduler**. Saiba mais [nesta página](../workflows/activities/scheduler.md).

1. Clique em **[!UICONTROL Configurações]** para acessar as opções avançadas relacionadas ao seu modelo de entrega. [Saiba mais](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable="yes"}
