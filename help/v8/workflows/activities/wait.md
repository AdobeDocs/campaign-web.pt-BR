---
audience: end-user
title: Usar a atividade de workflow Aguardar
description: Saiba como usar a atividade de workflow Aguardar
badge: label="Alpha" type="Positive"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 31%

---


# Aguardar {#wait}

A variável **Aguardar** a atividade é um **Controle de fluxo** atividade. É usado para permitir que um determinado período transcorra entre duas atividades que estão sendo executadas. Por exemplo, a espera de vários dias após uma atividade de delivery de email para depois analisar as aberturas e os cliques gerados durante esse período antes de executar qualquer operação de acompanhamento (email de lembrete, criação de uma público-alvo etc.).

## Configuração

Siga estas etapas para configurar o **Aguardar** atividade:

1. Adicionar um **Aguardar** atividade no seu workflow.

1. Especifique a **Duração** da espera entre as transições de entrada e saída.

1. Selecione a unidade de tempo na variável **Períodos** campo: segundos, minutos, horas.

## Exemplo

O exemplo a seguir ilustra a **Aguardar** em um caso de uso típico. Um convite é enviado por email para um evento. 24 horas após o envio, um delivery de SMS é enviado para a mesma população.

![](../assets/workflow-wait-example.png)
