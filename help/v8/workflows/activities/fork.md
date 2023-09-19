---
audience: end-user
title: Usar a atividade de fluxo de trabalho Bifurcação
description: Saiba como usar a atividade de fluxo de trabalho Bifurcação
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 66%

---


# Bifurcação {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Bifurcação Bifurcação"
>abstract="A atividade **Bifurcação** permite criar transições de saída para iniciar várias atividades ao mesmo tempo."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transições de atividade de bifurcação"
>abstract="Por padrão, duas transições são criadas com um **Bifurcar** atividade. Clique em **Adicionar transição** para definir uma transição de saída adicional e insira seu rótulo."

A variável **Bifurcar** a atividade é um **Controle de fluxo** atividade. Ele permite criar transições de saída para iniciar várias atividades ao mesmo tempo.

## Configurar a atividade de bifurcação{#fork-configuration}

Siga estas etapas para configurar a atividade de **Bifurcação**:

![](../assets/workflow-fork.png)

1. Adicione uma atividade de **Bifurcação** ao seu fluxo de trabalho.
1. Clique em **Adicionar transição** para adicionar uma nova transição de saída. Por padrão, são definidas duas transições.
1. Adicione um rótulo a cada transição.

## Exemplo{#fork-example}

No exemplo a seguir, estaremos usando duas atividades de **Bifurcação**:

* Uma antes das duas consultas, para executá-las ao mesmo tempo.
* Uma após a interseção, para enviar um email e um SMS simultaneamente à população direcionada.

![](../assets/workflow-fork-example.png)

