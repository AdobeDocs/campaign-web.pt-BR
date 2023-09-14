---
audience: end-user
title: Usar a atividade de workflow do Scheduler
description: Saiba como usar a atividade de workflow do Scheduler
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 22%

---


# Scheduler {#scheduler}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler activity"
>abstract="The Scheduler activity allows you..."
-->

A variável **Scheduler** a atividade é um **Controle de fluxo** atividade. Ele permite programar quando o workflow será iniciado. Essa atividade deve ser considerada como um início agendado. Ela só pode ser usada como a primeira atividade do workflow.

## Práticas recomendadas

É recomendável não agendar um workflow para execução por mais de 15 minutos, pois pode atrapalhar o desempenho geral do sistema e criar bloqueios no banco de dados.

## Configuração

Siga estas etapas para configurar o **Scheduler** atividade:

1. Adicionar um **Scheduler** atividade ao seu fluxo de trabalho.

   ![](../assets/workflow-scheduler.png)

1. Configure o **Frequência de execução**:

   * **Uma vez**: o fluxo de trabalho é executado uma única vez.

   * **Diariamente**: o fluxo de trabalho é executado em um horário específico, uma vez por dia.

   * **Várias vezes ao dia:** o workflow é executado regularmente várias vezes ao dia. Você pode configurar as execuções em horários específicos ou periodicamente.

   * **Semanalmente**: o fluxo de trabalho é executado em um horário especificado, uma ou várias vezes por semana.

   * **Mensal**: o fluxo de trabalho é executado em um horário especificado, uma ou várias vezes por mês. Você pode selecionar meses quando precisar que o fluxo de trabalho seja executado. Você também pode configurar as execuções em dias da semana especificados do mês, como a segunda terça-feira do mês.

1. Defina os detalhes da execução de acordo com a frequência selecionada. Os campos de detalhes podem variar dependendo da frequência usada (tempo, frequência de repetição, dias especificados etc.).

1. Clique em **Visualizar tempos de inicialização** para verificar a programação das próximas dez execuções do seu fluxo de trabalho.

1. Defina o período de validade do scheduler:

   * **Permanente (nunca expira)**: o fluxo de trabalho é executado de acordo com a frequência especificada, sem limites para o intervalo de tempo ou o número de iterações.

   * **Período de validade**: o fluxo de trabalho é executado de acordo com a frequência especificada, até uma data específica. É necessário especificar datas de início e término.

## Exemplo

No exemplo a seguir, a atividade é configurada para iniciar o workflow várias vezes por dia às 9h e 12h, todos os dias da semana de 1º de outubro de 2023 a 1º de janeiro de 2024.

![](../assets/workflow-scheduler2.png)



