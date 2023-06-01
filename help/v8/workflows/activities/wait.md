---
audience: end-user
title: Usar a atividade de workflow Aguardar
description: Saiba como usar a atividade de workflow Aguardar
badge: label="Alpha" type="Positive"
source-git-commit: 9be56c3c9c7a339e1f348ac9c74d425b501c317d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 39%

---


# Aguardar {#wait}

A variável **Aguardar** A atividade suspende temporariamente a execução de uma parte do fluxo de trabalho. Ela ativa a transição de saída após um atraso que pode variar de alguns segundos a vários meses, o que executa as atividades colocadas depois.

A variável **Aguardar** A atividade é usada para permitir que um determinado período transcorra entre duas atividades que estão sendo executadas. Por exemplo, a espera de vários dias após uma atividade de delivery de email para depois analisar as aberturas e os cliques gerados durante esse período antes de executar qualquer operação de acompanhamento (email de lembrete, criação de uma público-alvo etc.).

## Configuração

Siga estas etapas para configurar o **Aguardar** atividade:

1. Adicionar um **Aguardar** atividade no seu workflow.

1. Especifique a **Duração** da espera entre a ativação das transições de entrada e saída da atividade.

1. Selecionar a unidade de tempo **Período**: segundos, minutos, horas.

## Exemplo

O exemplo a seguir ilustra a **Aguardar** em um caso de uso típico. Um convite é enviado por email para um evento. 24 horas após o envio, um delivery de SMS é enviado para a mesma população.

![](../assets/workflow-wait-example.png)
