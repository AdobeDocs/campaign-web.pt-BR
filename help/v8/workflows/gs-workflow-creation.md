---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alpha"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 76%

---


# Princípios básicos da criação de workflows {#gs-workflow-creation}

Com o Campaign v8 Web, é possível criar workflows em uma tela visual para projetar processos entre canais, como segmentação, execução de campanha e processamento de arquivos.

Os workflows podem ser criados como workflows independentes, no menu Workflows, ou diretamente em uma campanha. Nesse caso, o workflow será vinculado à campanha e executado junto com todos os outros workflows da campanha.

## O que há dentro de um workflow?

O diagrama de workflow é uma representação do que deveria acontecer. Ele descreve as várias tarefas a serem executadas e como elas estão vinculadas.

![](assets/workflow-example.png)

Cada workflow contém:

* **Activities**: uma atividade é uma tarefa a ser executada. As várias atividades são representadas no diagrama por ícones. Cada atividade tem propriedades específicas e outras propriedades que são comuns a todas as atividades.

  Em um diagrama de workflow, uma dada atividade pode produzir várias tarefas, principalmente quando houver ações de loop ou recorrentes.

* **Transições**: as transições vinculam uma atividade de origem a uma atividade de destino e definem sua sequência.

* **Tabelas de trabalho**: as tabelas de trabalho contêm todas as informações transportadas pela transição. Cada fluxo de trabalho usa várias tabelas de trabalho. Os dados transmitidos nessas tabelas podem ser usados durante o ciclo de vida do workflow.

## Etapas principais para criar um fluxo de trabalho

As principais etapas para criar workflows são as seguintes:

![](assets/workflow-creation-process.png)
