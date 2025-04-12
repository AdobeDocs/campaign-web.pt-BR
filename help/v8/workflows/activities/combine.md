---
audience: end-user
title: Usar a atividade de fluxo de trabalho Combinar
description: Saiba como usar a atividade de fluxo de trabalho Combinar
exl-id: 7e821678-e6a2-4613-b05e-6ccbe4df41c3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 35%

---

# Combinar {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Atividade de combinar"
>abstract="A atividade **Combinar** permite executar a segmentação na população de entrada. É possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários targets."

A atividade **Combinar** é uma atividade **de Direcionamento**. Essa atividade permite executar a segmentação na população de entrada. É possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários targets. Estes são os tipos de segmentação disponíveis:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* A **União** reagrupa o resultado de várias atividades em um único público-alvo.
* A **Interseção** mantém apenas os elementos comuns aos diferentes preenchimentos de entrada na atividade.
* A **Exclusão** exclui elementos de uma população de acordo com determinados critérios.

## Configurar a atividade Combinar {#combine-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Opções de mesclagem de interseção"
>abstract="A interseção mantém somente os elementos comuns aos diferentes preenchimentos de entrada na atividade. Na seção Sets to join, marque todas as atividades anteriores que deseja unir."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Opções de mesclagem de exclusão"
>abstract="A exclusão exclui elementos de uma população de acordo com determinados critérios. Na seção Sets to join, marque todas as atividades anteriores que deseja unir."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Selecione o tipo de segmentação"
>abstract="Selecione como combinar os públicos-alvo. A **União** reagrupa o resultado de várias atividades em um único público-alvo. A **Interseção** mantém apenas os elementos comuns aos diferentes preenchimentos de entrada na atividade. A **Exclusão** exclui elementos de uma população de acordo com determinados critérios."

Siga estas etapas comuns para configurar a atividade **Combinar**:

![](../assets/workflow-combine.png)

1. Adicione várias atividades, como **Criar público-alvo** atividades, para formar pelo menos duas ramificações de execução diferentes.
1. Adicione uma atividade **Combinar** a qualquer uma das ramificações anteriores.
1. Selecione o tipo de segmentação: [união](#union), [interseção](#intersection) ou [exclusão](#exclusion).
1. Clique em **Continuar**.
1. Na seção **Conjuntos para ingressar**, marque todas as atividades anteriores nas quais deseja ingressar.

## União {#combine-union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Opções de reconciliação"
>abstract="Selecione o **Tipo de reconciliação** para definir como lidar com duplicatas. Por padrão, a opção **Chaves** está ativada, o que significa que a atividade mantém apenas um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Use a opção **Uma seleção de colunas** para definir a lista de colunas nas quais a reconciliação de dados será aplicada."

Na atividade **Combine**, configure uma **Union** selecionando o **Tipo de reconciliação** para definir como as duplicatas são tratadas:

* **Somente chaves**: este é o modo padrão. A atividade mantém apenas um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Essa opção só poderá ser usada se as populações de entrada forem homogêneas.
* **Uma seleção de colunas**: selecione esta opção para definir a lista de colunas em que a reconciliação de dados é aplicada. Primeiro, selecione o conjunto principal (os dados de origem) e, em seguida, as colunas a serem usadas para a associação.

## Interseção {#combine-intersection}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Opções de reconciliação de interseção"
>abstract="Selecione o **Tipo de reconciliação** para definir como lidar com duplicatas. Por padrão, a opção **Chaves** está ativada, o que significa que a atividade mantém apenas um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Use a opção **Uma seleção de colunas** para definir a lista de colunas nas quais a reconciliação de dados será aplicada."

Na atividade **Combinar**, configure uma **Interseção** seguindo estas etapas adicionais:

1. Selecione o **Tipo de reconciliação** para definir como as duplicatas são tratadas. Consulte a seção [União](#union).
1. Marque a opção **Gerar complemento** se desejar processar o público restante. O complemento contém a união dos resultados de todas as atividades de entrada menos a interseção. Em seguida, uma transição de saída adicional é adicionada à atividade.

## Regras de  {#combine-exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Regras de exclusão"
>abstract="Quando necessário, manipule tabelas de entrada. Para excluir um target de outra dimensão, retorne esse target à mesma targeting dimension que o target principal. Clique em Adicionar uma regra na seção Regras de exclusão e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma união."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Selecionar conjuntos a serem combinados"
>abstract="Na seção **Conjuntos para unir**, selecione o **Conjunto principal** das transições de entrada. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Regras de exclusão"
>abstract="Quando necessário, manipule tabelas de entrada. Para excluir um target de outra dimensão, retorne esse target à mesma targeting dimension que o target principal. Clique em Adicionar uma regra na seção Regras de exclusão e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma união."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_complement"
>title="Complemento de geração de combinação"
>abstract="Ative a opção Gerar complemento para processar a população restante em uma transição adicional."

Na atividade **Combinar**, configure uma **Exclusão** seguindo estas etapas adicionais:

1. Na seção **Conjuntos para unir**, selecione o **Conjunto principal** das transições de entrada. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal.
1. Quando necessário, manipule tabelas de entrada. Para excluir um target de outra dimensão, retorne esse target à mesma targeting dimension que o target principal. Clique em **Adicionar uma regra** na seção **Regras de exclusão** e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma união.
1. Marque a opção **Gerar complemento** se desejar processar o público restante. Consulte a seção [Interseção](#intersection).

## Exemplos {#combine-examples}

No exemplo a seguir, uma atividade **Combine** usa uma **Union** para recuperar todos os perfis das duas consultas: pessoas entre 18 e 27 anos e pessoas entre 34 e 40 anos.

![](../assets/workflow-union-example.png)

O exemplo a seguir mostra a **Interseção** entre duas atividades de consulta. Ele recupera perfis entre 18 e 27 anos e cujo endereço de email foi fornecido.

![](../assets/workflow-intersection-example.png)

O exemplo **Exclusão** a seguir mostra duas consultas configuradas para filtrar perfis com idade entre 18 e 27 anos e que têm um domínio de email Adobe. Os perfis com um domínio de email do Adobe são excluídos do primeiro conjunto.

![](../assets/workflow-exclusion-example.png)