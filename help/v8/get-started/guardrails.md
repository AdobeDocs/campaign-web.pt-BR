---
title: Medidas de proteção e limitações nos workflows da interface do Campaign Web
description: Medidas de proteção e limitações ao trabalhar com workflows na interface do Campaign Web
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 56%

---

# Medidas de proteção e limitações para workflows {#guardrails-limitations}

As medidas de proteção e limitações listadas abaixo se aplicam ao trabalhar na interface do Campaign Web com fluxos de trabalho criados ou modificados no console do cliente do Campaign.

Observe que, embora esta página forneça infomações importantes sobre o uso de fluxos de trabalho no console e na interface web, ela não abrange todas as possíveis incompatibilidades entre as duas interfaces.

## Atividades de fluxos de trabalho {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Atividade não editável"
>abstract="Quando uma atividade de **Consulta** ou **Enriquecimento** é configurada com dados adicionais no console, os dados de enriquecimento são levados em consideração no Campaign Web e transmitidos para a transição de saída, mas não podem ser editados."

As atividades de fluxo de trabalho que ainda não são compatíveis com a interface do Campaign Web são somente leitura e exibidas como atividades incompatíveis. Você ainda pode executar o fluxo de trabalho, enviar mensagens, verificar os logs e executar outras tarefas. As atividades de fluxo de trabalho que estão disponíveis na interface do Campaign Web e no console do cliente do Campaign podem ser editadas.

| Console | Web |
| --- | --- |
| ![Captura de tela mostrando limitações de atividades no console](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela mostrando limitações de atividades na interface da Web](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Quando uma atividade de **Consulta** ou **Enriquecimento** é configurada com dados adicionais no console, os dados de enriquecimento são levados em consideração no Campaign Web e transmitidos para a transição de saída, mas não podem ser editados.

| Console | Web |
| --- | --- |
| ![Captura de tela mostrando limitações de opções no console](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela mostrando limitações de opções na interface da Web](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

No console, a atividade **Enriquecimento** pode executar a reconciliação e o enriquecimento. Se você tiver definido as configurações de reconciliação na atividade **Enrichment** no console do cliente, ela será exibida como uma atividade **Reconciliation** na interface do usuário da Web do Campaign.

| Console | Web |
| --- | --- |
| ![Captura de tela mostrando a atividade de enriquecimento no console](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela mostrando a atividade de enriquecimento na interface da Web](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Tela de fluxo de trabalho {#wkf-canvas}

Ao criar um novo fluxo de trabalho na interface do Campaign Web, a tela permite apenas um ponto de entrada. No entanto, se você criou um workflow no console com vários pontos de entrada, é possível abri-lo e editá-lo na interface do usuário da Web do Campaign.

| Console | Web |
| --- | --- |
| ![Captura de tela mostrando vários pontos de entrada no console](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela mostrando vários pontos de entrada na interface da Web](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

O posicionamento dos nós é atualizado sempre que uma atividade é adicionada ou removida. Se você criar um fluxo de trabalho no console, modificá-lo usando a interface da Web do Campaign e reabri-lo no console, poderá observar algumas pequenas imperfeições de posicionamento. Isso não afeta os processos e as tarefas do fluxo de trabalho.

| Fluxo de trabalho inicial | Alteração de posicionamento |
| --- | --- |
| ![Captura de tela mostrando o posicionamento inicial do fluxo de trabalho](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela mostrando alterações de posicionamento após modificações](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |