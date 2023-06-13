---
audience: end-user
title: Criar campanhas com o Adobe Campaign Web
description: Saiba como criar campanhas entre canais com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: 3f2fc84132eab0f75aa405ba16f996601b21b784
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 18%

---


# Criar campanhas entre canais {#create-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Propriedades de criação de campanha"
>abstract="Defina as propriedades e os metadados da campanha."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Propriedades da campanha"
>abstract="Defina as configurações e os metadados da campanha."

As campanhas podem incluir workflows e deliveries independentes.

Para criar uma nova campanha, siga estas etapas:

1. Clique em **[!UICONTROL Campanhas]** e clique no botão **[!UICONTROL Criar campanha]** botão.
1. Selecione o **Modelo** para usar e fornecer um rótulo para a campanha. Os templates de campanha são pré-configurados para que possam ser reutilizados para criar novas campanhas. Eles são criados no console do cliente.
   [Leia mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=pt-BR).
1. Se necessário, você pode alterar o seguinte **Opções adicionais**: nome interno, pasta, responsável, descrição e natureza.
1. Defina o **Agendar** da sua campanha. A campanha começa quando a data de início é atingida. As datas de início e término são exibidas na lista de campanhas e podem ser usadas como filtro. Consulte esta [seção](gs-campaigns.md#access-campaigns).

   ![Definir as propriedades da campanha](assets/campaign-properties.png)

   >[!NOTE]
   >
   >Você sempre pode modificar essas propriedades posteriormente, no **Definir configurações da campanha** ícone, ao lado do rótulo da campanha. Consulte esta [seção](gs-campaigns.md#campaign-dashboard)

1. Clique em **Create**.
1. Adicione workflows e deliveries à sua campanha.

   * No **Fluxos de trabalho** clique em **Criar fluxo de trabalho**. Um workflow padrão é adicionado automaticamente ao criar sua campanha. Saiba como [criar um fluxo de trabalho](../workflows/create-workflow.md)
   * No **Entregas** clique em **Criar entrega**. [Saiba mais](../msg/gs-messages.md)

1. Use o **Logs** e **Relatórios** botões para analisar sua campanha.

## Logs de monitoramento e rastreamento{#campaign-monitoring}

O monitoramento de campanhas é uma etapa essencial para analisar suas campanhas. Abra a campanha e clique no link **Logs** botão.

Também é possível exibir os relatórios dedicados clicando no link **Relatórios** botão. Consulte esta [seção](../reporting/campaign-reports.md).

## Duplicar e excluir uma campanha

É possível duplicar ou excluir uma campanha:

* na lista de campanhas, clique no botão de reticências e selecione **Duplicar** ou **Excluir**.
* na própria campanha, clique no link **Mais** e selecione **Duplicar** ou **Excluir**.

>[!NOTE]
>
>A variável **Entrega** exibe todos os deliveries vinculados à campanha. No entanto, os deliveries criados em um workflow não podem ser excluídos dali. Para excluir um delivery criado no contexto de um workflow, você deve excluir a atividade de delivery do workflow.


<!--
## Create a cross-channel campaign {#cross-channel-campaign}


>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Workflow list"
>abstract="List of workflows available for your campaign. Use the 'Create workflow' button to add a workflow in your campaign."

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.

-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header


About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and help you organize your marketing activities: you can separate them by country, by brand, by unit, etc.
A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.
To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

Timeline
About dynamic reports
Creating a campaign
In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card and access a program or sub-program.

Click on the Create button and select Campaign.

In the Creation mode screen, select a campaign type.



The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date to your campaign. These dates only apply to the campaign itself.



Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

NOTE
Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.


Programs and campaigns icons and statuses
Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

Gray: the program/campaign has not yet started - Editing status.
Blue: the program/campaign is in progress - In progress status.
Green: the program/campaign has finished - Finished status. By default, the current date is automatically shown as the validity start date and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.


Business.Adobe.com resources
-->
