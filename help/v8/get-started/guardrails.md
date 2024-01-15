---
title: Medidas de proteção e limitações na interface do Campaign Web
description: Medidas de proteção e limitações na interface do Campaign Web
badge: label="Beta"
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 3903513d43b699416973b26755dfc4f0337dc757
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 88%

---

# Medidas de proteção e limitações {#guardrails-limitations}

Ao trabalhar na interface do Campaign Web com componentes criados ou modificados no console do cliente do Campaign, as medidas de proteção e as limitações listadas abaixo se aplicam.

## Workflows {#wf-guardrails-limitations}

### Atividades

As atividades de fluxo de trabalho que ainda não são compatíveis com a interface da web são somente leitura e exibidas como atividades incompatíveis. Você ainda pode executar o fluxo de trabalho, enviar mensagens, verificar os logs etc. As atividades de fluxo de trabalho disponíveis na interface da web e no console do cliente são editáveis.

| Console | Interface da web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="800px" align="left" zoomable="yes"} |

As configurações da atividade de fluxo de trabalho que ainda não são compatíveis com a interface da web não são exibidas. No entanto, quando o fluxo de trabalho é executado, essas configurações se aplicam.

| Console | Interface da web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

No console, a atividade **Enriquecimento** pode executar a reconciliação e o enriquecimento. Na interface da web, os recursos de reconciliação ainda não estão disponíveis. Se você tiver definido no console as configurações de reconciliação na atividade de **Enriquecimento**, ela será exibida como uma atividade somente leitura não compatível na interface da web.

| Console | Interface da web |
| --- | --- |
| ![](assets/limitations-options-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){width="800px" align="left" zoomable="yes"} |

### Tela

Ao criar um novo fluxo de trabalho na interface da web, a tela é compatível apenas um ponto de entrada. No entanto, se você criou um fluxo de trabalho no console com vários pontos de entrada, é possível abri-lo e editá-lo na interface da Web.

| Console | Interface da web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){width="800px" align="left" zoomable="yes"} |

Os loops ainda não estão disponíveis na interface da Web. Se você criou um fluxo de trabalho incluindo um loop usando o console, não é possível acessá-lo a partir da interface da web. Uma mensagem de erro é exibida.

| Console | Interface da web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="800px" align="left" zoomable="yes"} |

O posicionamento dos nós é atualizado sempre que uma atividade é adicionada ou removida. Ao criar um fluxo de trabalho no console, modifique-o usando a interface da web e reabra-o no console. Você poderá observar algumas pequenas imperfeições de posicionamento. Isso não afeta os processos e as tarefas do fluxo de trabalho.

| Fluxo de trabalho inicial | Alteração de posicionamento |
| --- | --- |
| ![](assets/limitations-positioning1.png){width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){width="800px" align="left" zoomable="yes"} |

## Filtros predefinidos {#filters-guardrails-limitations}

>[!CONTEXTUALHELP]
>id="acw_predefined_filter_read_only"
>title="Este filtro é somente leitura"
>abstract="Alguns filtros predefinidos não estão disponíveis na interface dessa versão do produto. Esses filtros são marcados como somente leitura. Mesmo que não seja possível exibir a representação gráfica da consulta no modelador de consultas e editar o filtro, ainda será possível usá-lo e ver as condições de filtragem no **Atributos** seção da tela."

Ao selecionar o público-alvo de uma entrega ou criar um público-alvo em um fluxo de trabalho, alguns filtros predefinidos não estarão disponíveis na interface nessa versão do produto. Esses filtros são marcados como somente leitura.

Uma mensagem de erro específica é exibida.

![](assets/filter-unavailable.png){width="70%" align="left"}

Mesmo que não seja possível exibir a representação gráfica da consulta no modelador de consultas e editar o filtro, ainda será possível usá-lo e ver as condições de filtragem no **Atributos** seção da tela.

![](assets/rule-edit.png){width="70%" align="left"}

Você também pode acessar a consulta SQL para verificar as configurações exatas. Para fazer isso, clique em **Visualização de código**.

![](assets/rule-code-view.png){width="70%" align="left"}

Clique em **Calcular** para verificar quantos itens atendem aos critérios do filtro.

![](assets/rule-calculate.png){width="70%" align="left"}

Clique em **Exibir resultados** para exibir esses itens.

![](assets/rule-view-results.png){width="70%" align="left"}

Observe que, se você criar um filtro na interface da web e modificá-lo no console com atributos incompatíveis, a representação gráfica deixará de estar disponível na interface da web. Em qualquer caso, ainda é possível usar o filtro.

Os atributos incompatíveis estão listados abaixo.

### Tipos de dados incompatíveis {#unsupported-data-type}

Os seguintes tipos de dados disponíveis no console do cliente não são compatíveis ao exibir um filtro ou uma regra na interface da web:

* data e hora
* tempo
* intervalo de tempo
* duplo
* flutuante

### Recursos de filtragem incompatíveis {#unsupported-filtering-capabilities}

Quando um filtro é criado com expressões e funções complexas no console do cliente, não pode ser editado na interface da web.

Além disso, os seguintes operadores não são compatíveis:

* Tipo numérico
   * é incluído em
   * não em

* Tipo de string
   * maior que
   * menor que
   * é maior que ou igual a
   * é menor que ou igual a
   * semelhante
   * não semelhante

* Tipo de dados
   * em ou depois de
   * em ou antes de
   * não é igual a
   * está vazio
   * não está vazio
   * é incluído em
   * não está em
   * no último

* links 1-N
   * COUNT, SUM, AVG, MIN, MAX
