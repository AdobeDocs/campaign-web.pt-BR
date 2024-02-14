---
title: Medidas de proteção e limitações nos workflows da interface da Web do Campaign
description: Medidas de proteção e limitações ao trabalhar com workflows na interface do usuário da Web do Campaign
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 19864179f02d39583cc90d42bf6ab677f4841600
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 19%

---

# Medidas de proteção e limitações para fluxos de trabalho {#guardrails-limitations}

Ao trabalhar na interface do usuário da Web do Campaign com workflows criados ou modificados no console do cliente do Campaign, as medidas de proteção e as limitações listadas abaixo se aplicam.

Observe que, embora esta página identifique as principais considerações ao trabalhar com workflows no console e na interface do usuário da Web, ela não abrange todas as incompatibilidades potenciais entre as duas interfaces.

## Atividades de fluxos de trabalho {#wkf-activities}

As atividades de workflow ainda não compatíveis na Web do Campaign são somente leitura e exibidas como atividades incompatíveis. Você ainda pode executar o fluxo de trabalho, enviar mensagens, verificar os logs etc. As atividades de workflow disponíveis na Web do Campaign e no console do cliente são editáveis.

As atividades de fluxo de trabalho que ainda não são compatíveis com a interface da Web do Campaign são somente leitura e exibidas como atividades incompatíveis. Você ainda pode executar o fluxo de trabalho, enviar mensagens, verificar os logs etc. As atividades de workflow disponíveis na interface da Web do Campaign e no console do cliente do Campaign podem ser editadas.

| Console | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Quando um **Query** ou um **Enriquecimento** for configurada com dados adicionais no console, os dados de enriquecimento serão considerados no Campaign Web e transmitidos para a transição de saída, mas não poderão ser editados.

| Console | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

No console, a atividade **Enriquecimento** pode executar a reconciliação e o enriquecimento. Se você tiver definido, no console do cliente, as configurações de reconciliação no **Enriquecimento** atividade, será exibido como um **Reconciliação** atividade na interface da Web do Campaign.

| Console | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

## Tela de fluxo de trabalho {#wkf-canvas}

Ao criar um novo workflow na interface da Web do Campaign, a tela oferece suporte apenas a um ponto de entrada. No entanto, se você criou um fluxo de trabalho no console com vários pontos de entrada, é possível abri-lo e editá-lo na interface do usuário da Web do Campaign.

| Console | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

O posicionamento dos nós é atualizado sempre que uma atividade é adicionada ou removida. Se você criar um fluxo de trabalho no console, modificá-lo usando a interface da Web do Campaign e reabri-lo no console, poderá notar algumas pequenas imperfeições de posicionamento. Isso não afeta os processos e as tarefas do fluxo de trabalho.

| Fluxo de trabalho inicial | Alteração de posicionamento |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoom=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |
