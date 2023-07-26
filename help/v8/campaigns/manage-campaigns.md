---
audience: end-user
title: Introdução às campanhas
description: Saiba como começar com as campanhas entre canais
badge: label="Alfa"
source-git-commit: c9954ce69e50e1c8db2532be3292f71ff20f9f74
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 100%

---


# Acesso e gerenciamento de suas campanhas{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Programação de campanha"
>abstract="Defina ou modifique a programação da campanha."

Para criar uma nova campanha ou gerenciar suas campanhas já existentes, clique no menu **[!UICONTROL Campanhas]** no painel de navegação esquerdo.

## A lista de campanhas{#access-campaigns}

Na lista de campanhas, duas guias estão disponíveis:

* A guia **Procurar** lista todas as campanhas existentes. É possível clicar em uma campanha para abrir seu painel ou criar uma nova campanha clicando no botão **Criar campanha**. Consulte esta [seção](create-campaigns.md#create-campaigns).

* A guia **Modelos** lista todos os modelos de campanha disponíveis. Os modelos de campanha são pré-configurados para que possam ser reutilizados ao criar novas campanhas. Eles são criados no console cliente. [Leia mais](https://experienceleague.adobe.com/docs/campaign/automation/campaign-orchestration/marketing-campaign-templates.html?lang=pt-BR)

![Lista de campanhas](assets/campaign-list.png)

Por padrão, cada campanha da lista exibe informações sobre seu status atual, data de criação, última modificação etc.

É possível personalizar as colunas exibidas clicando no ícone **Configurar coluna para um layout personalizado** localizado no canto superior direito da lista. Isso permite adicionar mais informações à lista. Além disso, uma barra de pesquisa e filtros estão disponíveis para facilitar a pesquisa na lista. [Saiba mais](../get-started/user-interface.md#list-screens).

Por exemplo, você pode filtrar pelo cronograma da campanha. Abra o painel de filtro e use a seção **Data de início - término**:

![Filtro de campanha](assets/campaign-filter-on-dates.png)

## O painel de campanha{#campaign-dashboard}

Na guia **Procurar** da lista de campanhas, clique em uma campanha para exibir seus detalhes.

![Painel de campanha](assets/campaign-dashboard.png)

O status e o cronograma da campanha são exibidos na parte superior da tela. Você pode usar o ícone **Definir configurações da campanha** para modificar as propriedades da campanha que foram definidas ao criá-la. Há três botões disponíveis que permitem visualizar logs, relatórios, duplicar ou excluir a campanha. Consulte esta [seção](create-campaigns.md#create-campaigns)

Duas guias estarão disponíveis:

* A guia **Workflows** lista todos os workflows vinculados à campanha. Essa guia também permite criar um novo workflow dentro da campanha. Consulte esta [seção](create-campaigns.md#create-campaigns).

* A guia **Entregas** lista todas as entregas vinculadas à campanha atual. Você também pode criar uma nova entrega dentro da campanha. Consulte esta [seção](create-campaigns.md#create-campaigns).

## Duplicar e excluir uma campanha

É possível duplicar ou excluir uma campanha:

* na lista de campanhas, clique no botão de reticências e clique em **Duplicar** ou **Excluir**.
* na própria campanha, clique no botão **Mais** e selecione **Duplicar** ou **Excluir**.

>[!NOTE]
>
>A guia **Envíos** exibe todas as envíos vinculadas à campanha. No entanto, as entregas criadas em um fluxo de trabalho não podem ser excluídas dali. Para excluir uma entrega criada no contexto de um workflow, será necessário excluir a atividade de entrega do workflow. [Saiba mais](../msg/gs-messages.md#delivery-delete).
