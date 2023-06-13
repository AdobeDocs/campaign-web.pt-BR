---
audience: end-user
title: Usar a atividade de workflow Fork
description: Saiba como usar a atividade de workflow Fork
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 19%

---


# Bifurcação {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Bifurcação atividade"
>abstract="A atividade Fork permite criar transições de saída para iniciar várias atividades ao mesmo tempo."

## Configuração

Siga estas etapas para configurar o **Bifurcar** atividade:

1. Adicionar um **Bifurcar** atividade ao seu fluxo de trabalho.
1. Clique em **Adicionar transição** para adicionar uma nova transição de saída. Por padrão, duas transições são definidas.
1. Adicione um rótulo a cada transição.

## Exemplo

O exemplo a seguir, estamos usando dois **Bifurcar** atividades:

* Uma antes das duas queries, para executá-las ao mesmo tempo.
* Um após a interseção, para enviar um email e um SMS simultaneamente à população direcionada.

![](../assets/workflow-fork-example.png)

