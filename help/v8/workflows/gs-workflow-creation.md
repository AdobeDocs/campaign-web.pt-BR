---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 53148300ecb5d52d89875519c44ae979d29a4d76
workflow-type: ht
source-wordcount: '281'
ht-degree: 100%

---


# Princípios básicos da criação de workflows {#gs-workflow-creation}

Com o Campaign v8 Web, é possível criar workflows em uma tela visual para projetar processos entre canais, como segmentação, execução de campanha e processamento de arquivos.


## O que há dentro de um workflow? {#gs-workflow-inside}

O diagrama de workflow é uma representação do que deveria acontecer. Ele descreve as várias tarefas a serem executadas e como elas estão vinculadas.

![](assets/workflow-example.png)

Cada workflow contém:

* **Activities**: uma atividade é uma tarefa a ser executada. As várias atividades são representadas no diagrama por ícones. Cada atividade tem propriedades específicas e outras propriedades que são comuns a todas as atividades.

  Em um diagrama de workflow, uma dada atividade pode produzir várias tarefas, principalmente quando houver ações de loop ou recorrentes.

* **Transições**: as transições vinculam uma atividade de origem a uma atividade de destino e definem sua sequência.

* **Tabelas de trabalho**: as tabelas de trabalho contêm todas as informações transportadas pela transição. Cada fluxo de trabalho usa várias tabelas de trabalho. Os dados transmitidos nessas tabelas podem ser usados durante o ciclo de vida do fluxo de trabalho.

## Etapas principais para criar um fluxo de trabalho {#gs-workflow-steps}


As campanhas oferecem duas maneiras de criar um fluxo de trabalho:

1. Os fluxos de trabalho podem ser criados como independentes, a partir do menu **Fluxos de trabalho**.

   ![](assets/create-a-standalone-wf.png)

1. Os fluxos de trabalho podem ser criados diretamente em uma campanha, a partir da guia **Fluxo de trabalho** da campanha. Quando incluído em uma campanha, o fluxo de trabalho é executado em conjunto com todos os outros fluxos de trabalho da campanha e as métricas de relatório são agrupadas no nível da campanha.

   ![](assets/create-a-wf-from-a-campaign.png)


Estas são as principais etapas para criar fluxos de trabalho:

![](assets/workflow-creation-process.png)

Essas etapas estão detalhadas na seguinte seção:

1. [Criar o fluxo de trabalho e definir suas propriedades](create-workflow.md)
1. [Orquestrar e configurar atividades](orchestrate-activities.md)
1. [Definir as configurações avançadas do fluxo de trabalho](workflow-settings.md)
1. [Inicie o fluxo de trabalho e monitore sua execução](start-monitor-workflows.md)

