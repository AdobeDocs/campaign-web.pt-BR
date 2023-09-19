---
audience: end-user
title: Usar a atividade de fluxo de trabalho Aguardar
description: Saiba como usar a atividade de fluxo de trabalho Aguardar
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 91%

---


# Aguardar {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Atividade de espera"
>abstract="A variável **Aguardar** A atividade é usada para atrasar a transição de uma atividade para outra."

A atividade **Aguardar** é uma atividade de **Controle de fluxo**. Ela é usada para permitir que um determinado período transcorra entre duas atividades que estão sendo executadas. Por exemplo, a espera de vários dias após uma atividade de entrega de email para depois analisar as aberturas e os cliques gerados durante esse período antes de executar qualquer operação de acompanhamento (email de lembrete, criação de público-alvo, etc.).

## Configuração{#wait-configuration}

Siga estas etapas para configurar a atividade **Aguardar**:

1. Adicione uma atividade **Aguardar** ao seu fluxo de trabalho.

1. Especifique a **Duração** da espera entre as transições de entrada e saída.

1. Selecione a unidade de tempo no campo **Períodos**: segundos, minutos, horas.

## Exemplo{#wait-example}

O exemplo a seguir ilustra a atividade **Aguardar** em um caso de uso comum. Um convite é enviado por email para um evento. 24 horas após o envio, é feita uma entrega de SMS para a mesma população.

![](../assets/workflow-wait-example.png)
