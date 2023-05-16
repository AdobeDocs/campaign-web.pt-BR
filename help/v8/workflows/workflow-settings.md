---
audience: end-user
title: Criar fluxos de trabalho com o Adobe Campaign Web
description: Saiba como criar fluxos de trabalho com o Adobe Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: ad5a995563c3192a73e1658878eeb58ce55fc24c
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 100%

---

# Definir as configurações do fluxo de trabalho {#workflow-settings}

Conteúdo a ser definido

defina as configurações disponíveis no botão na tela do fluxo de trabalho
<!--à reformuler-->

## Propriedades do fluxo de trabalho {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Propriedades do fluxo de trabalho"
>abstract="A confirmar"

(= igual ao criar o fluxo de trabalho ? para verificar)

* Rótulo
* Opções adicionais
* Nome interno
* Pasta
* Campanha vinculada > pode alterá-la. Nesse caso, o fluxo de trabalho desaparecerá da campanha atual e aparecerá no novo vinculado
* Fuso horário: por padrão, é possível definir um fuso horário específico para usar em todas as atividades do fluxo de trabalho. Por padrão, o fuso horário do fluxo de trabalho é aquele definido para o operador atual do Campaign.
* Supervisor: quando um fluxo de trabalho está com erro, o(s) operador(es) pertencente(s) ao grupo de supervisão do fluxo de trabalho recebe(m) notificação por email, desde que o endereço de email esteja listado em seu respectivo perfil. Esse grupo é selecionado no campo **[!UICONTROL Supervisor(es)]** das propriedades do fluxo de trabalho.
* descrição

## Configurações de segmentação

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Configurações de segmentação"
>abstract="A confirmar"

* targeting dimension:

   Durante as operações de segmentação de dados, a chave de direcionamento é mapeada para uma dimensão de filtro. O targeting dimension permite definir o público alvo da operação: recipients, beneficiários de contrato, operadores, assinantes etc. A dimensão de filtro permite selecionar o público com base em determinados critérios: titulares de contratos, assinantes de boletins informativos, etc.

* manter resultados: a opção **Manter o resultado de populações intermediárias entre duas execuções** mantém tabelas temporárias entre duas execuções de um fluxo de trabalho.  Está disponível na guia **[!UICONTROL General]** das propriedades do workflow e pode ser usado para desenvolvimento e testes para monitorar dados e verificar resultados. Você pode usar essa opção em ambientes de desenvolvimento, mas nunca usá-la em ambientes de produção. Manter tabelas temporárias pode resultar no aumento significativo do tamanho de banco de dados e, por fim, atingir o limite de tamanho. Além disso, o backup ficará lento.

   Somente as tabelas de trabalho da última execução do workflow são mantidas. As tabelas de trabalho das execuções anteriores são removidas pelo workflow **[!UICONTROL cleanup]**, executado diariamente.

   >[!CAUTION]
   >
   >Essa opção **nunca** deve ser selecionada em um fluxo de trabalho de **produção**. Essa opção é usada para analisar os resultados e é projetada apenas para fins de teste e, portanto, deve ser usada apenas em ambientes de desenvolvimento ou de preparo.

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
