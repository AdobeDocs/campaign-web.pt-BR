---
audience: end-user
title: Criar campanhas com o Adobe Campaign Web
description: Saiba como criar campanhas entre canais com o Adobe Campaign Web
exl-id: a6e01470-73e5-4973-aa6a-9836a6ee1cd2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 35%

---

# Criar sua primeira campanha {#create-first-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_properties"
>title="Propriedades de criação de campanha"
>abstract="Nesta tela, defina as configurações da campanha: selecione um modelo e insira um rótulo para a campanha. Navegue até as configurações adicionais para alterar o nome interno padrão, a pasta, adicionar uma descrição e selecionar o responsável."

>[!CONTEXTUALHELP]
>id="acw_campaign_properties"
>title="Propriedades da campanha"
>abstract="Nesta tela, é possível verificar e atualizar as configurações da campanha: rótulo, nome interno, pasta e descrição. Você também pode visualizar a quem ela está atribuída."

Para criar uma nova campanha, defina suas configurações, agende e inclua workflows e deliveries.

## Criar a campanha {#campaign-create}

Para criar uma nova campanha, siga estas etapas:

1. Clique no menu **[!UICONTROL Campanhas]** e clique no botão **[!UICONTROL Criar campanha]**.

   ![Captura de tela mostrando o botão &quot;Criar campanha&quot; no menu Campanhas](assets/create-campaign-button.png)

1. Selecione o **Modelo** a ser usado e forneça um rótulo para a campanha. [Leia mais](manage-campaigns.md#manage-campaign-templates).
1. Se necessário, altere as seguintes **Opções adicionais**: nome interno, pasta, destinatário, descrição e natureza.
1. Defina o **Agendamento** da sua campanha. Saiba como definir o agendamento da campanha em [esta seção](#campaign-schedule).
1. Clique em **Create**.

   ![Captura de tela mostrando a tela de propriedades da campanha, incluindo campos para nome interno, pasta, destinatário, descrição e natureza.](assets/create-a-campaign-properties.png)

1. Adicione workflows e deliveries à sua campanha:

   * Na guia **Fluxos de trabalho**, clique em **Criar fluxo de trabalho**. Um workflow padrão é adicionado automaticamente ao criar sua campanha. Saiba como [criar um fluxo de trabalho](../workflows/create-workflow.md).

   * Na guia **Entregas**, clique em **Criar entrega**. [Saiba mais](../msg/gs-messages.md)

## Monitorar e rastrear sua campanha {#campaign-monitoring}

O monitoramento da campanha é uma etapa essencial para analisar a eficácia da campanha. Abra a campanha e clique no botão **Logs**.

Você também pode exibir os relatórios dedicados clicando no botão **Relatórios**. Consulte esta [seção](../reporting/campaign-reports.md).

## Definir a programação da campanha {#campaign-schedule}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_schedule"
>title="Programação de campanha"
>abstract="Selecione a programação de campanha. É possível criar a campanha para que ela comece na data inicial. Por padrão, a data inicial da campanha é a data de criação, e ela dura 5 dias. As datas inicial e final são exibidas na lista de campanhas e podem ser usadas como um filtro."

A campanha começa quando a data de início é atingida. Desde que a data de início não seja atingida, a campanha terá o status **[!UICONTROL Rascunho]**. Quando a data de início é atingida, ela muda para **[!UICONTROL Em andamento]**. Ao atingir a data de término, a campanha será definida como **[!UICONTROL Concluída]**.

As datas de início e término são exibidas na lista de campanhas e podem ser usadas como filtro. Consulte esta [seção](manage-campaigns.md#access-campaigns).

>[!NOTE]
>
>Você pode modificar essas propriedades posteriormente, a partir do ícone **Definir configurações da campanha** ao lado do rótulo da campanha. Consulte esta [seção](gs-campaigns.md#campaign-dashboard).

Quando a data é atingida, os deliveries criados nessa campanha no contexto de um workflow, que estão prontos para serem enviados, são realmente enviados. Para isso, o workflow deve ter sido iniciado.

<!--
    +++WORKF
++screen
## Create a cross-channel campaign {#cross-channel-campaign}

In a cross-channel campaign, a single marketing communication uses different channels. Data is passed between the channels. The customer receives communication through multiple channels based on, for example, their interaction with the previous communication.
-->
<!--
existing campaign: settings button -> properties like when creation
schedule in header

About plans, programs and campaigns
Adobe Campaign allows you to plan marketing campaigns in which you can create and manage different types of activities: emails, SMS messages, push notifications, workflows, landing pages. These campaigns and their contents can be gathered into programs.

The programs and campaigns allow you to regroup and view the different marketing activities that are linked to them.

A program may contain other programs as well as campaigns, workflows, and landing pages. It appears in the timeline and helps you organize your marketing activities: you can separate them by country, by brand, by unit, and similar criteria.

A campaign enables you to gather all the marketing activities of your choice under a single entity. A campaign may contain emails, SMS, push notifications, direct mails, workflows, and landing pages.

To better organize your marketing plans, Adobe recommends the following hierarchy: Program > Sub-programs > Campaigns > Workflows > Deliveries.

Reports on programs and campaigns allow you to analyze their impact. For example, you can build reports at the campaign level to aggregate data on all deliveries contained in that campaign.

Related topics:

* Timeline
* About dynamic reports
* Creating a campaign

In programs and sub-programs, you can add campaigns. Campaigns can contain marketing activities such as emails, SMS, push notifications, workflows, and landing pages.

From the Adobe Campaign home page, select the Programs & Campaigns card, and access a program or sub-program.

Click on the Create button, and select Campaign.

In the Creation mode screen, select a campaign type.

The campaign types available are based on templates defined in Resources > Templates > Campaign templates. For more on this, refer to the Managing templates section.

In the Properties screen, enter the name and ID of the campaign.

Select a start and end date for your campaign. These dates only apply to the campaign itself.

Click on Create to confirm the creation of the campaign.

The campaign is created and displayed. Use the Create button to add marketing activities to your campaign.

>[!NOTE]
>
>Depending on your license agreement, you may access only some of these activities.

You can also create a campaign from the marketing activity list. You can choose to link the marketing activity to a parent program or sub-program via the properties window of the campaign.

Programs and campaigns icons and statuses:

Each program and each campaign in the list has a visual symbol and an icon whose color indicates the execution status. This status depends on the validity period of the program or the campaign.

* Gray: the program/campaign has not yet started - Editing status.
* Blue: the program/campaign is in progress - In progress status.
* Green: the program/campaign has finished - Finished status.

By default, the current date is automatically shown as the validity start date, and the end date is calculated according to the start date (D+186 days). You can change these dates in the program or campaign properties.

Business.Adobe.com resources
-->