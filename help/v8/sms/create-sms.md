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


Você pode criar um delivery de SMS independente ou criar um SMS no contexto de um workflow da campanha. As etapas abaixo detalham o procedimento para um delivery de SMS independente (único). Se estiver trabalhando no contexto de um workflow da campanha, as etapas de criação serão detalhadas em [nesta seção](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Para criar um novo delivery de SMS independente, siga estas etapas:

1. Navegue até o **[!UICONTROL Entregas]** no painel à esquerda e clique no botão  **[!UICONTROL Criar entrega]** botão.

1. No **[!UICONTROL Canal]** escolha SMS como canal e selecione um modelo. [Saiba mais sobre modelos](../msg/delivery-template.md)

1. Clique no botão **[!UICONTROL Criar entrega]** para confirmar.

   ![](assets/sms_create_1.png){zoomable="yes"}

1. Insira um **[!UICONTROL Rótulo]** para o delivery e acesse o **[!UICONTROL Opções adicionais]** menu suspenso. Se o seu delivery for baseado em um schema estendido, **Opções personalizadas** campos estão disponíveis.

   +++Defina as seguintes configurações com base nos seus requisitos.
   * **[!UICONTROL Nome interno]**: atribua um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazene a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: organize suas entregas usando sua própria convenção de nomeação.
   * **[!UICONTROL Descrição]**: forneça uma descrição da entrega.
   * **[!UICONTROL Natureza]**: especifique a natureza do delivery para fins de classificação.
+++

1. Clique no botão **[!UICONTROL Selecionar público-alvo]** para direcionar um público já existente ou criar o seu próprio. [Saiba mais sobre públicos](../audience/about-recipients.md).

   ![](assets/sms_create_2.png){zoomable="yes"}

   Saiba como selecionar um público existente no [esta página](../audience/add-audience.md)

   Saiba como criar um novo público-alvo no [esta página](../audience/one-time-audience.md)

1. Ligue o **[!UICONTROL Ativar grupo de controle]** opção para definir um grupo de controle para medir o impacto do delivery. As mensagens não são enviadas para esse grupo de controle, para que você possa comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não receberam. [Saiba mais](../audience/control-group.md)

1. Clique em **[!UICONTROL Editar conteúdo]** para começar a projetar o conteúdo da mensagem SMS. [Saiba mais](content-sms.md)

   ![](assets/sms_create_4.png){zoomable="yes"}

   Nessa tela, também é possível [simular seu conteúdo](../preview-test/preview-test.md) e [configurar ofertas](../msg/offers.md).

1. Para programar sua entrega para uma data e hora específicas, ative a opção **[!UICONTROL Habilitar agendamento]**. Depois de iniciar o delivery, a mensagem será enviada automaticamente na data e hora exatas definidas para o recipient. Saiba mais sobre a programação de delivery em [nesta seção](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Quando um delivery é enviado no contexto de um workflow, você deve usar o **Scheduler** atividade. Saiba mais [nesta página](../workflows/activities/scheduler.md).

1. Clique em **[!UICONTROL Configurações]** para acessar opções avançadas relacionadas ao seu template do delivery. [Saiba mais](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable="yes"}
