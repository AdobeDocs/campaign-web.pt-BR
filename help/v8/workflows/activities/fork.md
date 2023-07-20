---
audience: end-user
title: Usar a atividade de fluxo de trabalho Bifurcação
description: Saiba como usar a atividade de fluxo de trabalho Bifurcação
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '110'
ht-degree: 100%

---


# Bifurcação {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Atividade de   Bifurcação"
>abstract="A atividade Bifurcação permite criar transições de saída para iniciar várias atividades ao mesmo tempo."

## Configuração

Siga estas etapas para configurar a atividade de **Bifurcação**:

1. Adicione uma atividade de **Bifurcação** ao seu fluxo de trabalho.
1. Clique em **Adicionar transição** para adicionar uma nova transição de saída. Por padrão, são definidas duas transições.
1. Adicione um rótulo a cada transição.

## Exemplo

No exemplo a seguir, estamos usando duas atividades de **Bifurcação**:

* Uma antes das duas consultas, para executá-las ao mesmo tempo.
* Uma após a interseção, para enviar um email e um SMS simultaneamente à população direcionada.

![](../assets/workflow-fork-example.png)

