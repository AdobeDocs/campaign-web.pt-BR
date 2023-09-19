---
audience: end-user
title: Introdução às campanhas
description: Saiba como começar com as campanhas entre canais
badge: label="Beta"
source-git-commit: a7a7a345e7e01f30516d2925afc46cfe32738aa4
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 72%

---


# Acesso e gerenciamento de suas campanhas{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Programação de campanha"
>abstract="Defina ou modifique a programação da campanha."

Para criar uma nova campanha ou gerenciar suas campanhas já existentes, clique no menu **[!UICONTROL Campanhas]** no painel de navegação esquerdo.

## Lista de campanhas {#access-campaigns}

Na lista de campanhas, duas guias estão disponíveis:

* A guia **Procurar** lista todas as campanhas existentes. É possível clicar em uma campanha para abrir seu painel ou criar uma nova campanha clicando no botão **Criar campanha**. Consulte esta [seção](create-campaigns.md#create-campaigns).

* A guia **Modelos** lista todos os modelos de campanha disponíveis. É possível exibir um modelo existente ou criar um novo. [Leia mais](manage-campaign-templates.md).

![Lista de campanhas](assets/campaign-list.png)

Por padrão, cada campanha da lista exibe informações sobre seu status atual, data de criação, última modificação etc.

É possível personalizar as colunas exibidas clicando no ícone **Configurar coluna para um layout personalizado** localizado no canto superior direito da lista. Isso permite adicionar mais informações à lista. Além disso, uma barra de pesquisa e filtros estão disponíveis para facilitar a pesquisa na lista. [Saiba mais](../get-started/user-interface.md#list-screens).

Por exemplo, você pode filtrar pelo cronograma da campanha. Abra o painel de filtro e use a seção **Data de início - término**:

![Filtro de campanha](assets/campaign-filter-on-dates.png)

## Painel de campanha{#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lista de deliveries na campanha"
>abstract="A guia **Entregas** lista todas as entregas vinculadas à campanha atual. Clique no nome de um delivery para editá-lo. Use o botão Create delivery para adicionar um novo delivery para esta campanha."

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
>A guia **Entrega** exibe todas as entregas vinculadas à campanha. No entanto, as entregas criadas em um fluxo de trabalho não podem ser excluídas dali. Para excluir uma entrega criada no contexto de um workflow, será necessário excluir a atividade de entrega do workflow. [Saiba mais](../msg/gs-messages.md#delivery-delete).

## Trabalhar com modelos de campanha{#manage-campaign-templates}

Os templates de campanha contêm configurações pré-definidas que podem ser reutilizadas para criar novos workflows. Um conjunto de modelos integrados está disponível para ajudar você a começar. Você pode criar e configurar seus modelos de campanha e, em seguida, criar campanhas com base nesses modelos.

Um template de campanha pode armazenar as seguintes informações:

* a campanha **Propriedades** e **Agendar** configurações
* modelos de fluxo de trabalho
* templates do delivery

Para criar um template de campanha, siga as etapas abaixo:

1. Clique em **[!UICONTROL Campanhas]** , navegue até o menu **Modelos** e clique na guia **[!UICONTROL Criar modelo]** botão.
1. Selecione o **Modelo** para usar e fornecer um rótulo para a campanha. Isso permite que você baseie seu novo modelo em um modelo já criado.
1. Se necessário, você pode alterar o seguinte **Opções adicionais**: nome interno, pasta, responsável, descrição e natureza.
1. Defina o **Agendar** da sua campanha. Saiba como definir a programação da campanha no [nesta seção](create-campaigns.md#campaign-schedule)
1. Clique em **Create**.
1. Adicione workflows e templates de delivery à sua campanha.
