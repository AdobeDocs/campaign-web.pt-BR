---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alfa"
exl-id: 51648665-8400-426c-85cf-dbf5f4f81d20
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 15%

---

# Acessar e gerenciar workflows {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Fluxos de trabalho"
>abstract="Nesta tela, você pode acessar a lista completa de workflows independentes e da campanha, verificar o status atual, as datas de última/próxima execução e criar um novo workflow. Navegue até a guia “Modelos” para acessar os modelos de fluxo de trabalho disponíveis."

A variável **[!UICONTROL Fluxos de trabalho]** permite acessar a lista completa de workflows. Esta lista inclui **workflows independentes** que foram criados nessa tela, e **workflows da campanha**, que foram criados em uma campanha.

![](assets/workflow-list.png)

Cada workflow na lista exibe informações sobre seu workflow atual [status](#status), a última vez que foi executada ou modificada e a data e hora da próxima execução programada.

É possível personalizar as colunas exibidas clicando no ícone **[!UICONTROL Configurar coluna para layout personalizado]** ícone localizado no canto superior direito da lista. Isso permite adicionar mais informações à lista, como a última atividade com erro para cada workflow ou o targeting dimension aplicado.

Além disso, uma barra de pesquisa e filtros estão disponíveis para facilitar a pesquisa na lista. Por exemplo, você pode filtrar os workflows para exibir apenas aqueles pertencentes a uma campanha ou aqueles processados durante um intervalo de datas específico.

Para duplicar ou excluir um workflow, clique no botão de reticências e selecione **[!UICONTROL Duplicar]** ou **[!UICONTROL Excluir]**.

>[!NOTE]
>
>É possível duplicar um workflow em andamento, mas não excluí-lo.

## Status dos fluxos de trabalho {#status}

Os workflows podem ter vários status:

* **[!UICONTROL Rascunho]**: o workflow foi criado e salvo.
* **[!UICONTROL Em andamento]**: o workflow está em execução no momento.
* **[!UICONTROL Concluído]**: a execução do workflow está concluída.
* **[!UICONTROL Pausado]**: o workflow foi pausado.
* **[!UICONTROL Errado]**: o workflow encontrou um erro. Abra o workflow e acesse os logs e as tarefas para identificar o erro e resolvê-lo. [Saiba como monitorar logs e tarefas](start-monitor-workflows.md#logs-tasks)

Informações detalhadas sobre como iniciar e monitorar a execução do workflow estão disponíveis em [esta página](start-monitor-workflows.md).

## Templates de workflow {#templates}

A variável **[!UICONTROL Modelos]** A guia lista todos os modelos de fluxos de trabalho disponíveis.

Os templates de workflow contêm atividades pré-configuradas e configurações gerais de propriedade que podem ser reutilizadas para criar novos workflows. Eles são criados no console cliente. [Saiba como trabalhar com modelos](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)
