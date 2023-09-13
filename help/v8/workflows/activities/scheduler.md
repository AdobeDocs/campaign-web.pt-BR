---
audience: end-user
title: Usar a atividade de workflow do Scheduler
description: Saiba como usar a atividade de workflow do Scheduler
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 42%

---


# Scheduler {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Atividade Scheduler"
>abstract="A atividade Scheduler permite..."

A atividade Scheduler permite programar quando um fluxo de trabalho ou uma atividade será iniciada.

A atividade Scheduler deve ser considerada como um início agendado. Esta atividade só pode ser usada como a primeira atividade do fluxo de trabalho.

## Práticas recomendadas

* É recomendável não agendar um workflow para execução por mais de 15 minutos, pois pode atrapalhar o desempenho geral do sistema e criar bloqueios no banco de dados.

## Configuração

Siga estas etapas para configurar o **Scheduler** atividade:

1. Adicionar um **Scheduler** atividade ao seu fluxo de trabalho.

1. Configure o **Frequência de execução**:

   * Uma vez: o fluxo de trabalho é executado uma única vez.

   * Daily: o workflow é executado em um horário específico, uma vez por dia.

   * Several times the day: o fluxo de trabalho é executado regularmente várias vezes ao dia. Você pode configurar as execuções em horários específicos ou periodicamente.

   * Semanalmente: o fluxo de trabalho é executado em um horário especificado, uma ou várias vezes por semana.

   * Mensalmente: o fluxo de trabalho é executado em um horário especificado, uma ou várias vezes por mês. Você pode selecionar meses quando precisar que o fluxo de trabalho seja executado. Você também pode configurar as execuções em um determinado dia da semana do mês, como a segunda terça-feira do mês.
1. Defina os detalhes da execução de acordo com a frequência selecionada. Os campos de detalhes podem variar dependendo da frequência usada (tempo, frequência de repetição, dias especificados etc.).

1. Clique em **Visualizar tempos de inicialização** para verificar a programação das próximas dez execuções do seu fluxo de trabalho.

1. Defina o período de validade do scheduler:

   * Permanente (nunca expira): o fluxo de trabalho será executado, de acordo com a frequência especificada, sem limites para o intervalo de tempo ou o número de iterações.

   * Período de validade: o fluxo de trabalho será executado de acordo com a frequência especificada, até uma data específica. Portanto, o prazo de execução precisará ser especificado.

## Exemplo


