---
audience: end-user
title: Trabalhar com atividades de fluxo de trabalho
description: Saiba como usar as atividades de fluxo de trabalho
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 32%

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

* [Criar público-alvo](build-audience.md): defina sua população de destino. Você pode selecionar um público existente ou usar o modelador de consultas para definir sua própria consulta.
* [Alterar fonte de dados](change-data-source.md): altere a fonte de dados da tabela de Trabalho do seu fluxo de trabalho.&quot;
* [Alterar dimensão](change-dimension.md): altere a targeting dimension enquanto você constrói seu fluxo de trabalho.
* [Combinar](combine.md): executar segmentação na população de entrada. Você pode usar uma união, uma interseção ou uma exclusão.
* [Desduplicação](deduplication.md): excluir duplicados no(s) resultado(s) das atividades de entrada.
* [Enriquecimento](enrichment.md): defina dados adicionais para processar em seu fluxo de trabalho. Com essa atividade, você pode aproveitar a transição de entrada e configurar a atividade para concluir a transição de saída com dados adicionais.
* [Consulta incremental](incremental-query.md): consulte o banco de dados de acordo com o agendamento. Todas as vezes que essa atividade é executada, os resultados das execuções anteriores são excluídos. Ela permite direcionar somente elementos novos.
* [Reconciliação](reconciliation.md): defina o vínculo entre os dados no banco de dados do Adobe Campaign e os dados em uma tabela de trabalho, por exemplo, dados carregados de um arquivo externo.
* [Salvar público-alvo](save-audience.md): atualize um público-alvo existente ou crie um novo público-alvo a partir da população computada upstream em um fluxo de trabalho.
* [Split](split.md): segmente a população de entrada em vários subconjuntos.

## Atividades de gerenciamento de dados {#data}

Essas atividades são específicas para manipular e enriquecer dados de população.

* [Extrair arquivo](extract-file.md): exporte dados do Adobe Campaign para outro sistema como um arquivo externo.
* [Carregar arquivo](load-file.md): trabalhar com perfis e dados armazenados em um arquivo externo.
* [Transferir arquivo](transfer-file.md): receber ou enviar arquivos, testar a presença de arquivos ou listar arquivos em um servidor. O protocolo usado pode ser o protocolo servidor para servidor ou o protocolo HTTP.
* [Código JavaScript](javascript-code.md): execute um trecho de código JavaScript no contexto de um fluxo de trabalho.
* [Serviços de assinatura](subscription-services.md): assine ou cancele a assinatura de vários perfis para/de um serviço em uma única ação.
* [Atualizar dados](update-data.md): execute atualizações em massa nos campos do banco de dados. Várias opções permitem personalizar a atualização de dados.

## Atividades do canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais. Você pode combinar atividades de canal na tela para criar workflows entre canais que podem acionar ações com base no comportamento do cliente. As seguintes atividades do **Canal** estão disponíveis: notificações por push de email, SMS, Android e iOS. [Saiba como configurar uma entrega no contexto de um fluxo de trabalho](channels.md).

## Atividades de controle de fluxo {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Finalizar atividade"
>abstract="A atividade **Fim** permite marcar graficamente o final de um fluxo de trabalho. Essa atividade não tem impacto funcional e, portanto, é opcional."

As atividades a seguir são específicas para organizar e executar fluxos de trabalho. Sua principal tarefa é coordenar as outras atividades:

* [And-join](and-join.md): sincroniza várias ramificações de execução de um fluxo de trabalho.
* **Fim**: marca graficamente o fim de um fluxo de trabalho. Esta atividade não tem impacto funcional e, portanto, é opcional
* [Sinal externo](external-signal.md): acione a execução de um fluxo de trabalho a partir de outro fluxo de trabalho ou uma chamada de API.
* [Bifurcação](fork.md): crie transições de saída para iniciar várias atividades ao mesmo tempo.
* [Agendador](scheduler.md): agenda quando o fluxo de trabalho é iniciado.
* [Test](test.md): habilitar transições com base em condições especificadas.
* [Aguardar](wait.md): pausar momentaneamente a execução de uma parte de um fluxo de trabalho.
