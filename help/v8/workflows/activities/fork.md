---
audience: end-user
title: Usar a atividade de workflow Fork
description: Saiba como usar a atividade de workflow Fork
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 5%

---


# Bifurcação {#fork}

A variável **Bifurcar** permite criar transições de saída para iniciar várias atividades ao mesmo tempo.

A variável **Bifurcar** A atividade de permite realizar várias atividades diferentes de maneira independente no mesmo fluxo de trabalho.

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

