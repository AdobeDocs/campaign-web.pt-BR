---
audience: end-user
title: Usar a atividade de fluxo de trabalho Aguardar
description: Saiba como usar a atividade de fluxo de trabalho Aguardar
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
TQID: https://experienceleague.adobe.com/pe-T3-3w5HaS0pNOZITNC1YS5hiJpj3H3P1eM0GmXb8
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 185
ht-degree: 47%

---

# Aguardar {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Atividade de espera"
>abstract="A Atividade **aguardar** é usada para atrasar a transição de uma atividade para outra."

A atividade **Aguardar** é uma atividade de **Controle de fluxo**. Ele permite que um determinado período transcorra entre a execução de duas atividades. Por exemplo, ele pode ser usado para aguardar vários dias após uma atividade de delivery de email e depois analisar as aberturas e os cliques gerados durante esse período antes de executar operações de acompanhamento, como enviar um email de lembrete ou criar um público-alvo.

## Configuração {#wait-configuration}

Siga estas etapas para configurar a atividade **Aguardar**:

1. Adicione uma atividade **Aguardar** ao seu fluxo de trabalho.

1. Especifique a **Duração** da espera entre as transições de entrada e saída.

1. Selecione a unidade de tempo no campo **Períodos**: segundos, minutos, horas ou dias.

## Exemplo {#wait-example}

O exemplo a seguir ilustra a atividade **Aguardar** em um caso de uso comum. Um convite é enviado por email para um evento. Após 24 horas, um delivery de SMS é enviado para a mesma população.

![Exemplo de um fluxo de trabalho usando a atividade Aguardar para enviar um SMS 24 horas após um convite por email.](../assets/workflow-wait-example.png)