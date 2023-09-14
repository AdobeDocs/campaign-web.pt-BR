---
title: Medidas de proteção e limitações na interface do usuário da Web do Campaign
description: Medidas de proteção e limitações na interface do usuário da Web do Campaign
badge: label="Beta"
source-git-commit: 2ce9dc99fd88f4731ed0d5ac934e66d4934a2c02
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 5%

---


# Medidas de proteção e limitações {#guardrails-limitations}

Ao trabalhar na interface da Web do Campaign com componentes criados ou modificados no console do cliente do Campaign, as medidas de proteção e as limitações listadas abaixo se aplicam.

## Fluxos de trabalho {#wf-guardrails-limitations}

O mesmo workflow pode ser acessado no console e na interface do usuário da Web. No entanto, esteja ciente de que determinadas limitações se aplicam.

**Edição de atividade**

* Ao acessar um workflow de console na interface do usuário da Web, você só pode modificar atividades compatíveis.

**Edição da tela de desenho**

* Se um workflow de console tiver vários nós/ramificações iniciais ou atividades flutuantes, será necessário adicionar uma atividade inicial e uma bifurcação para conectar os nós iniciais ao nó principal. Você também precisa remover as atividades flutuantes.

**Posicionamento da atividade**

* O posicionamento dos nós será recalculado (o posicionamento inicial das atividades, portanto, será modificado) somente quando uma atividade tiver sido adicionada ou removida (nem sempre).

**Opções não expostas**

* As opções não compatíveis não são exibidas na interface do usuário da Web.

**Loops**

* Os fluxos de trabalho que incluem loops não são exibidos na interface do usuário da Web. Uma mensagem de erro é exibida.

**Reconciliação e enriquecimento**

No console do cliente do Campaign, a variável **Enriquecimento** A atividade de pode executar reconciliação e enriquecimento. Na interface da Web do Campaign, os recursos de reconciliação ainda não estão disponíveis. Se você definiu a reconciliação na atividade do console, ela será exibida como uma atividade não compatível na interface do usuário da Web.

* Se a variável **Enriquecimento** no console só realizar um enriquecimento, a variável **Enriquecimento** atividade é exibida na web.
* Se a variável **Enriquecimento** Uma atividade de no console só executa uma reconciliação, uma atividade incompatível é exibida.

## Filtros predefinidos {#filters-guardrails-limitations}

Ao selecionar o público de uma entrega ou ao criar um público em um fluxo de trabalho, alguns filtros predefinidos não estão disponíveis. Uma mensagem de erro específica é exibida. Você ainda pode usar a consulta e ver: a condição de filtragem e os resultados, mas não pode visualizar a consulta exata no construtor de regras e não pode editar o filtro.

![](assets/filter-unavailable.png){width="70%" align="left"}


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