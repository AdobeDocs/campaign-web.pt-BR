---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 806e465b7c1df6cd26d68103c45b175371d73485
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 63%

---

# Definir configurações avançadas de fluxo de trabalho {#workflow-settings}

Ao orquestrar atividades de workflow na tela, você pode acessar configurações avançadas relacionadas ao workflow. Por exemplo, é possível definir um fuso horário específico para o workflow, gerenciar como o workflow deve se comportar em caso de erro ou gerenciar o atraso após o qual o histórico do workflow deve ser removido.

Para fazer isso, clique no link **[!UICONTROL Configurações do fluxo de trabalho]** no canto superior esquerdo da tela, ao lado do rótulo do workflow.

![](assets/workflow-settings.png)

## Propriedades do fluxo de trabalho {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="A confirmar"

A seção de propriedades do fluxo de trabalho fornece propriedades genéricas que também podem ser acessadas ao criar o fluxo de trabalho.

* **[!UICONTROL Rótulo]**: o rótulo do fluxo de trabalho que é exibido na lista.
* **[!UICONTROL Nome interno]**: o nome interno do workflow.
* **[!UICONTROL Pasta]**: a pasta onde o fluxo de trabalho deve ser salvo.
* **[!UICONTROL Campanha vinculada]**: este campo é exibido se o workflow foi criado em uma campanha. Ele permite abrir a campanha associada.
* **[!UICONTROL Fuso horário]**: defina um fuso horário específico para usar por padrão em todas as atividades do workflow. Por padrão, o fuso horário do fluxo de trabalho é aquele definido para o operador atual do Campaign.
* **[!UICONTROL Supervisor]**: quando um workflow está com erro, os operadores pertencentes ao grupo de supervisão do workflow são notificados por email, desde que seu endereço de email esteja listado em seu perfil.
* **[!UICONTROL Descrição]**: use esse campo para fornecer uma descrição do fluxo de trabalho.

## Configurações de segmentação

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configurações de segmentação"
>abstract="A confirmar"

* **[!UICONTROL Dimensão de direcionamento]**: selecione a targeting dimension a ser usada para direcionar perfis: recipients, beneficiários de contrato, operadores, assinantes, etc.
* **[!UICONTROL Manter o resultado de públicos provisórios entre duas execuções]**: por padrão, somente as tabelas de trabalho da última execução do workflow são mantidas. As tabelas de trabalho das execuções anteriores são removidas por um workflow técnico, executado diariamente.

   Se essa opção estiver ativada, as tabelas de trabalho serão mantidas mesmo após a execução do workflow. Você pode usá-lo para fins de teste e, portanto, deve ser usado apenas em ambientes de desenvolvimento ou de preparo. Nunca deve ser verificado em um workflow de produção,

## Configurações de execução do fluxo de trabalho

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Configurações de execução"
>abstract="A confirmar"

* Histórico em dias: as tabelas de trabalho do banco de dados mantêm um histórico de execuções (tarefas, eventos e logs). Aqui você pode definir a quantidade de dias para o arquivamento deste workflow: o processo de limpeza excluirá os arquivos mais antigos uma vez por dia. Se o valor nesse campo for zero, o arquivo nunca será excluído.

   especifica o número de dias após o qual o histórico deve ser apagado. O histórico contém elementos relacionados ao fluxo de trabalho: logs, tarefas, eventos (objetos técnicos vinculados ao funcionamento do fluxo de trabalho), bem como arquivos baixados pela atividade **[!UICONTROL Transferir arquivo]**. O valor padrão é de 30 dias para modelos de fluxo de trabalho prontos para uso.

   A limpeza do histórico é executada pelo fluxo de trabalho técnico de limpeza do banco de dados, que é executado todos os dias por padrão

   >[!IMPORTANT]
   >
   >Se o campo **[!UICONTROL Histórico em dias]** for deixado em branco, o valor “1” será considerado, o que significa que o histórico será removido após 1 dia.

* afinidade padrão: este campo permite forçar a execução de um fluxo de trabalho ou de uma atividade de fluxo de trabalho em um computador específico.   Se a sua instalação incluir vários servidores de workflow, utilize este campo para escolher a máquina em que o workflow será executado. Se o valor definido nesse campo não existir em nenhum servidor, o workflow permanecerá pendente.

* salvar consultas SQL no log: permite salvar as consultas SQL do fluxo de trabalho nos logs. (onde acessar logs de SQL?)

   Essa operação é reservada para usuários avançados. Refere-se a workflows que contêm atividades de direcionamento (consulta, união, intersecção, etc.). Quando essa opção é marcada, as queries SQL enviadas ao banco de dados durante a execução do workflow são exibidas na Adobe Campaign: isso significa que você pode analisá-las para otimizar as queries ou diagnosticar problemas.

   Os queries são exibidos em uma guia **[!UICONTROL SQL logs]** adicionada ao workflow (exceto workflows da campanha) e à atividade **[!UICONTROL Properties]** quando a opção está habilitada. A aba **[!UICONTROL Audit]** também inclui queries SQL.

## Configurações de gerenciamento de erros

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Configurações de gerenciamento de erros"
>abstract="A confirmar"

* Este campo permite a definição das ações a serem tomadas se uma tarefa de workflow tiver erros. Há duas opções possíveis:

   Interromper o processo: o fluxo de trabalho é pausado automaticamente. O status do fluxo de trabalho muda para Com falha. Quando o problema for resolvido, reinicie o fluxo de trabalho usando os botões Iniciar ou Reiniciar.

   Ignorar: o status da tarefa que provocou o erro muda para Com falha, mas o fluxo de trabalho mantém o status Iniciado. Essa configuração é relevante para tarefas recorrentes: se a ramificação incluir um programador, ela iniciará normalmente na próxima vez que o fluxo de trabalho for executado.

* Erros consecutivos: este campo fica disponível quando o valor Ignorar é selecionado no campo Em caso de erros. Você pode especificar quantos erros podem ser ignorados antes que o processo seja interrompido. Após esse número ser alcançado, o status do fluxo de trabalho será alterado para Com falha. Se o valor desse campo for 0, o fluxo de trabalho nunca será interrompido, independentemente do número de erros.
