---
title: Medidas de proteção e limitações nos fluxos de trabalho da interface do Campaign Web
description: Medidas de proteção e limitações ao trabalhar com fluxos de trabalho na interface do Campaign Web
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 100%

---

# Medidas de proteção e limitações para fluxos de trabalho {#guardrails-limitations}

As medidas de proteção e limitações listadas abaixo se aplicam ao trabalhar na interface do Campaign Web com fluxos de trabalho criados ou modificados no console do cliente do Campaign.

Observe que, embora esta página forneça infomações importantes sobre o uso de fluxos de trabalho no console e na interface web, ela não abrange todas as possíveis incompatibilidades entre as duas interfaces.

## Atividades de fluxos de trabalho {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Atividade não editável"
>abstract="Quando uma atividade de **Consulta** ou **Enriquecimento** é configurada com dados adicionais no console, os dados de enriquecimento são levados em consideração no Campaign Web e transmitidos para a transição de saída, mas não podem ser editados."

As atividades de fluxo de trabalho que ainda não são compatíveis com a interface do Campaign Web são somente leitura e exibidas como atividades incompatíveis. Ainda é possível executar o fluxo de trabalho, enviar mensagens, verificar os logs e realizar outras tarefas. As atividades de fluxo de trabalho que estão disponíveis na interface do Campaign Web e no console do cliente do Campaign podem ser editadas.

| Console | Web |
| --- | --- |
| ![Captura de tela que mostra as limitações de atividades no console](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela que mostra as limitações de atividades na interface web](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Quando uma atividade de **Consulta** ou **Enriquecimento** é configurada com dados adicionais no console, os dados de enriquecimento são levados em consideração no Campaign Web e transmitidos para a transição de saída, mas não podem ser editados.

| Console | Web |
| --- | --- |
| ![Captura de tela que mostra as limitações de opções no console](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela que mostra as limitações de opções na interface web](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

No console, a atividade **Enriquecimento** pode executar a reconciliação e o enriquecimento. Se você tiver ajustado as configurações de reconciliação da atividade de **Enriquecimento** no console do cliente, ela será exibida como uma atividade de **Reconciliação** na interface web do Campaign.

| Console | Web |
| --- | --- |
| ![Captura de tela que mostra a atividade de enriquecimento no console](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela que mostra a atividade de enriquecimento na interface web](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Tela de fluxo de trabalho {#wkf-canvas}

Ao criar um novo fluxo de trabalho na interface do Campaign Web, a tela permite apenas um ponto de entrada. No entanto, se você tiver criado um fluxo de trabalho no console com vários pontos de entrada, será possível abri-lo e editá-lo na interface web do Campaign.

| Console | Web |
| --- | --- |
| ![Captura de tela que mostra os vários pontos de entrada no console](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela que mostra os vários pontos de entrada na interface web](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

O posicionamento dos nós é atualizado sempre que uma atividade é adicionada ou removida. Se você criar um fluxo de trabalho no console, modificá-lo por meio da interface web do Campaign e reabri-lo no console, será possível observar alguns pequenos erros de posicionamento. Isso não afeta os processos e as tarefas do fluxo de trabalho.

| Fluxo de trabalho inicial | Alteração do posicionamento |
| --- | --- |
| ![Captura de tela que mostra o posicionamento inicial do fluxo de trabalho](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![Captura de tela que mostra as alterações do posicionamento após modificações](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |