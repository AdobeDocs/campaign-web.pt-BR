---
audience: end-user
title: Trabalhar com atividades de fluxo de trabalho
description: Saiba como usar as atividades de fluxo de trabalho
badge: label="Beta"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: a8b73ba5664eedf473f09050602a61895993663e
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 83%

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

* A variável [Salvar público-alvo](save-audience.md) A atividade permite atualizar um público-alvo ou criar um novo público-alvo a partir da população computada upstream em um fluxo de trabalho.
* A atividade [Criar público-alvo](build-audience.md) permite definir a população de público-alvo. Você pode selecionar um público-alvo existente ou usar o criador de regras para definir sua própria consulta.
* A atividade [Combinar](combine.md) permite executar a segmentação na população de entrada. Você pode usar uma união, uma interseção ou uma exclusão.
* A atividade de [Divisão](split.md) permite segmentar a população recebida em vários subconjuntos.
* A atividade [Enriquecimento](enrichment.md) permite definir dados adicionais a serem processados no fluxo de trabalho. Com essa atividade, você pode aproveitar a transição de entrada e configurar a atividade para concluir a transição de saída com dados adicionais.
* A variável [Desduplicação](deduplication.md) A atividade de permite excluir duplicados no(s) resultado(s) das atividades de entrada.
* A variável [Alterar dimensão](change-dimension.md) A atividade permite alterar o targeting dimension à medida que você constrói seu fluxo de trabalho.

## Atividades do canal {#channel}

O Adobe Campaign Web permite automatizar e executar campanhas de marketing em vários canais, como email, SMS ou push. É possível combinar atividades do canal na tela para criar fluxos de trabalho entre canais que podem iniciar ações com base no comportamento do cliente.

As seguintes atividades do **canal** estão disponíveis:

* Email
* Push
* SMS

Consulte esta [seção](channels.md).

## Atividades de controle de fluxo {#flow-control}


>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Finalizar atividade"
>abstract="A atividade **Fim** permite marcar graficamente o final de um fluxo de trabalho. Essa atividade não tem impacto funcional e, portanto, é opcional."

As atividades a seguir são específicas para organizar e executar fluxos de trabalho. Sua principal tarefa é coordenar as outras atividades:

* A variável [Scheduler](scheduler.md) A atividade permite programar quando o workflow será iniciado.
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

