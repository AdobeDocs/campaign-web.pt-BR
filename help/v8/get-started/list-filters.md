---
audience: end-user
title: Procurar e filtrar listas
description: Saiba como procurar e filtrar listas no Campaign Web v8
exl-id: 46b83e8c-6c8c-40a1-a08b-9d0b438b80cb
source-git-commit: 1cec57c38b5f196db0881c498044fc9b999ed3b0
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 100%

---

# Procurar e filtrar listas {#list-screens}

A maioria dos links do menu de navegação esquerdo exibe listas de objetos, como a lista de **Entregas** ou **Campanhas**. Algumas dessas telas de lista são de somente leitura. É possível personalizar a exibição das listas e filtrá-las como detalhado abaixo.

## Personalizar telas de lista {#custom-lists}

As listas são exibidas em colunas. É possível exibir informações adicionais alterando a configuração da coluna. Para fazer isso, clique no ícone de **Configurar coluna para um layout personalizado** no canto superior direito da lista.

[A captura de tela mostra o ícone de “Configurar coluna” usado para personalizar o layout das colunas da lista.](assets/config-columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Na tela **Configurar colunas**, adicione ou remova colunas e altere a ordem na qual elas são exibidas.

Você pode alterar a ordem da lista ao **arrastar e soltar** ou com as **setas para cima e para baixo** conforme mostrado abaixo:

[A captura de tela demonstra como reordenar as colunas da lista, usando arrastar e soltar, ou os botões de seta.](assets/list-reorder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Por exemplo, para estas configurações:

[A captura de tela exibe um exemplo de configurações das colunas na tela “Configurar colunas”.](assets/columns.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

A lista mostrará as seguintes colunas:

[A captura de tela mostra a lista resultante, com colunas definidas de acordo com as configurações do exemplo.](assets/column-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

## Classificação de dados {#sort-lists}

Você pode classificar itens na lista clicando em qualquer cabeçalho de coluna. Uma seta é exibida (para cima ou para baixo), indicando que a lista está ordenada nessa coluna. 

Para colunas numéricas ou de datas, a seta para **cima** indica que a lista está ordenada em ordem crescente, enquanto a seta para **baixo** indica ela está em ordem decrescente. Para strings ou colunas alfanuméricas, os valores são listados em ordem alfabética.

## Filtros {#list-built-in-filters}

Para encontrar itens mais rapidamente, você pode usar a barra de pesquisa ou os filtros personalizados integrados para adaptar a lista com base em critérios contextuais.

[A captura de tela mostra as opções de filtro disponíveis para refinar a exibição de lista.](assets/filter.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Informações detalhadas sobre como usar filtros e criar os seus próprios filtros personalizados estão disponíveis [nesta seção](../query/filter.md).

<!--
## Use advanced attributes {#adv-attributes}

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Display advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Rule builder advanced fields"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Rule builder advanced attributes"
>abstract="Only the most common attributes are displayed by default in the attribute list. Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links."

Only the most common attributes are displayed by default in the attribute list and filter configuration screens. Attributes set as `advanced` attributes in the data schema are hidden from the configuration screens.

Activate the **Display advanced attributes** toggle to see all available attributes for the current list in the left palette of the rule builder, such as nodes, groupings, 1-1 links, 1-N links. The attribute list updates instantly.

[The screenshot shows the Display advanced attributes toggle used to reveal hidden attributes in the rule builder palette.](assets/adv-toggle.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}
-->