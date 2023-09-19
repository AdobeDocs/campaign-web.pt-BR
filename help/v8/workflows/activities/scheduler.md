---
audience: end-user
title: Usar a atividade de workflow do Scheduler
description: Saiba como usar a atividade de workflow do Scheduler
badge: label="Beta"
source-git-commit: 4f53f8765aeb2254a52eb48591d5e14250afc69d
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 15%

---


# Scheduler {#scheduler}


>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Atividade Scheduler"
>abstract="A variável **Scheduler** A atividade permite programar quando o workflow será iniciado. Essa atividade deve ser considerada como um início agendado. Ela só pode ser usada como a primeira atividade do workflow."


A variável **Scheduler** a atividade é um **Controle de fluxo** atividade. Ele permite programar quando o workflow será iniciado. Essa atividade deve ser considerada como um início agendado. Ela só pode ser usada como a primeira atividade do workflow.

## Práticas recomendadas{#scheduler-best-practices}

* É recomendável não agendar um workflow para execução por mais de 15 minutos, pois pode atrapalhar o desempenho geral do sistema e criar bloqueios no banco de dados.
* Se quiser enviar um delivery instantâneo no fluxo de trabalho, adicione uma atividade de scheduler e defina-a para executar **Uma vez**. Você também pode definir a variável **Agendar** nas configurações do delivery.
* Para enviar um delivery recorrente no workflow, é necessário usar um **Scheduler** e defina a frequência de execução. A atividade recorrente de delivery não permite definir um agendamento.

## Configuração{#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Validade do agendador"
>abstract="Você pode definir um período de validade para o scheduler. Pode ser permanente (padrão) ou pode ser válido até uma data específica."


>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Opções do agendador"
>abstract="Defina a frequência do scheduler. Ele pode ser executado em um momento específico, uma ou várias vezes por dia, semana ou mês."

Siga estas etapas para configurar o **Scheduler** atividade:

![](../assets/workflow-scheduler.png)

1. Adicionar um **Scheduler** atividade ao seu fluxo de trabalho.

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

>[!NOTE]
>
>Se quiser iniciar o workflow imediatamente, clique no link **Executar tarefa pendente** na barra de ação superior do scheduler. Esse botão só estará disponível quando você tiver iniciado o workflow.

## Exemplo{#scheduler-example}

No exemplo a seguir, a atividade é configurada para que o workflow seja executado várias vezes por dia às 9h e às 12h, todos os dias da semana de 1º de outubro de 2023 a 1º de janeiro de 2024.

![](../assets/workflow-scheduler2.png)



