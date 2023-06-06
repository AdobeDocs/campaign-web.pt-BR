---
audience: end-user
title: Trabalhar com atividades de fluxos de trabalho
description: Saiba como executar atividades de workflow
badge: label="Alpha" type="Positive"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 40ca8ca9825706be7b82a58136627911132bc14a
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 12%

---


# Sobre atividades de fluxo de trabalho {#workflow-activities}

As atividades de workflow são agrupadas em três categorias. Dependendo do contexto, as atividades disponíveis podem ser diferentes.

Todas as atividades estão detalhadas nas seções abaixo:

* [Atividades de direcionamento](#targeting)
* [Atividades de canal](#channel)
* [Atividades de controle de fluxo](#flow-control)

![](../assets/workflow-activities.png)

## Atividades de direcionamento {#targeting}

Essas atividades são específicas para direcionar, manipular e enriquecer dados de população. Eles permitem criar um ou mais públicos-alvo definindo um público-alvo e dividindo ou combinando esses públicos-alvo usando operações de interseção, união ou exclusão.

* A variável [Criar público-alvo](build-audience.md) A atividade permite definir o público-alvo. Você pode selecionar um público existente ou usar o construtor de regras para definir sua própria consulta.
* A variável [Combinar](combine.md) A atividade de permite executar a segmentação na população de entrada. Você pode usar uma união, uma interseção ou uma exclusão.
* A variável [Enriquecimento](enrichment.md) A atividade permite definir dados adicionais a serem processados no fluxo de trabalho. Com essa atividade, você pode aproveitar a transição de entrada e configurar a atividade para concluir a transição de saída com dados adicionais.

## Atividades de canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais, como email, SMS ou push. Você pode combinar atividades de canal na tela para criar workflows entre canais que podem acionar ações com base no comportamento do cliente.

As seguintes **Canal** As atividades do estão disponíveis:

* Email
* Push
* SMS

Consulte esta [seção](enrichment.md).

## Atividades de controle de fluxo {#flow-control}

As atividades a seguir são específicas para organizar e executar workflows. Sua principal tarefa é coordenar as outras atividades:

* A variável [Associação AND](and-join.md) A atividade permite sincronizar várias ramificações de execução de um fluxo de trabalho.
* A variável [Fim](end.md) permite marcar graficamente o final de um workflow. Essa atividade não tem impacto funcional e, portanto, é opcional.
* A variável [Bifurcar](fork.md) permite criar transições de saída para iniciar várias atividades ao mesmo tempo.
* A variável [Aguardar](wait.md) A atividade suspende temporariamente a execução de uma parte do fluxo de trabalho.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

