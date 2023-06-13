---
audience: end-user
title: Introdução às campanhas
description: Saiba como começar com as campanhas entre canais
badge: label="Alpha" type="Positive"
exl-id: f2b9f8e6-5ded-4a47-89e9-96650cd78229
source-git-commit: e933562e4046d9cdea9fc898e5c4c4c9a7e9ee38
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 8%

---


# Introdução às campanhas {#campaigns}

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Projetar e enviar campanhas entre canais"
>abstract="Os recursos do Adobe Campaign ajudam você a gerenciar dados centralizados do cliente, projetar comunicações e campanhas do cliente e criar experiências personalizadas em diferentes canais: Email, Push e SMS."

O Adobe Campaign permite que você orquestre facilmente suas iniciativas de marketing direcionadas, usando o recurso integrado de gerenciamento de campanhas. Com a capacidade de definir um agendamento, você pode planejar a duração e o tempo de suas campanhas para se alinharem a objetivos estratégicos e maximizar o engajamento do público-alvo.

Ao adicionar vários workflows e deliveries específicos à campanha, você pode criar experiências personalizadas em vários canais, garantindo que cada ponto de contato corresponda ao público desejado.

As campanhas oferecem métricas de relatórios dedicadas para obter insights abrangentes sobre o desempenho de toda a campanha, permitindo avaliar sua eficácia, identificar tendências e tomar decisões orientadas por dados para otimizar esforços futuros.

<!--
Use Adobe Campaign to create cross-channel campaigns. With its marketing campaign orchestration capabilities, you can manage and centralize customer data, design customer communications and campaigns, and create personalized experiences across different channels. In this version, email, push and SMS channels are available.

Design and execute high-volume email campaigns to deliver personalized messages, for all platforms and screen sizes. 
Measure the effectiveness of your deliveries with detailed reports including the counts of opens, clicks, forwards, and more. With Adobe Campaign segmentation capabilities, you can run queries against a high-volume database, and easily define dynamic marketing segments which perfectly target your campaigns.
-->

<!--
Get Started with campaigns
Adobe Campaign offers a set of solutions that help you personalize and deliver campaigns across all of your online and offline channels. You can create, configure, execute and analyze marketing campaigns. All marketing campaigns can be managed from a unified control center. Discover how to browse and create marketing campaigns in this section.

Campaigns include actions (deliveries) and processes (importing or extracting files), as well as resources (marketing documents, delivery outlines). They are used in marketing campaigns. Campaigns are part of a program, and programs are included in a campaign plan.
-->

## Acessar e gerenciar suas campanhas{#access-campaigns}

Para criar uma nova campanha ou gerenciar suas campanhas existentes, clique no link **[!UICONTROL Campanhas]** menu. Duas guias estão disponíveis:

* A variável **Procurar** A guia lista todas as campanhas existentes. Você pode clicar em uma campanha para abrir seu painel ou criar uma nova campanha clicando no **Criar campanha** botão. Consulte esta [seção](create-campaigns.md#create-campaigns)

* A variável **Modelos** A guia lista todos os templates de campanha disponíveis. Os templates de campanha são pré-configurados para que possam ser reutilizados para criar novas campanhas. Eles são criados no console do cliente. [Leia mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=pt-BR).

Cada campanha na lista exibe informações sobre seu status atual, data de criação, última vez que foi modificada, etc.

Você pode personalizar as colunas exibidas clicando no ícone **Configurar coluna para layout personalizado** ícone localizado no canto superior direito da lista. Isso permite adicionar mais informações à lista. Além disso, uma barra de pesquisa e filtros estão disponíveis para facilitar a pesquisa na lista. [Saiba mais](../get-started/user-interface.md#list-screens)

Por exemplo, você pode filtrar pelo cronograma da campanha. Abra o painel Filtros e use o **Data de início - término** seção:

![Lista de campanhas](assets/campaign-filter-on-dates.png)

## O painel de campanha{#campaign-dashboard}

No **Procurar** clique em uma campanha para exibir seu painel. Duas guias estão disponíveis:

* A variável **Fluxos de trabalho** A guia lista todos os workflows vinculados à campanha. Essa guia também permite criar um novo workflow dentro da campanha. Consulte esta [seção](create-campaigns.md#create-campaigns)
* A variável **Entregas** A guia lista todos os deliveries vinculados à campanha. Essa guia também permite criar um novo delivery dentro da campanha. Consulte esta [seção](create-campaigns.md#create-campaigns)

A variável **Definir configurações da campanha** O ícone permite modificar as propriedades da campanha que foram definidas ao criar a campanha. Consulte esta [seção](create-campaigns.md#create-campaigns)

## Logs de monitoramento e rastreamento{#campaign-monitoring}

O monitoramento de campanhas é uma etapa essencial para analisar suas campanhas. Abra a campanha e clique no link **Logs** botão.

Também é possível exibir os relatórios dedicados clicando no link **Relatórios** botão. Consulte esta [seção](../reporting/campaign-reports.md).

## Duplicar e excluir

É possível duplicar ou excluir uma campanha:

* na lista de campanhas, clique no botão de reticências e selecione **Duplicar** ou **Excluir**.
* na própria campanha, clique no link **Mais** e selecione **Duplicar** ou **Excluir**.

>[!NOTE]
>
>A variável **Entrega** A guia exibe todos os deliveries vinculados à campanha, mas os deliveries criados em um fluxo de trabalho não podem ser excluídos. Para excluir um delivery criado no contexto de um workflow, você deve excluir a atividade de delivery do workflow.

