---
audience: end-user
title: Introdução às campanhas
description: Saiba como começar com as campanhas entre canais
badge: label="Alpha"
source-git-commit: f8d3e227d99387cc82b8db2ab602cd58404ee7ee
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 9%

---


# Acessar e gerenciar suas campanhas{#manage-campaigns}

Para criar uma nova campanha ou gerenciar suas campanhas existentes, clique no link **[!UICONTROL Campanhas]** menu.

## A lista de campanhas{#access-campaigns}

Na lista da campanha, duas guias estão disponíveis:

* A variável **Procurar** A guia lista todas as campanhas existentes. Você pode clicar em uma campanha para abrir seu painel ou criar uma nova campanha clicando no **Criar campanha** botão. Consulte esta [seção](create-campaigns.md#create-campaigns).

* A variável **Modelos** A guia lista todos os templates de campanha disponíveis. Os templates de campanha são pré-configurados para que possam ser reutilizados ao criar novas campanhas. Eles são criados no console do cliente. [Leia mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=pt-BR)

![Lista de campanhas](assets/campaign-list.png)

Cada campanha na lista exibe informações sobre seu status atual, data de criação, última vez que foi modificada, etc.

Você pode personalizar as colunas exibidas clicando no ícone **Configurar coluna para layout personalizado** ícone localizado no canto superior direito da lista. Isso permite adicionar mais informações à lista. Além disso, uma barra de pesquisa e filtros estão disponíveis para facilitar a pesquisa na lista. [Saiba mais](../get-started/user-interface.md#list-screens)

Por exemplo, você pode filtrar pelo cronograma da campanha. Abra o painel de filtro e use o **Data de início - término** seção:

![Filtro de campanha](assets/campaign-filter-on-dates.png)

## O painel de campanha{#campaign-dashboard}

No **Procurar** da lista da campanha, clique em uma campanha para exibir seus detalhes.

![Painel de campanha](assets/campaign-dashboard.png)

O status e o agendamento da campanha são exibidos na parte superior da tela. Você pode usar o **Definir configurações da campanha** ícone para modificar as propriedades da campanha que foram definidas ao criar a campanha. Há três botões disponíveis que permitem visualizar logs, criar relatórios, duplicar ou excluir a campanha. Consulte esta [seção](create-campaigns.md#create-campaigns)

Duas guias estão disponíveis:

* A variável **Fluxos de trabalho** A guia lista todos os workflows vinculados à campanha. Essa guia também permite criar um novo workflow dentro da campanha. Consulte esta [seção](create-campaigns.md#create-campaigns).

* A variável **Entregas** A guia lista todos os deliveries vinculados à campanha. Você também pode criar um novo delivery dentro da campanha. Consulte esta [seção](create-campaigns.md#create-campaigns).

## Duplicar e excluir uma campanha

É possível duplicar ou excluir uma campanha:

* na lista de campanhas, clique no botão de reticências e selecione **Duplicar** ou **Excluir**.
* na própria campanha, clique no link **Mais** e selecione **Duplicar** ou **Excluir**.

>[!NOTE]
>
>A variável **Entregas** exibe todos os deliveries vinculados à campanha. No entanto, os deliveries criados em um workflow não podem ser excluídos dali. Para excluir um delivery criado no contexto de um workflow, você deve excluir a atividade de delivery do workflow. [Saiba mais](../msg/gs-messages.md#delivery-delete).
