---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 59%

---


# Princípios básicos da criação de fluxos de trabalho {#gs-workflow-creation}

Com o Campaign v8 Web, você pode criar fluxos de trabalho em uma tela visual para projetar processos entre canais, como segmentação, execução de campanha, processamento de arquivos.

Os workflows podem ser criados como workflows independentes, no menu Workflows , ou de dentro de uma campanha, no menu Campaigns .

A ser definido: detalhes específicos entre workflows da campanha e workflows independentes.

## O que há dentro de um fluxo de trabalho?

O diagrama do workflow é uma representação do que deve acontecer. Ele descreve as várias tarefas a serem executadas e como elas são vinculadas.

Cada workflow contém:

* **Activities**: Uma atividade é uma tarefa a ser executada. As várias atividades são representadas no diagrama por ícones. Cada atividade tem propriedades específicas e outras propriedades comuns a todas as atividades.

   Em um diagrama de fluxo de trabalho, uma dada atividade pode produzir várias tarefas, principalmente quando houver as ações de loop ou recorrentes (periódicas).

* **Transições**: As transições vinculam uma atividade de origem a uma atividade de destino e definem sua sequência.

* **Tabelas de trabalho**: as tabelas de trabalho contêm todas as informações transportadas pela transição. Cada fluxo de trabalho usa várias tabelas de trabalho. Os dados transmitidos nessas tabelas podem ser acelerados e usados durante o ciclo de vida do fluxo de trabalho, desde que não sejam eliminados. De fato, tabelas desnecessárias são removidas toda vez que o fluxo de trabalho se torna passivo e possivelmente durante a execução dos maiores workflows para evitar sobrecarga no servidor.

## Etapas principais para criar um fluxo de trabalho

As principais etapas para criar workflows são as seguintes:

A ser definido: gráfico mostrando todo o processo com explicação e referências para páginas doc

criar e definir propriedades > orquestrar atividades na tela > definir configurações, se necessário > iniciar a execução e monitorar