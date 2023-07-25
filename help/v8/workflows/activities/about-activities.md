---
audience: end-user
title: Trabalhar com atividades de fluxo de trabalho
description: Saiba como usar as atividades de fluxo de trabalho
badge: label="Alfa"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 96%

---


# Sobre atividades de fluxo de trabalho {#workflow-activities}

As atividades de fluxo de trabalho são agrupadas em três categorias. Dependendo do contexto, as atividades disponíveis podem ser diferentes.

Todas as atividades estão detalhadas nas seções abaixo:

* [Atividades de direcionamento](#targeting)
* [Atividades do canal](#channel)
* [Atividades de controle de fluxo](#flow-control)

![](../assets/workflow-activities.png)

## Atividades de direcionamento {#targeting}

Essas atividades são específicas para direcionar, manipular e enriquecer dados de população. Elas permitem criar uma ou mais direções definindo um público-alvo e dividindo ou combinando esses públicos-alvo usando operações de interseção, união ou exclusão.

* A atividade [Criar público-alvo](build-audience.md) permite definir a população de público-alvo. Você pode selecionar um público-alvo existente ou usar o criador de regras para definir sua própria consulta.
* A atividade [Combinar](combine.md) permite executar a segmentação na população de entrada. Você pode usar uma união, uma interseção ou uma exclusão.
* A atividade [Enriquecimento](enrichment.md) permite definir dados adicionais a serem processados no fluxo de trabalho. Com essa atividade, você pode aproveitar a transição de entrada e configurar a atividade para concluir a transição de saída com dados adicionais.
* A variável [Split](split.md) A atividade permite segmentar a população recebida em vários subconjuntos.

## Atividades do canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais, como email, SMS ou push. É possível combinar atividades do canal na tela para criar fluxos de trabalho entre canais que podem iniciar ações com base no comportamento do cliente.

As seguintes atividades do **canal** estão disponíveis:

* Email
* Push
* SMS

Consulte esta [seção](enrichment.md).

## Atividades de controle de fluxo {#flow-control}

As atividades a seguir são específicas para organizar e executar fluxos de trabalho. Sua principal tarefa é coordenar as outras atividades:

* A atividade [AND-join](and-join.md) permite sincronizar várias ramificações de execução de um fluxo de trabalho.
* A atividade **Fim** permite marcar graficamente o final de um fluxo de trabalho. Essa atividade não tem impacto funcional e, portanto, é opcional.
* A atividade [Bifurcação](fork.md) permite criar transições de saída para iniciar várias atividades ao mesmo tempo.
* A atividade [Aguardar](wait.md) suspende temporariamente a execução de uma parte do fluxo de trabalho.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

