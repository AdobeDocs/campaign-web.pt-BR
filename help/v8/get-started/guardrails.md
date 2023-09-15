---
title: Medidas de proteção e limitações na interface do usuário da Web do Campaign
description: Medidas de proteção e limitações na interface do usuário da Web do Campaign
badge: label="Beta"
source-git-commit: 86d87e9a3ac9028634a08c2c0969cd232dff15f5
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 4%

---


# Medidas de proteção e limitações {#guardrails-limitations}

Ao trabalhar na interface da Web do Campaign com componentes criados ou modificados no console do cliente do Campaign, as medidas de proteção e as limitações listadas abaixo se aplicam.

## Fluxos de trabalho {#wf-guardrails-limitations}

**Activities**

* As atividades de fluxo de trabalho que ainda não são compatíveis na interface do usuário da Web são somente leitura. Você ainda pode executar o fluxo de trabalho, enviar mensagens, verificar os logs etc. As atividades de fluxo de trabalho disponíveis na interface da Web e no console do cliente são editáveis.

| Console | Interface do usuário da Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="50%" align="left" zoomable="yes"} |

**Tela**

* Ao criar um novo fluxo de trabalho na interface da Web, a tela de desenho suporta apenas um ponto de entrada. No entanto, se você criou um workflow no console com vários pontos de entrada,

No entanto, mesmo que o fluxo de trabalho tenha sido criado na tela do console do cliente com vários pontos de entrada, ele também será editável na interface do usuário da Web. Ainda é possível abrir e editar



Para experimentar este cenário, crie um fluxo de trabalho no console do cliente com vários pontos de entrada e abra-o na interface do usuário da Web para ver o resultado.



É claro que você pode editar as atividades e iniciar e executar o workflow como de costume.



**Posicionamento da atividade**

* O posicionamento dos nós será recalculado (o posicionamento inicial das atividades, portanto, será modificado) somente quando uma atividade tiver sido adicionada ou removida (nem sempre).

**Opções não expostas**

* As opções não compatíveis não são exibidas na interface do usuário da Web.

**Loops**

* Os loops ainda não estão disponíveis na interface da Web. Se você criou um workflow incluindo um loop usando o console, não é possível acessá-lo a partir da interface do usuário da Web. Uma mensagem de erro é exibida.

| Console | Interface do usuário da Web |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="50%" align="left" zoomable="yes"} |

**Reconciliação e enriquecimento**

No console do cliente do Campaign, a variável **Enriquecimento** A atividade de pode executar reconciliação e enriquecimento. Na interface da Web do Campaign, os recursos de reconciliação ainda não estão disponíveis. Se você definiu a reconciliação na atividade do console, ela será exibida como uma atividade não compatível na interface do usuário da Web.

* Se a variável **Enriquecimento** no console só realizar um enriquecimento, a variável **Enriquecimento** atividade é exibida na web.
* Se a variável **Enriquecimento** Uma atividade de no console só executa uma reconciliação, uma atividade incompatível é exibida.

## Filtros predefinidos {#filters-guardrails-limitations}

Nessa versão do produto, ao selecionar o público de um delivery ou ao criar um público em um workflow, alguns filtros predefinidos não estão disponíveis na interface do usuário.

Uma mensagem de erro específica é exibida. Mesmo que não seja possível exibir a representação gráfica da consulta no construtor de regras e editar o filtro, você ainda poderá usá-lo, ver as condições de filtragem e os resultados. Você também pode acessar a consulta SQL para verificar as configurações exatas.

![](assets/filter-unavailable.png){width="70%" align="left"}

Observe que, se você criar um filtro na interface da Web e modificá-lo no console com atributos não suportados, a representação gráfica não poderá mais estar disponível na interface da Web. Em qualquer caso, ainda é possível usar o filtro.

Os atributos não compatíveis estão listados abaixo.

### Tipos de dados incompatíveis {#unsupported-data-type}

Os seguintes tipos de dados disponíveis no console do cliente não são compatíveis ao exibir um filtro ou uma regra na interface da Web:

* datetime
* tempo
* timespan
* duplo
* flutuante

### Recursos de filtragem não compatíveis {#unsupported-filtering-capabilities}

Quando um filtro é criado com expressões complexas e funções no console do cliente, ele não pode ser editado na interface da Web.

Além disso, os seguintes operadores não são compatíveis:

* Tipo numérico
   * está incluído em
   * não em

* Tipo de string
   * maior que
   * menor que
   * maior que ou igual a
   * menor que ou igual a
   * curtir
   * não é como

* Tipo de data
   * em ou depois de
   * em ou antes de
   * não é igual
   * está vazio
   * não está vazio
   * está incluído em
   * não está em
   * no(s) último(s)

* Links 1-N
   * CONTAGEM, SOMA, MÉDIA, MÍN, MAX