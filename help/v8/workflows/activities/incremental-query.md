---
audience: end-user
title: Usar a atividade do fluxo de trabalho Query incremental
description: Saiba como usar a atividade de workflow Query incremental
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 13%

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

A atividade de **Consulta incremental** é uma atividade de **Direcionamento** que permite consultar o banco de dados de forma agendada. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Isso permite direcionar somente elementos novos.

>[!NOTE]
>
>Embora o console do cliente do Campaign integre a atividade **[!UICONTROL Query incremental]** a um scheduler integrado, a Interface do Usuário da Web do Campaign trata essa funcionalidade separadamente. Para agendar execuções de consultas incrementais, adicione uma atividade **[!UICONTROL Scheduler]** no fluxo de trabalho antes da atividade **[!UICONTROL Query incremental]**. [Saiba como configurar uma atividade do Agendador](scheduler.md)

A atividade **[!UICONTROL Query incremental]** pode ser usada para várias finalidades:

* Segmentação de indivíduos para definir o público-alvo de uma mensagem, público ou outras operações.
* Exportação de dados. Por exemplo, use a atividade para exportar regularmente novos logs em arquivos. Isso é útil para ferramentas de geração de relatórios externos ou de business intelligence.

A população já direcionada por execuções anteriores é armazenada no workflow. Dois workflows iniciados do mesmo modelo não compartilham o mesmo log. No entanto, duas tarefas baseadas no mesmo query incremental no mesmo workflow usam o mesmo log.

Se o resultado de um query incremental for igual a 0 durante uma de suas execuções, o workflow pausará até a próxima execução programada do query. As transições e atividades que seguem o query incremental não são processadas antes da próxima execução.

## Configurar a atividade de query incremental {#incremental-query-configuration}

Siga estas etapas para configurar a atividade **Consulta incremental**:

[Descrição: captura de tela que mostra a interface de configuração da atividade de consulta incremental no Adobe Campaign.]\
![](../assets/incremental-query.png)

1. Adicione uma atividade de **Consulta incremental** ao seu fluxo de trabalho.

1. Na seção **[!UICONTROL Público-alvo]**, escolha a **Dimensão de direcionamento** e clique em **[!UICONTROL Continuar]**.

   O targeting dimension define o público alvo da operação, como recipients, beneficiários de contrato, operadores ou assinantes. Por padrão, o público-alvo é selecionado entre os destinatários. [Saiba mais sobre dimensões de direcionamento](../../audience/about-recipients.md#targeting-dimensions)

1. Use o modelador de consultas para definir sua consulta, de modo semelhante a como você cria um público-alvo ao criar um novo email. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md)

1. Na seção **[!UICONTROL Dados processados]**, selecione o modo incremental a ser usado:

   * **[!UICONTROL Excluir resultados da execução anterior]**: cada vez que a atividade é executada, os resultados das execuções anteriores são excluídos.

     Os registros já direcionados em execuções anteriores podem ser registrados por um número máximo de dias a partir do dia em que foram direcionados. Use o campo **[!UICONTROL Histórico em dias]** para definir este valor. Se esse valor for zero, os destinatários nunca serão removidos do log.

   * **[!UICONTROL Use um campo de data]**: essa opção exclui os resultados das execuções anteriores com base em um campo de data específico. Escolha o campo de data desejado na lista de atributos disponíveis para o targeting dimension selecionado. Em execuções subsequentes do workflow, somente os dados modificados ou criados após a última data de execução serão recuperados.

     Após a primeira execução do fluxo de trabalho, o campo **[!UICONTROL Data da última execução]** ficará disponível. Especifica a data usada para a próxima execução e é atualizada automaticamente sempre que o workflow é executado. Você pode substituir manualmente esse valor para atender às suas necessidades.

   >[!NOTE]
   >
   >O modo **[!UICONTROL Usar um campo de data]** oferece mais flexibilidade dependendo do campo de data selecionado. Por exemplo, se o campo especificado corresponder a uma data de modificação, o modo do campo de data recuperará os dados atualizados recentemente. O outro modo exclui gravações já direcionadas em uma execução anterior, mesmo que tenham sido modificadas desde a última execução do workflow.

## Exemplo {#incremental-query-example}

O exemplo a seguir mostra a configuração de um fluxo de trabalho que filtra perfis no banco de dados do Adobe Campaign todas as semanas. Ele direciona os indivíduos inscritos no serviço de boletim informativo de Yoga e envia a eles um email de boas-vindas.

![Captura de tela de um exemplo de configuração de fluxo de trabalho para filtrar perfis inscritos no serviço Yoga Newsletter.](../assets/incremental-query-example.png)

O workflow inclui os seguintes elementos:

* Uma atividade **[!UICONTROL Scheduler]**, que executa o fluxo de trabalho toda segunda-feira às 6 horas.
* Uma atividade de **[!UICONTROL Consulta incremental]**, que segmenta todos os assinantes atuais durante a primeira execução e somente os novos assinantes durante as execuções subsequentes.
* Uma atividade de **[!UICONTROL Entrega de email]**.