---
audience: end-user
title: Usar a atividade de workflow do Scheduler
description: Saiba como usar a atividade de workflow do Scheduler
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 058a9347329b35e49463b7d74bffa5b3c69b4a92
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 27%

---

# Scheduler {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Atividade Scheduler"
>abstract="A atividade **Scheduler** permite programar quando o fluxo de trabalho será iniciado. Esta atividade deve ser considerada como um início agendado. Ela só pode ser usada como a primeira atividade do fluxo de trabalho."

A atividade **Scheduler** é uma atividade de **Controle de fluxo**. Ela permite programar quando o fluxo de trabalho será iniciado. Esta atividade deve ser considerada como um início programado. Ela só pode ser usada como a primeira atividade do fluxo de trabalho.

## Práticas recomendadas {#scheduler-best-practices}

* Não agende um workflow para execução por mais de 15 minutos, pois pode atrapalhar o desempenho geral do sistema e criar bloqueios no banco de dados.
* Para enviar uma entrega única no seu fluxo de trabalho, adicione uma atividade de agendador e configure-a para ser executada **Uma vez**. Defina o **Cronograma** nas configurações de entrega.
* Para enviar uma entrega recorrente no seu fluxo de trabalho, use uma atividade **Scheduler** e defina a frequência de execução. A atividade recorrente de delivery não permite definir um agendamento.

## Configuração de atividade do scheduler {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Validade do Scheduler"
>abstract="É possível definir um período de validade para o Scheduler. Pode ser permanente (padrão) ou pode ser válido até uma data específica."

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Opções do Scheduler"
>abstract="Defina a frequência do scheduler. Pode ser executado em um momento específico, uma ou várias vezes por dia, semana ou mês."

Siga estas etapas para configurar a atividade **Scheduler**:

![Interface de configuração de atividade do agendador](../assets/workflow-scheduler.png)

1. Adicione uma atividade **Scheduler** ao seu fluxo de trabalho.

1. Configure a **Frequência de execução**:

   * **Uma vez**: o fluxo de trabalho é executado uma única vez.
   * **Diariamente**: o fluxo de trabalho é executado em um horário específico, uma vez por dia.
   * **Várias vezes por dia**: o fluxo de trabalho é executado regularmente várias vezes ao dia. Configure as execuções em horários específicos ou periodicamente.
   * **Semanalmente**: o fluxo de trabalho é executado em um horário especificado, uma ou várias vezes por semana.
   * **Monthly**: o fluxo de trabalho é executado em um momento especificado, uma ou várias vezes por mês. Selecione os meses em que o workflow precisa ser executado. Você também pode configurar as execuções em dias da semana especificados do mês, como a segunda terça-feira do mês.

1. Defina os detalhes da execução de acordo com a frequência selecionada. Os campos de detalhes podem variar dependendo da frequência usada (tempo, frequência de repetição, dias especificados e opções semelhantes).

1. Clique em **Visualizar horários de inicialização** para verificar o agendamento das próximas dez execuções do seu fluxo de trabalho.

1. Defina o período de validade do scheduler:

   * **Permanente (nunca expira)**: o fluxo de trabalho é executado de acordo com a frequência especificada, sem limites para o intervalo de tempo ou o número de iterações.
   * **Período de validade**: o fluxo de trabalho é executado de acordo com a frequência especificada, até uma data específica. Especifique datas de início e término.

>[!NOTE]
>Para iniciar o fluxo de trabalho imediatamente, clique em **Executar tarefa pendente** na barra de ações superior do agendador. Esse botão só estará disponível quando o workflow tiver sido iniciado.

## Exemplo {#scheduler-example}

No exemplo a seguir, a atividade é configurada para que o workflow seja executado várias vezes por dia às 9h e às 12h, todos os dias da semana de 1º de outubro de 2023 a 1º de janeiro de 2024.

![Configuração de exemplo de atividade do agendador](../assets/workflow-scheduler2.png)
