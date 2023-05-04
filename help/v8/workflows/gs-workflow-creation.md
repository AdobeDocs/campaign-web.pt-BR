---
audience: end-user
title: Criar workflows com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com a Web Adobe Campaign
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 11%

---


# Princípios básicos da criação de workflow {#gs-workflow-creation}

Com o Campaign v8 Web, você pode criar fluxos de trabalho em uma tela visual para projetar processos entre canais, como segmentação, execução de campanha, processamento de arquivos.

Os workflows podem ser criados como workflows independentes, no menu Workflows , ou de dentro de uma campanha, no menu Campaigns .

TBD: detalhes específicos entre workflows independentes e de campanha.

## O que há dentro de um fluxo de trabalho?

O diagrama do workflow é uma representação do que deve acontecer. Ele descreve as várias tarefas a serem executadas e como elas são vinculadas.

Cada workflow contém:

* **Activities**: Uma atividade é uma tarefa a ser executada. As várias atividades são representadas no diagrama por ícones. Cada atividade tem propriedades específicas e outras propriedades comuns a todas as atividades.

   Em um diagrama de workflow, uma determinada atividade pode produzir várias tarefas, principalmente quando há ações de loop ou recorrentes.

* **Transições**: As transições vinculam uma atividade de origem a uma atividade de destino e definem sua sequência.

* **Worktables**: O worktable contém todas as informações transportadas pela transição. Cada fluxo de trabalho usa várias tabelas de trabalho. Os dados transmitidos nessas tabelas podem ser acelerados e usados no ciclo de vida do workflow, desde que não sejam apagados. De fato, tabelas desnecessárias são removidas toda vez que o workflow se torna passivo e possivelmente durante a execução dos maiores workflows para evitar sobrecarga no servidor.

## Etapas principais para criar um workflow

As principais etapas para criar workflows são as seguintes:

TBD: gráfico mostrando todo o processo com explicação e ref para páginas doc

criar e definir propriedades > orquestrar atividades na tela > definir configurações, se necessário > iniciar a execução e monitorar