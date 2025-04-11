---
audience: end-user
title: Princípios básicos da criação de fluxos de trabalho
description: Conheça os princípios básicos dos fluxos de trabalho no Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 41%

---

# Princípios básicos da criação de fluxos de trabalho {#gs-workflow-creation}

Com o Adobe Campaign Web, você pode criar fluxos de trabalho em uma tela visual para projetar processos entre canais, como segmentação, execução de campanha e processamento de arquivos.

## O que há dentro de um workflow? {#gs-workflow-inside}

O diagrama de workflow representa o processo planejado. Ele descreve as várias tarefas a serem executadas e como elas estão vinculadas.

![Diagrama de exemplo de fluxo de trabalho mostrando tarefas e suas conexões](assets/workflow-example.png){zoomable="yes"}

Cada fluxo de trabalho contém:

* **Atividades**: uma atividade é uma tarefa a ser executada. Os ícones no diagrama representam as várias atividades. Cada atividade tem propriedades específicas e propriedades comuns a todas as atividades.

  Em um diagrama de workflow, uma determinada atividade pode produzir várias tarefas, especialmente quando há um loop ou ações recorrentes.

* **Transições**: as transições vinculam uma atividade de origem a uma atividade de destino e definem sua sequência.

* **Tabelas de trabalho**: as tabelas de trabalho contêm todas as informações transportadas pela transição. Cada fluxo de trabalho usa várias tabelas de trabalho. Os dados nessas tabelas podem ser usados durante o ciclo de vida do workflow.

## Etapas principais para criar um fluxo de trabalho {#gs-workflow-steps}

As campanhas oferecem duas maneiras de criar um fluxo de trabalho:

1. Os fluxos de trabalho podem ser criados como fluxos de trabalho independentes no menu **Fluxos de trabalho**.

   ![Captura de tela da interface para criar um fluxo de trabalho autônomo](assets/create-a-standalone-wf.png){zoomable="yes"}

1. Os fluxos de trabalho podem ser criados diretamente em uma campanha a partir da guia **Workflow** da campanha. Quando incluído em uma campanha, o fluxo de trabalho é executado junto com todos os outros fluxos de trabalho da campanha e as métricas de relatório são agrupadas no nível da campanha.

   ![Captura de tela da interface para criar um fluxo de trabalho em uma campanha](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

Estas são as principais etapas para criar fluxos de trabalho:

![Diagrama mostrando o processo de criação do fluxo de trabalho](assets/workflow-creation-process.png){zoomable="yes"}

Essas etapas estão detalhadas nas seguintes seções:

1. [Criar o fluxo de trabalho e definir suas propriedades](create-workflow.md)
1. [Orquestrar e configurar atividades](orchestrate-activities.md)
1. [Definir as configurações avançadas do fluxo de trabalho](workflow-settings.md)
1. [Inicie o fluxo de trabalho e monitore sua execução](start-monitor-workflows.md)