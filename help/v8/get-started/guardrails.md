---
title: Medidas de proteção e limitações na interface do usuário da Web do Campaign
description: Medidas de proteção e limitações na interface do usuário da Web do Campaign
badge: label="Beta"
source-git-commit: ff95b563784ae507245e6690feedda33ea6a111b
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

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

![](assets/filter-unavailable.png)
