---
audience: end-user
title: Trabalhar com atividades de fluxo de trabalho
description: Saiba como usar as atividades de fluxo de trabalho
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 26%

---


# Sobre atividades de fluxo de trabalho {#workflow-activities}

As atividades de fluxo de trabalho são agrupadas em três categorias. Dependendo do contexto, as atividades disponíveis podem ser diferentes.

Todas as atividades estão detalhadas nas seções abaixo:

* [Atividades de direcionamento e gestão de dados](#targeting)
* [Atividades do canal](#channel)
* [Atividades de controle de fluxo](#flow-control)

![](../assets/workflow-activities.png)

## Atividades de direcionamento {#targeting}

Essas atividades são específicas para direcionamento. Elas permitem criar uma ou mais direções definindo um público-alvo e dividindo ou combinando esses públicos-alvo usando operações de interseção, união ou exclusão.

* [Criar público-alvo](build-audience.md): defina a população do target. Você pode selecionar um público existente ou usar o modelador de consultas para definir sua própria consulta.
* [Alterar fonte de dados](change-data-source.md): altere a fonte de dados da tabela de Trabalho do seu fluxo de trabalho.&quot;
* [Alterar dimensão](change-dimension.md): altere o targeting dimension enquanto constrói seu fluxo de trabalho.
* [Combinar](combine.md): execute a segmentação na população de entrada. Você pode usar uma união, uma interseção ou uma exclusão.
* [Desduplicação](deduplication.md): exclua duplicatas no(s) resultado(s) das atividades de entrada.
* [Enriquecimento](enrichment.md): defina dados adicionais para processar no fluxo de trabalho. Com essa atividade, você pode aproveitar a transição de entrada e configurar a atividade para concluir a transição de saída com dados adicionais.
* [Query incremental](incremental-query.md): consulta o banco de dados de acordo com o agendamento. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Ela permite direcionar somente elementos novos.
* [Reconciliação](reconciliation.md): defina o link entre os dados no banco de dados do Adobe Campaign e os dados em uma tabela de trabalho, por exemplo, dados carregados de um arquivo externo.
* [Salvar público-alvo](save-audience.md): atualize um público-alvo ou crie um novo público-alvo a partir da população computada upstream em um fluxo de trabalho.
* [Split](split.md): segmente a população de entrada em vários subconjuntos.

## Atividades de gerenciamento de dados {#data}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Atividades Extrair arquivo e Carregar arquivo"
>abstract="Novas atividades de gestão de dados estão disponíveis em workflows. Use a atividade Extract File para exportar dados do Adobe Campaign para outro sistema como um arquivo externo. Use a atividade Load File para trabalhar com perfis e dados armazenados em um arquivo externo."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

Essas atividades são específicas para manipular e enriquecer dados de população.

* [Extrair arquivo](extract-file.md): exporte dados do Adobe Campaign para outro sistema como um arquivo externo.
* [Carregar arquivo](load-file.md): trabalhe com perfis e dados armazenados em um arquivo externo.
* [Transferir arquivo](transfer-file.md): Receba ou envie arquivos, teste a presença de arquivos ou liste arquivos em um servidor. O protocolo usado pode ser protocolo servidor a servidor ou protocolo HTTP.
* [Código JavaScript](javascript-code.md): executa um trecho de código JavaScript no contexto de um workflow.
* [Serviços de assinatura](subscription-services.md): assine ou cancele a assinatura de vários perfis para/de um serviço em uma única ação.
* [Atualizar dados](update-data.md): Execute atualizações em massa nos campos no banco de dados. Várias opções permitem personalizar a atualização de dados.

## Atividades do canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais. Você pode combinar atividades de canal na tela para criar workflows entre canais que podem acionar ações com base no comportamento do cliente. As seguintes **Canal** Atividades estão disponíveis: Notificações por push por email, SMS, Android e iOS. [Saiba como configurar um delivery no contexto de um workflow](channels.md).

## Atividades de controle de fluxo {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Atividades avançadas de fluxo de trabalho"
>abstract="Agora você pode configurar atividades de Teste, Código JavaScript e Sinal externo em um workflow. Use a atividade Test para habilitar transições de fluxo de trabalho com base em condições. Adicione uma atividade JavaScript Code para executar um trecho de código JS no contexto do workflow. Configure uma atividade External Signal para acionar a execução do workflow a partir de uma API ou de outro workflow."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"



>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Finalizar atividade"
>abstract="A atividade **Fim** permite marcar graficamente o final de um fluxo de trabalho. Essa atividade não tem impacto funcional e, portanto, é opcional."

As atividades a seguir são específicas para organizar e executar fluxos de trabalho. Sua principal tarefa é coordenar as outras atividades:

* [Associação AND](and-join.md): sincronize várias ramificações de execução de um fluxo de trabalho.
* **Fim**: marca graficamente o fim de um workflow. Esta atividade não tem impacto funcional e, portanto, é opcional
* [Sinal externo](external-signal.md): acione a execução de um workflow a partir de outro workflow ou uma chamada à API.
* [Bifurcar](fork.md): crie transições de saída para iniciar várias atividades ao mesmo tempo.
* [Scheduler](scheduler.md): agenda quando o fluxo de trabalho é iniciado.
* [Teste](test.md): ative as transições com base nas condições especificadas.
* [Aguardar](wait.md): pausa momentaneamente a execução de uma parte de um workflow.
