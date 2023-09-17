---
audience: end-user
title: Usar a atividade de fluxo de trabalho Combinar
description: Saiba como usar a atividade de fluxo de trabalho Combinar
badge: label="Beta"
source-git-commit: b81fb2bf4cc0accadce47627865379e564c8bd94
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 81%

---


# Combinar {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Combinar atividade"
>abstract="A variável **Combinar** A atividade de permite executar a segmentação na população de entrada. Dessa forma, é possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários targets."


A variável **Combinar** a atividade é um **Direcionamento** atividade. Essa atividade permite executar a segmentação na população de entrada. Dessa forma, é possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários públicos-alvo. Estes são os tipos de segmentação disponíveis:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* A **União** permite reagrupar o resultado de várias atividades em um só público-alvo.
* A **Interseção** permite manter somente os elementos comuns às diferentes populações de entrada na atividade.
* A **Exclusão** permite excluir elementos de uma população de acordo com determinados critérios.

## Configuração geral {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Opções de mesclagem de interseção"
>abstract="A Interseção permite manter somente os elementos comuns às diferentes populações de entrada na atividade. Na seção Conjuntos para unir, marque todas as atividades anteriores que você deseja unir."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Opções de mesclagem de exclusão"
>abstract="A Exclusão permite excluir elementos de uma população de acordo com determinados critérios. Na seção Conjuntos para unir, marque todas as atividades anteriores que você deseja unir."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Selecionar o tipo de segmentação"
>abstract="Selecione como combinar públicos: união, interseção ou exclusão."

Siga estas etapas comuns para começar a configurar a atividade **Combinar**:

1. Adicione várias atividades, por exemplo, **Criar público-alvo**, para formar pelo menos duas ramificações de execução diferentes.
1. Adicione uma atividade **Combinar** a qualquer uma das ramificações anteriores.
1. Selecione o tipo de segmentação: [união](#union), [interseção](#intersection) ou [exclusão](#exclusion).
1. Clique em **Continuar**.
1. Na seção **Conjuntos para unir**, marque todas as atividades anteriores que deseja unir.

## União {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Opções de reconciliação de interseção"
>abstract="Selecione o tipo de reconciliação para definir como as duplicatas são tratadas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Opções de reconciliação"
>abstract="Selecione o **Tipo de reconciliação** para definir como lidar com duplicatas."

No **Combinar** atividade, você pode configurar um **União**. Para isso, é necessário selecionar o **Tipo de reconciliação** para definir como as duplicatas são tratadas:

* **Somente chaves**: este é o modo padrão. A atividade só mantém um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Essa opção só poderá ser usada se as populações de entrada forem homogêneas.
* **Uma seleção de colunas**: selecione esta opção para definir a lista de colunas em que a reconciliação de dados será aplicada. Primeiro, selecione o conjunto principal (que contém os dados de origem) e, em seguida, as colunas a serem usadas para a união.

## Interseção {#intersection}

No **Combinar** atividade, você pode configurar um **Interseção**. Para isso, você precisa seguir as etapas adicionais abaixo:

1. Selecione o **Tipo de reconciliação** para definir como as duplicatas são tratadas. Consulte a seção [União](#union).
1. Marque a opção **Gerar complemento** se desejar processar a população restante. O complemento conterá a união dos resultados de todas as atividades de entrada menos a intersecção. Será adicionada uma transição de saída adicional à atividade.

## Exclusão {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Regras de  exclusão"
>abstract="Quando necessário, é possível manipular tabelas de entrada. De fato, para excluir um público-alvo de outra dimensão, esse público-alvo deve ser devolvido à mesma dimensão de direcionamento como público-alvo principal. Para fazer isso, clique em Adicionar uma regra na seção Regras de exclusão e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma união."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Selecionar conjuntos para combinar"
>abstract="Na seção **Conjuntos para unir**, selecione o **Conjunto principal** das transições de entrada. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_exclusion"
>title="Regras de  exclusão"
>abstract="Quando necessário, é possível manipular tabelas de entrada. De fato, para excluir um público-alvo de outra dimensão, esse público-alvo deve ser devolvido à mesma dimensão de direcionamento como público-alvo principal. Para fazer isso, clique em Adicionar uma regra na seção Regras de exclusão e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma união."



No **Combinar** atividade, você pode configurar um **Exclusão**. Para isso, você precisa seguir as etapas adicionais abaixo:

1. Na seção **Conjuntos para unir**, selecione o **Conjunto principal** das transições de entrada. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal.
1. Quando necessário, é possível manipular tabelas de entrada. De fato, para excluir um público-alvo de outra dimensão, esse público-alvo deve ser devolvido à mesma dimensão de direcionamento como público-alvo principal. Para fazer isso, clique em **Adicionar uma regra** na seção **Regras de exclusão** e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma união.
1. Marque a opção **Gerar complemento** se desejar processar a população restante. Consulte a seção [Interseção](#intersection).

## Exemplos

No exemplo a seguir, estamos usando uma variável **Combinar** atividade e adicionamos um **união** para recuperar todos os perfis dos dois queries: pessoas entre 18 e 27 anos e pessoas entre 34 e 40 anos.

![](../assets/workflow-union-example.png)

O exemplo a seguir mostra a **interseção** entre duas atividades de consulta. Ela está sendo usada aqui para recuperar perfis com idade entre 18 e 27 anos cujo endereço de email foi fornecido.

![](../assets/workflow-intersection-example.png)

O exemplo de **exclusão** a seguir mostra duas consultas configuradas para filtrar perfis com idade entre 18 e 27 anos e que possuem um domínio de email Adobe. Os perfis com um domínio de email inválido são excluídos do primeiro conjunto.

![](../assets/workflow-exclusion-example.png)


