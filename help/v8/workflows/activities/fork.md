---
audience: end-user
title: Usar a atividade de fluxo de trabalho Bifurcação
description: Saiba como usar a atividade de fluxo de trabalho Bifurcação
badge: label="Beta"
source-git-commit: 4b005f3feb70b8c5cf0f4cd9c5ba54547bd9261a
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 71%

---


# Bifurcação {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Bifurcação Bifurcação"
>abstract="A variável **Bifurcar** a atividade é um **Controle de fluxo** atividade. Ele permite criar transições de saída para iniciar várias atividades ao mesmo tempo."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Bifurcação Bifurcação"
>abstract="A atividade Bifurcação permite criar transições de saída para iniciar várias atividades ao mesmo tempo."

A variável **Bifurcar** a atividade é um **Controle de fluxo** atividade. Ele permite criar transições de saída para iniciar várias atividades ao mesmo tempo.

## Configuração

Siga estas etapas para configurar a atividade de **Bifurcação**:

1. Adicione uma atividade de **Bifurcação** ao seu fluxo de trabalho.
1. Clique em **Adicionar transição** para adicionar uma nova transição de saída. Por padrão, são definidas duas transições.
1. Adicione um rótulo a cada transição.

## Exemplo

No exemplo a seguir, estaremos usando duas atividades de **Bifurcação**:

* Uma antes das duas consultas, para executá-las ao mesmo tempo.
* Uma após a interseção, para enviar um email e um SMS simultaneamente à população direcionada.

![](../assets/workflow-fork-example.png)

