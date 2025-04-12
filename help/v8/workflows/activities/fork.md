---
audience: end-user
title: Usar a atividade de fluxo de trabalho Bifurcação
description: Saiba como usar a atividade de fluxo de trabalho Bifurcação
exl-id: 5c7ff58b-5504-4b8e-879f-44754b7dcf8a
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 55%

---


# Bifurcação {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Atividade Bifurcação"
>abstract="A atividade **Bifurcação** permite criar transições de saída para iniciar várias atividades ao mesmo tempo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Transições da atividade bifurcação"
>abstract="Por padrão, duas transições são criadas com uma atividade **Bifurcação**. Clique em **Adicionar transição** para definir uma transição de saída adicional e insira seu rótulo."

A atividade **Bifurcação** é uma atividade de **Controle de fluxo**. Ela permite criar transições de saída para iniciar várias atividades simultaneamente.

## Configurar a atividade de bifurcação {#fork-configuration}

Siga estas etapas para configurar a atividade de **Bifurcação**:

![Captura de tela de configuração da atividade de bifurcação do fluxo de trabalho](../assets/workflow-fork.png)

1. Adicione uma atividade de **Bifurcação** ao seu fluxo de trabalho.
1. Clique em **Adicionar transição** para adicionar uma nova transição de saída. Por padrão, duas transições são definidas.
1. Adicione um rótulo a cada transição.

## Exemplo {#fork-example}

No exemplo a seguir, duas atividades **Fork** são usadas:

* Uma antes das duas queries, para executá-las simultaneamente.
* Uma após a interseção, para enviar um email e um SMS ao mesmo tempo à população direcionada.

![Captura de tela de exemplo de bifurcação de fluxo de trabalho](../assets/workflow-fork-example.png)
