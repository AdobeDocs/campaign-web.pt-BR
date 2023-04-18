---
audience: end-user
title: Criar workflows com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com a Web Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 9a4ca68d475cfbbcccb7a5b0d84f841589824288
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Princípios básicos da criação de workflow {#gs-workflow-creation}

Um workflow é uma definição de processo: o diagrama do workflow, que é uma representação do que deveria acontecer. Um workflow também é uma instância desse processo: uma instância de workflow, que é uma representação do que está realmente acontecendo.

O template de workflow descreve as várias tarefas a serem executadas e como elas são vinculadas. Os templates de tarefa são chamados de atividades e são representados por ícones. Eles são vinculados por transições.

captura de tela TBD

## O que há dentro de um fluxo de trabalho?

Cada workflow contém:

* **Activities**: Uma atividade descreve um template de tarefa. As várias atividades disponíveis são representadas no diagrama por ícones. Cada tipo tem propriedades comuns e específicas.

   Em um diagrama de workflow, uma determinada atividade pode produzir várias tarefas, principalmente quando há ações de loop ou recorrentes.

* **Transições**: As transições permitem vincular atividades e definir sua sequência. Uma transição vincula uma atividade de origem a uma atividade de destino.

* **Worktables**: O worktable contém todas as informações transportadas pela transição. Cada fluxo de trabalho usa várias tabelas de trabalho. Os dados transmitidos nessas tabelas podem ser acelerados e usados no ciclo de vida do workflow, desde que não sejam apagados. De fato, tabelas desnecessárias são removidas toda vez que o workflow se torna passivo e possivelmente durante a execução dos maiores workflows para evitar sobrecarga no servidor.

## Workflows autônomos e de campanha

Os workflows podem ser criados como workflows independentes ou de dentro de uma campanha.

TBD: detalhes específicos entre workflows independentes e de campanha.

## Etapas principais para criar um workflow

As principais etapas para criar workflows são as seguintes:

TBD: gráfico mostrando todo o processo com explicação e ref para páginas doc