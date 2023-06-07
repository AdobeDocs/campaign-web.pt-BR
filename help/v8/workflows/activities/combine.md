---
audience: end-user
title: Usar a atividade Combinar workflow
description: Saiba como usar a atividade Combinar workflow
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 22%

---


# Combinar {#combine}

Essa atividade permite executar a segmentação na população de entrada. Dessa forma, é possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários targets. Estes são os tipos de segmentação disponíveis:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* A variável **União** permite reagrupar o resultado de várias atividades em um único público-alvo.
* A variável **Interseção** O permite manter somente os elementos comuns aos diferentes preenchimentos de entrada na atividade.
* A variável **Exclusão** O permite excluir elementos de uma população de acordo com determinados critérios.

## Configuração geral {#general}

Siga estas etapas comuns para começar a configurar o **Combinar** atividade:

1. Adicione várias atividades, como **Criar público-alvo** para formar pelo menos duas ramificações de execução diferentes.
1. Adicionar um **Combinar** atividade a qualquer uma das ramificações anteriores.
1. Selecione o tipo de segmentação: [união](#union), [interseção](#intersection) ou [exclusão](#exclusion).
1. Clique em **Continue**.
1. No **Conjuntos para ingressar** marque todas as atividades anteriores nas quais deseja participar.

## União {#union}

Para o **União**, é necessário selecionar o **Tipo de reconciliação** para definir como as duplicatas são tratadas:

* **Chaves somente**: este é o modo padrão. A atividade só mantém um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Essa opção só poderá ser usada se as populações de entrada forem homogêneas.
* **Uma seleção de colunas**: selecione esta opção para definir a lista de colunas em que a reconciliação de dados será aplicada. Primeiro, selecione o conjunto principal (que contém os dados de origem) e, em seguida, as colunas a serem usadas para a junção.

## Intersecção {#intersection}

Para o **Interseção**, é necessário seguir estas etapas adicionais:

1. Selecione o **Tipo de reconciliação** para definir como as duplicatas são tratadas. Consulte a [União](#union) seção.
1. Você pode verificar o **Gerar conclusão** opção se desejar processar o público restante. O complemento conterá a união dos resultados de todas as atividades de entrada menos a intersecção. Uma transição de saída adicional será adicionada à atividade.

## Exclusão {#exclusion}

Para o **Exclusão**, é necessário seguir estas etapas adicionais:

1. No **Conjuntos para ingressar** , selecione a **Conjunto principal** das transições de entrada. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal.
1. Quando necessário, é possível manipular tabelas de entrada. De fato, para excluir um target de outra dimensão, esse target deve ser devolvido ao mesmo targeting dimension como o target principal. Para fazer isso, clique em **Adicionar uma regra** no **Regras de exclusão** e especifique as condições de alteração da dimensão. A reconciliação de dados é realizada por meio de um atributo ou uma junção.
1. Você pode verificar o **Gerar conclusão** opção se desejar processar o público restante. Consulte a [Interseção](#intersection) seção.

## Exemplos

No exemplo a seguir, adicionamos uma variável **união** que recupera todos os perfis dos dois queries: pessoas entre 18 e 27 anos e pessoas entre 34 e 40 anos.

![](../assets/workflow-union-example.png)

O exemplo a seguir mostra o **interseção** entre duas atividades de query. Ela está sendo usada aqui para recuperar perfis com idade entre 18 e 27 anos e cujo endereço de email foi fornecido.

![](../assets/workflow-intersection-example.png)

As seguintes **exclusão** O exemplo mostra dois queries configurados para filtrar perfis com idade entre 18 e 27 anos e domínio de email Adobe. Os perfis com um domínio de email Adobe são excluídos do primeiro conjunto.

![](../assets/workflow-exclusion-example.png)


