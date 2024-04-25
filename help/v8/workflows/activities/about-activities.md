---
audience: end-user
title: Trabalhar com atividades de fluxo de trabalho
description: Saiba como usar as atividades de fluxo de trabalho
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 35%

---


# Sobre atividades de fluxo de trabalho {#workflow-activities}

As atividades de fluxo de trabalho são agrupadas em três categorias. Dependendo do contexto, as atividades disponíveis podem ser diferentes.

Todas as atividades estão detalhadas nas seções abaixo:

* [Atividades de direcionamento e gestão de dados](#targeting)
* [Atividades do canal](#channel)
* [Atividades de controle de fluxo](#flow-control)

![](../assets/workflow-activities.png)

## Atividades de direcionamento e gestão de dados {#targeting}

Essas atividades são específicas para direcionar, manipular e enriquecer dados de população. Elas permitem criar uma ou mais direções definindo um público-alvo e dividindo ou combinando esses públicos-alvo usando operações de interseção, união ou exclusão.

* Use o [Salvar público-alvo](save-audience.md) atividade para atualizar um público-alvo ou criar um novo público-alvo a partir da população computada upstream em um fluxo de trabalho.
* Use o [Criar público-alvo](build-audience.md) atividade para definir seu público-alvo. Você pode selecionar um público existente ou usar o modelador de consultas para definir sua própria consulta.
* Use o [Combinar](combine.md) atividade para executar a segmentação na população de entrada. Você pode usar uma união, uma interseção ou uma exclusão.
* Use o [Split](split.md) atividade para segmentar a população recebida em vários subconjuntos.
* Use o [Reconciliação](reconciliation.md) atividade para definir o link entre os dados no banco de dados do Adobe Campaign e os dados em uma tabela de trabalho, por exemplo, dados carregados de um arquivo externo.
* Use o [Enriquecimento](enrichment.md) atividade para definir dados adicionais a serem processados no fluxo de trabalho. Com essa atividade, você pode aproveitar a transição de entrada e configurar a atividade para concluir a transição de saída com dados adicionais.
* Use o [Desduplicação](deduplication.md) atividade para excluir duplicados no(s) resultado(s) das atividades de entrada.
* Use o [Alterar dimensão](change-dimension.md) atividade para alterar o targeting dimension enquanto você constrói seu fluxo de trabalho.
* Use o [Carregar arquivo](load-file.md) para trabalhar com perfis e dados armazenados em um arquivo externo.

## Atividades do canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais. Você pode combinar atividades de canal na tela para criar workflows entre canais que podem acionar ações com base no comportamento do cliente. As seguintes **Canal** Atividades estão disponíveis: Notificações por push por email, SMS, Android e iOS. [Saiba como configurar um delivery no contexto de um workflow](channels.md).

## Atividades de controle de fluxo {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Finalizar atividade"
>abstract="A atividade **Fim** permite marcar graficamente o final de um fluxo de trabalho. Essa atividade não tem impacto funcional e, portanto, é opcional."

As atividades a seguir são específicas para organizar e executar fluxos de trabalho. Sua principal tarefa é coordenar as outras atividades:

* Use o [Scheduler](scheduler.md) atividade a ser agendada quando o fluxo de trabalho é iniciado.
* Use o [Associação AND](and-join.md) atividade para sincronizar várias ramificações de execução de um fluxo de trabalho.
* Adicionar um **Fim** atividade para marcar graficamente o fim de um workflow. Essa atividade não tem impacto funcional e, portanto, é opcional.
* Use o [Bifurcar](fork.md) atividade para criar transições de saída para iniciar várias atividades ao mesmo tempo.
* Adicionar um [Aguardar](wait.md) para pausar temporariamente a execução de uma parte de um fluxo de trabalho.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activities + short description + ref to section
-->

