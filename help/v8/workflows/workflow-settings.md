---
audience: end-user
title: Criar workflows com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com a Web Adobe Campaign
badge: label="Alpha" type="Positive"
source-git-commit: 60cd0ed8dcbe3e6003c1cde674fe3441d6d88869
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 61%

---

# Definir as configurações do fluxo de trabalho {#workflow-settings}

TBD de conteúdo

defina as configurações disponíveis no botão na tela do fluxo de trabalho
<!--à reformuler-->

## Propriedades do workflow {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriedades do workflow"
>abstract="A confirmar"

(= igual ao criar workflow ? para verificar)

* Rótulo
* Opções adicionais
* Nome interno
* Pasta
* Campanha vinculada > pode alterá-la. Nesse caso, o workflow desaparecerá da campanha atual e aparecerá no novo vinculado
* Fuso horário: defina um fuso horário específico para usar por padrão em todas as atividades do workflow. Por padrão, o fuso horário do workflow é aquele definido para o operador atual do Campaign.
* Supervisor: Quando um workflow está com erro, os operadores pertencentes ao grupo de supervisão do workflow são notificados por email, desde que seu endereço de email esteja listado em seu perfil. Esse grupo é selecionado no campo **[!UICONTROL Supervisor(s)]** das propriedades do workflow.
* descrição

## Configurações de segmentação

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configurações de segmentação"
>abstract="A confirmar"

* targeting dimension:

   Durante as operações de segmentação de dados, a chave de target é mapeada para uma dimensão de filtro. O targeting dimension permite definir o público alvo da operação: recipients, beneficiários de contrato, operadores, assinantes etc. A dimensão de filtro permite selecionar o público com base em determinados critérios: titulares de contratos, assinantes de boletins informativos, etc.

* manter resultados: O **Manter o resultado de públicos provisórios entre duas execuções** mantém tabelas temporárias entre duas execuções de um workflow.  Está disponível na guia **[!UICONTROL General]** das propriedades do workflow e pode ser usado para desenvolvimento e testes para monitorar dados e verificar resultados. Você pode usar essa opção em ambientes de desenvolvimento, mas nunca usá-la em ambientes de produção. Manter tabelas temporárias pode resultar no aumento significativo do tamanho de banco de dados e, por fim, atingir o limite de tamanho. Além disso, o backup ficará lento.

   Somente as tabelas de trabalho da última execução do workflow são mantidas. As tabelas de trabalho das execuções anteriores são removidas pelo workflow **[!UICONTROL cleanup]**, executado diariamente.

   >[!CAUTION]
   >
   >Essa opção deve **never** seja verificado em um **produção** fluxo de trabalho. Essa opção é usada para analisar os resultados e é projetada apenas para fins de teste e, portanto, deve ser usada apenas em ambientes de desenvolvimento ou de preparo.

## Configurações de execução do workflow

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Configurações de execução"
>abstract="A confirmar"

* Histórico em dias: As tabelas de trabalho do banco de dados mantêm um histórico de execuções (tarefas, eventos, log). Aqui você pode definir a quantidade de dias para o arquivamento deste workflow: o processo de limpeza excluirá os arquivos mais antigos uma vez por dia. Se o valor nesse campo for zero, o arquivo nunca será excluído.

   especifica o número de dias após o qual o histórico deve ser removido. O histórico contém elementos relacionados ao workflow: logs, tarefas, eventos (objetos técnicos vinculados à operação do workflow), bem como arquivos baixados pela **[!UICONTROL Transferir arquivo]** atividade . O valor padrão é 30 dias para modelos de fluxo de trabalho prontos para uso.

   A limpeza do histórico é executada pelo workflow técnico Database cleanup , que é executado por padrão todos os dias

   >[!IMPORTANT]
   >
   >Se a variável **[!UICONTROL Histórico em dias]** for deixado em branco, seu valor será considerado como &quot;1&quot;, o que significa que o histórico será removido após 1 dia.

* afinidade padrão: este campo permite que você force a execução de um fluxo de trabalho ou de uma atividade de fluxo de trabalho em uma máquina específica.   Se a sua instalação incluir vários servidores de workflow, utilize este campo para escolher a máquina em que o workflow será executado. Se o valor definido nesse campo não existir em nenhum servidor, o workflow permanecerá pendente.

* salvar consultas sql no log: permite salvar as consultas SQL do workflow nos logs. (onde acessar logs sql?)

   Essa operação é reservada para usuários avançados. Refere-se a workflows que contêm atividades de definição de metas (query, união, intersecção, etc.). Quando essa opção é marcada, as queries SQL enviadas ao banco de dados durante a execução do workflow são exibidas na Adobe Campaign: isso significa que você pode analisá-las para otimizar as queries ou diagnosticar problemas.

   Os queries são exibidos em uma guia **[!UICONTROL SQL logs]** adicionada ao workflow (exceto workflows da campanha) e à atividade **[!UICONTROL Properties]** quando a opção está habilitada. A aba **[!UICONTROL Audit]** também inclui queries SQL.

## Configurações de gerenciamento de erros

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Configurações de gerenciamento de erros"
>abstract="A confirmar"

* Este campo permite a definição das ações a serem tomadas se uma tarefa de workflow tiver erros. Há duas opções possíveis:

   Stop the process: o workflow é pausado automaticamente. O status do workflow muda para Failed. Quando o problema for resolvido, reinicie o workflow usando os botões Start ou Restart.

   Ignore: o status da tarefa que provocou o erro muda para Failed, mas o workflow mantém o status de Started. Essa configuração é relevante para tarefas recorrentes: se a ramificação incluir um programador, ela iniciará normalmente na próxima vez que o workflow for executado.

* Erros consecutivos: Esse campo fica disponível quando o valor Ignore é selecionado no campo In case of errors . Você pode especificar quantos erros podem ser ignorados antes que o processo seja interrompido. Após esse número ser alcançado, o status do workflow será alterado para Failed. Se o valor desse campo for 0, o workflow nunca será interrompido independentemente do número de erros.
