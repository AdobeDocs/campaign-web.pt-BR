---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 17%

---

# Acessar e gerenciar fluxos de trabalho {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Fluxos de trabalho"
>abstract="Nesta tela, você pode acessar a lista completa de fluxos de trabalho independentes e da campanha, verificar o status atual, as datas de última/próxima execução e criar um novo fluxo de trabalho. Navegue até a guia “Modelos” para acessar os modelos de fluxo de trabalho disponíveis."

O menu **[!UICONTROL Fluxos de trabalho]** fornece acesso à lista completa de fluxos de trabalho. Esta lista inclui **fluxos de trabalho autônomos**, criados nesta tela, e **fluxos de trabalho da campanha**, criados em uma campanha.

![Tela da lista de fluxos de trabalho mostrando fluxos de trabalho independentes e de campanha](assets/workflow-list.png){zoomable="yes"}

Cada fluxo de trabalho na lista exibe informações sobre seu [status](#status) atual, a última vez que foi executado ou modificado e a data e hora da próxima execução agendada.

Personalize as colunas exibidas clicando no ícone **[!UICONTROL Configurar coluna para um layout personalizado]** localizado no canto superior direito da lista. Isso permite adicionar mais informações à lista, como a última atividade com erro para cada workflow ou o targeting dimension aplicado.

Além disso, uma barra de pesquisa e filtros estão disponíveis para simplificar a pesquisa na lista. Por exemplo, filtre os workflows para exibir somente aqueles pertencentes a uma campanha ou aqueles processados durante um intervalo de datas específico.

Para duplicar ou excluir um fluxo de trabalho, clique no botão de reticências e selecione **[!UICONTROL Duplicar]** ou **[!UICONTROL Excluir]**.

>[!NOTE]
>
>É possível duplicar um workflow em andamento, mas não excluí-lo.

## Status dos fluxos de trabalho {#status}

Os workflows podem ter vários status:

* **[!UICONTROL Rascunho]**: o fluxo de trabalho foi criado e salvo.
* **[!UICONTROL Em andamento]**: o fluxo de trabalho está em execução atualmente.
* **[!UICONTROL Concluído]**: a execução do fluxo de trabalho foi concluída.
* **[!UICONTROL Pausado]**: fluxo de trabalho pausado.
* **[!UICONTROL Erro]**: o fluxo de trabalho encontrou um erro. Abra o workflow e acesse os logs e as tarefas para identificar o erro e resolvê-lo. [Saiba como monitorar logs e tarefas](start-monitor-workflows.md#logs-tasks)

Informações detalhadas sobre como iniciar e monitorar a execução do fluxo de trabalho estão disponíveis em [esta página](start-monitor-workflows.md).

## Templates de workflow {#templates}

A guia **[!UICONTROL Modelos]** lista todos os modelos de fluxo de trabalho disponíveis.

Os templates de workflow contêm atividades pré-configuradas e configurações gerais de propriedade que podem ser reutilizadas para criar novos workflows.

Crie modelos de fluxo de trabalho a partir de um fluxo de trabalho existente ou do zero. [Saiba como criar modelos de fluxo de trabalho](create-workflow.md#workflow-templates)