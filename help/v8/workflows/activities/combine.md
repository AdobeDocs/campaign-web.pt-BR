---
audience: end-user
title: Usar a atividade Combinar workflow
description: Saiba como usar a atividade Combinar workflow
badge: label="Alpha" type="Positive"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 29%

---


# Combinar {#combine}

Essa atividade permite processar conjuntos em dados de entrada. Dessa forma, é possível combinar várias populações, excluir parte delas ou manter apenas dados comuns a vários targets. Estes são os tipos de segmentação disponíveis:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* A variável **União** permite reagrupar o resultado de várias atividades em um único público-alvo.
* A variável **Interseção** O permite manter somente os elementos comuns aos diferentes preenchimentos de entrada na atividade.
* A variável **Exclusão** O permite excluir elementos de uma população de acordo com determinados critérios.

Siga estas etapas para configurar o **Combinar** atividade:

1. Adicione **Combinar** para qualquer uma das transições de segmentação anteriores.
1. Selecione o tipo de segmentação: união, interseção ou exclusão.
1. Clique em **Continue**.
1. No **Conjuntos para ingressar** marque todas as atividades anteriores nas quais deseja participar.

Para o **União** e **Interseção**, é necessário selecionar o **Tipo de reconciliação** para definir como as duplicatas são tratadas:

    * Keys only: este é o modo padrão. A atividade só mantém um elemento quando elementos de transições de entrada diferentes têm a mesma chave. Essa opção só poderá ser usada se as populações de entrada forem homogêneas.
    * A selection of columns: selecione esta opção para definir a lista de colunas em que a reconciliação de dados será aplicada. Primeiro, selecione o conjunto principal (que contém os dados de origem) e, em seguida, as colunas a serem usadas para a junção.

Para o **Interseção** e **Exclusão**, você pode verificar o **Gerar conclusão** opção se desejar processar o público restante. O complemento conterá a união dos resultados de todas as atividades de entrada menos a intersecção. Uma transição de saída adicional será adicionada à atividade.

Para o **Exclusão**, selecione o **Conjunto principal** das transições de entrada, no **Conjuntos para ingressar** seção. Esse é o conjunto a partir do qual os elementos são excluídos. Os outros conjuntos correspondem a elementos antes de serem excluídos do conjunto principal.
