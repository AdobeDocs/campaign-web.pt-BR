---
audience: end-user
title: Usar a atividade de workflow Aguardar
description: Saiba como usar a atividade de workflow Aguardar
badge: label="Alpha" type="Positive"
source-git-commit: 12d87baff81298583fac12fdf04d39997e875954
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 42%

---


# Aguardar {#wait}

A variável **Aguardar** A atividade suspende temporariamente a execução de uma parte do fluxo de trabalho. Ela ativa a transição de saída após um atraso que pode variar de alguns segundos a vários meses, o que executa as atividades colocadas depois.

A variável **Aguardar** A atividade é usada para permitir que um determinado período transcorra entre duas atividades que estão sendo executadas. Por exemplo, a espera de vários dias após uma atividade de delivery de email para depois analisar as aberturas e os cliques gerados durante esse período antes de executar qualquer operação de acompanhamento (email de lembrete, criação de uma público-alvo etc.).

Siga estas etapas para configurar o **Aguardar** atividade:

1. Adicionar um **Aguardar** atividade no seu workflow.

1. Especifique a **Duração** da espera entre a ativação das transições de entrada e saída da atividade.

1. Selecionar a unidade de tempo **Período**: segundos, minutos, horas.





