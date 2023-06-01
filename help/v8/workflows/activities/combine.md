---
audience: end-user
title: Usar a atividade Combinar workflow
description: Saiba como usar a atividade Combinar workflow
badge: label="Alpha" type="Positive"
source-git-commit: 98b4b43427266d5f9580733d4674db938713296d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 21%

---


# Combinar {#combine}

Essa atividade permite processar conjuntos em dados de entrada. Dessa forma, é possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários targets. Estes são os tipos de segmentação disponíveis:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* A variável **União** permite reagrupar o resultado de várias atividades em um único público-alvo.
* A variável **Interseção** O permite manter somente os elementos comuns aos diferentes preenchimentos de entrada na atividade.
* A variável **Exclusão** O permite excluir elementos de uma população de acordo com determinados critérios.

## Configuração

Siga estas etapas para configurar o **Combinar** atividade:

1. Adicione várias atividades, como **Criar público-alvo** para formar pelo menos duas ramificações de execução diferentes.
1. Adicionar um **Combinar** para qualquer uma das transições de segmentação anteriores.
1. Selecione o tipo de segmentação: união, interseção ou exclusão.
1. Clique em **Continue**.
1. No **Conjuntos para ingressar** marque todas as atividades anteriores nas quais deseja participar.

Para o **União** e **Interseção**, é necessário selecionar o **Tipo de reconciliação** para definir como as duplicatas são tratadas:

* Keys only: este é o modo padrão. A atividade só mantém um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Essa opção só poderá ser usada se as populações de entrada forem homogêneas.
* A selection of columns: selecione esta opção para definir a lista de colunas em que a reconciliação de dados será aplicada. Primeiro, selecione o conjunto principal (que contém os dados de origem) e, em seguida, as colunas a serem usadas para a junção.

Para o **Interseção** e **Exclusão**, você pode verificar o **Gerar conclusão** opção se desejar processar o público restante. O complemento conterá a união dos resultados de todas as atividades de entrada menos a intersecção. Uma transição de saída adicional será adicionada à atividade.

Para o **Exclusão**, selecione o **Conjunto principal** das transições de entrada, no **Conjuntos para ingressar** seção. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal.

## Exemplos

No exemplo a seguir, adicionamos uma variável **união** que recupera todos os perfis dos dois queries: pessoas entre 18 e 27 anos e pessoas entre 34 e 40 anos.

![](../assets/workflow-union-example.png)

O exemplo a seguir mostra o **interseção** entre duas atividades de query. Ela está sendo usada aqui para recuperar perfis com idade entre 18 e 27 anos e cujo endereço de email foi fornecido.

![](../assets/workflow-intersection-example.png)

As seguintes **exclusão** O exemplo mostra dois queries configurados para filtrar perfis com idade entre 18 e 27 anos e que têm um domínio de email da adobe. Os perfis com um domínio de email da Adobe são excluídos do primeiro conjunto.

![](../assets/workflow-exclusion-example.png)





