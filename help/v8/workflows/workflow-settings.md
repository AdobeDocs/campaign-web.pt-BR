---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 1a608d2042ae257d89acbd67d99a0ce05d89f382
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 25%

---

# Definir as configurações do fluxo de trabalho {#workflow-settings}

Ao orquestrar atividades de workflow na tela, você pode acessar configurações avançadas relacionadas ao workflow. Por exemplo, é possível definir um fuso horário específico para o workflow, gerenciar como o workflow deve se comportar em caso de erro ou gerenciar o atraso após o qual o histórico do workflow deve ser removido.

Essas configurações são pré-definidas no template selecionado ao criar o workflow, mas podem ser editadas conforme necessário para esse workflow específico.

Para fazer isso, clique no link **[!UICONTROL Configurações do fluxo de trabalho]** no canto superior esquerdo da tela, ao lado do rótulo do workflow.

![](assets/workflow-settings.png)

## Propriedades do fluxo de trabalho {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="A confirmar"

A variável **[!UICONTROL Propriedades]** fornece configurações genéricas que também podem ser acessadas ao criar o workflow.

* **[!UICONTROL Rótulo]**: o rótulo do fluxo de trabalho que é exibido na lista.
* **[!UICONTROL Nome]**: o nome interno do workflow.
* **[!UICONTROL Pasta]**: a pasta onde o fluxo de trabalho deve ser salvo.
* **[!UICONTROL Campanha vinculada]**: este campo é exibido se o workflow foi criado em uma campanha. Ele permite abrir a campanha associada.
* **[!UICONTROL Fuso horário]**: defina um fuso horário específico para usar por padrão em todas as atividades do workflow. Por padrão, o fuso horário do fluxo de trabalho é aquele definido para o operador atual do Campaign.
* **[!UICONTROL Supervisor(es)]**: quando um workflow está com erro, os operadores pertencentes ao grupo de supervisão do workflow são notificados por email, desde que seu endereço de email esteja listado em seu perfil.
* **[!UICONTROL Descrição]**: use esse campo para fornecer uma descrição do fluxo de trabalho.

## Configurações de segmentação

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configurações de segmentação"
>abstract="A confirmar"

* **[!UICONTROL Dimensão de direcionamento]**: selecione a targeting dimension a ser usada para direcionar perfis: recipients, beneficiários de contrato, operadores, assinantes, etc.
* **[!UICONTROL Manter o resultado de públicos provisórios entre duas execuções]**: por padrão, somente as tabelas de trabalho da última execução do workflow são mantidas. As tabelas de trabalho das execuções anteriores são removidas por um workflow técnico, executado diariamente.

   Se essa opção estiver ativada, as tabelas de trabalho serão mantidas mesmo após a execução do workflow. Você pode usá-lo para fins de teste e, portanto, deve ser usado apenas em ambientes de desenvolvimento ou de preparo. Nunca deve ser verificado em um workflow de produção.

## Configurações de execução

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Configurações de execução"
>abstract="A confirmar"

* **[!UICONTROL Histórico em dias]**: especifica o número de dias após os quais o histórico deve ser limpo. O histórico contém elementos relacionados ao workflow: logs, tarefas, eventos (objetos técnicos vinculados à operação do workflow). O valor padrão é de 30 dias para modelos de fluxo de trabalho prontos para uso. A limpeza do histórico é executada pelo fluxo de trabalho técnico de limpeza do banco de dados, que é executado todos os dias por padrão

   >[!IMPORTANT]
   >
   >Se o campo **[!UICONTROL Histórico em dias]** for deixado em branco, o valor “1” será considerado, o que significa que o histórico será removido após 1 dia.

* **[!UICONTROL Afinidade padrão]**: se a instalação incluir vários servidores de workflow, use esse campo para escolher a máquina em que o workflow será executado. Se o valor definido nesse campo não existir em nenhum servidor, o workflow permanecerá pendente.

* **[!UICONTROL Salvar consultas SQL no log]**: permite salvar as consultas SQL do workflow nos logs. Essa operação é reservada para usuários avançados. Aplica-se a workflows que contêm atividades de direcionamento como **[!UICONTROL Criar público-alvo]**. Quando essa opção está habilitada, as consultas SQL enviadas ao banco de dados durante a execução do workflow são exibidas no Adobe Campaign, permitindo analisá-las para otimizar as consultas ou diagnosticar problemas.

   Os queries são exibidos em uma guia **[!UICONTROL SQL logs]** adicionada ao workflow (exceto workflows da campanha) e à atividade **[!UICONTROL Properties]** quando a opção está habilitada.<!-- where?-->

## Configurações de gerenciamento de erros

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Configurações de gerenciamento de erros"
>abstract="A confirmar"

* **[!UICONTROL Gerenciamento de erros]**: este campo permite que você defina as ações a serem tomadas se uma tarefa de workflow tiver erros. Há duas opções possíveis:

   * **[!UICONTROL Suspender processo]**: o workflow é pausado automaticamente e seu status é alterado para **[!UICONTROL Failed]**. Quando o problema for resolvido, retome o workflow usando o **[!UICONTROL Retomar]** botões.
   * **[!UICONTROL Ignorar]**: O status da tarefa que provocou o erro muda para **[!UICONTROL Failed]**, mas o workflow mantém o **[!UICONTROL Iniciado]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Interromper o processo]**: o workflow é interrompido automaticamente e seu status muda para **[!UICONTROL Failed]**. Quando o problema for resolvido, reinicie o workflow usando o **[!UICONTROL Início]** botões.

* **[!UICONTROL Consecutive errors]**: este campo fica disponível quando o **[!UICONTROL Ignorar]** valor estiver selecionado na variável **[!UICONTROL No caso de erros]** campo. Você pode especificar quantos erros podem ser ignorados antes que o processo seja interrompido. Após esse número ser alcançado, o status do workflow será alterado para **[!UICONTROL Failed]**. Se o valor desse campo for 0, o workflow nunca será interrompido independentemente do número de erros.
