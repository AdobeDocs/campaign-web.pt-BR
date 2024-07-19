---
audience: end-user
title: Usar a atividade do fluxo de trabalho Query incremental
description: Saiba como usar a atividade de workflow Query incremental
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 23%

---

# Query incremental {#incremental-query}



>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Query incremental"
>abstract="A atividade **Consulta incremental** é uma atividade de **Direcionamento** que permite consultar o banco de dados usando o Modelador de consulta. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Ela permite direcionar somente elementos novos."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Histórico de consultas incrementais"
>abstract="Histórico de consultas incrementais"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Dados processados da consulta incremental"
>abstract="Dados processados da consulta incremental"

A atividade de **Consulta incremental** é uma atividade de **Direcionamento** que permite consultar o banco de dados de forma agendada. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Ela permite direcionar somente elementos novos.

>[!NOTE]
>
>Embora o console do cliente do Campaign integre a atividade **[!UICONTROL Query incremental]** a um scheduler integrado, a Interface do Usuário da Web do Campaign trata essa funcionalidade separadamente. Para agendar execuções de consultas incrementais, você deve adicionar uma atividade **[!UICONTROL Scheduler]** no fluxo de trabalho antes da atividade **[!UICONTROL Query incremental]**. [Saiba como configurar uma atividade do Agendador](scheduler.md)

A atividade **[!UICONTROL Query incremental]** pode ser usada para vários tipos de usos:

* Segmentação de indivíduos para definir o público-alvo ou o público de uma mensagem, etc.
* Exportação de dados. Por exemplo, você pode usar a atividade para exportar regularmente novos logs em arquivos. Pode ser útil se você quiser usar seus dados de log em ferramentas externas de BI ou geração de relatórios.

A população já direcionada por execuções anteriores é armazenada no workflow. Isso significa que dois workflows iniciados do mesmo template não compartilham o mesmo log. No entanto, duas tarefas baseadas no mesmo query incremental no mesmo workflow usam o mesmo log.

Se o resultado de um query incremental for igual a 0 durante uma de suas execuções, o workflow será pausado até a próxima execução programada do query. As transições e as atividades que seguem o query incremental não são, portanto, processadas antes da execução a seguir.

## Configurar a atividade de query incremental {#incremental-query-configuration}

Siga estas etapas para configurar a atividade **Consulta incremental**:

![](../assets/incremental-query.png)

1. Adicione uma atividade de **Consulta incremental** ao seu fluxo de trabalho.

1. Na seção **[!UICONTROL Público-alvo]**, escolha a **Dimensão de direcionamento** e clique em **[!UICONTROL Continuar]**.

   A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, o público-alvo é selecionado entre os destinatários. [Saiba mais sobre dimensões de direcionamento](../../audience/about-recipients.md#targeting-dimensions)

1. Use o modelador de consultas para definir seu query, da mesma forma que você cria um público-alvo ao criar um novo email. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md)

1. Na seção **[!UICONTROL Dados processados]**, selecione o modo incremental a ser usado:

   * **[!UICONTROL Excluir resultados da execução anterior]**: cada vez que a atividade é executada, os resultados das execuções anteriores são excluídos.

     Os registros já direcionados em execuções anteriores podem ser registrados em um número máximo de dias a partir do dia em que foram direcionados. Para fazer isso, use o campo **[!UICONTROL Histórico em dias]**. Se esse valor for zero, os destinatários nunca serão removidos do log.

   * **[!UICONTROL Usar um campo de data]**: essa opção permite excluir resultados de execuções anteriores com base em um campo de data específico. Para fazer isso, escolha o campo de data desejado na lista de atributos disponíveis para o targeting dimension selecionado. Nas próximas execuções do workflow, somente os dados que foram modificados ou criados após a última data de execução serão recuperados.

     Após a primeira execução do fluxo de trabalho, o campo **[!UICONTROL Data da última execução]** ficará disponível. Especifica a data que será usada para a próxima execução e é atualizada automaticamente toda vez que o workflow é executado. Você ainda tem a possibilidade de substituir esse valor, inserindo manualmente um novo para que ele se ajuste às suas necessidades.

   >[!NOTE]
   >
   >O modo **[!UICONTROL Usar um campo de data]** permite mais flexibilidade dependendo do campo de data selecionado. Por exemplo, se o campo especificado corresponder a uma data de modificação, o modo de campo de data permitirá recuperar dados que foram atualizados recentemente, enquanto o outro modo simplesmente excluirá gravações que já foram direcionadas para uma execução anterior, mesmo que elas tenham sido modificadas desde a última execução do workflow.

## Exemplo {#incremental-query-example}

O exemplo a seguir mostra a configuração de um fluxo de trabalho que filtra todas as semanas os perfis no banco de dados do Adobe Campaign que estão inscritos no serviço Yoga Newsletter, para enviar a eles um email de boas-vindas.

![](../assets/incremental-query-example.png)

O fluxo de trabalho é composto dos seguintes elementos:

* Uma atividade **[!UICONTROL Scheduler]**, para executar o fluxo de trabalho todas as segundas-feiras às 6 horas.
* Uma atividade **[!UICONTROL Query incremental]**, que segmenta todos os assinantes atuais durante a primeira execução e depois somente os novos assinantes daquela semana durante as execuções a seguir.
* Uma atividade de **[!UICONTROL Entrega de email]**.
