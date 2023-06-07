---
audience: end-user
title: Usar a atividade do workflow Enrichment
description: Saiba como usar a atividade de workflow de enriquecimento
badge: label="Alpha" type="Positive"
source-git-commit: 773d2476232f4e0609346f4f4518c3250c26985a
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 28%

---


# Enriquecimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Enriquecimento atividade"
>abstract="A atividade Enriquecimento permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente, é usado em um workflow após o direcionamento de atividades.<br/>Depois que os dados de enriquecimento tiverem sido adicionados ao fluxo de trabalho, eles poderão ser usados nas atividades adicionadas após a atividade de Enriquecimento para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades, ou para criar mensagens e campanhas de marketing personalizadas que tenham mais probabilidade de ressoar com seu público-alvo."

A variável **Enriquecimento** a atividade é um **Direcionamento** atividade. Ele permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente, é usado em um workflow após atividades de segmentação.

Os dados de Enriquecimento podem vir de:

* **Da mesma tabela de trabalho** como o direcionado para o seu fluxo de trabalho:

   *Direcione um grupo de clientes e adicione o campo &quot;Data de nascimento&quot; à tabela de trabalho atual*

* **De outra tabela de trabalho**:

   *Direcione um grupo de clientes e adicione os campos &quot;Quantidade&quot; e &quot;Tipo de produto&quot; da tabela &quot;Compra&quot;*.

Após adicionar os dados de enriquecimento ao workflow, eles poderão ser usados nas atividades adicionadas após o **Enriquecimento** atividade para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades ou para criar mensagens e campanhas de marketing personalizadas com maior probabilidade de repercutir com seu público-alvo.

Por exemplo, você pode adicionar à tabela de trabalho do fluxo de trabalho as informações relacionadas às compras dos clientes e usar esses dados para personalizar emails com a compra mais recente ou a quantidade gasta nessas compras.

## Configuração geral

Siga estas etapas para configurar o **Enriquecimento** atividade:

1. Adicione atividades como **Criar público-alvo** e **Combinar** atividades.
1. Adicionar um **Enriquecimento** atividade.
1. Clique em **Adicionar dados de enriquecimento**.

![](../assets/workflow-enrichment1.png)

Você pode selecionar dois tipos de dados: um único atributo da target dimension ou um link de coleção.

## Atributo único

Aqui, estamos apenas adicionando um único atributo de enriquecimento, por exemplo, a data de nascimento. Siga estas etapas:

1. Clique dentro do **Atributo** campo.
1. Selecione um campo simples do targeting dimension, a data de nascimento em nosso exemplo.
1. Clique em **Confirmar**.

![](../assets/workflow-enrichment2.png)

## Link da coleção

Neste caso de uso mais complexo, selecionaremos um link de coleção que é um link com uma cardinalidade 1-N entre as tabelas. Vamos recuperar as três compras mais recentes que custam menos de US$ 100. Para isso, é necessário definir:

* um atributo: o **Valor total** campo
* o número de linhas a serem recuperadas: 3
* um filtro: filtrar itens maiores que 100$
* uma classificação: classificação descendente no **Data do pedido** campo.

Siga estas etapas:

### Adicionar o atributo

É aqui que você seleciona o link de coleção para usar como dados de enriquecimento.

1. Clique dentro do **Atributo** campo.
1. Clique em **Exibir atributos avançados**.
1. Selecione o **Valor total** do campo **Compras** tabela.

![](../assets/workflow-enrichment3.png)

### Definir as configurações da coleção

Em seguida, defina como os dados são coletados e o número de registros a serem recuperados.

1. Selecionar **Coletar dados** no **Selecionar como os dados são coletados** menu suspenso.
1. Digite &quot;3&quot; na caixa **Linhas a serem recuperadas (Colunas a serem criadas)** campo.

![](../assets/workflow-enrichment4.png)

Se quiser, por exemplo, obter o valor médio de compras de um cliente, selecione **Dados agregados** em vez disso, selecione **Média** no **Função agregada** menu suspenso.

![](../assets/workflow-enrichment5.png)

### Definir os filtros

Aqui, definimos o valor máximo do atributo. Filtramos itens maiores que US$ 100.

1. Clique em **Editar filtros**.
1. Adicione os dois filtros a seguir: **Valor total** existe E **Valor total** é inferior a 100. O primeiro filtra os valores NULL como eles seriam exibidos como o maior valor.
1. Clique em **Confirmar**.

![](../assets/workflow-enrichment6.png)

### Definir a classificação

Agora precisamos aplicar a classificação para recuperar os três **mais recente** compras.

1. Ativar o **Ativar classificação** opção.
1. Clique dentro do **Atributo** campo.
1. Selecione o **Data do pedido** campo.
1. Clique em **Confirmar**.
1. Selecionar **Decrescente** do **Ordenar** menu suspenso.

![](../assets/workflow-enrichment7.png)

<!--
cardinality between the tables (1-N)
1. select attribute to use as enrichment data

    display advanced fields option
    i button

    note: attributes from the target dimension

1. Select how the data is collected
1. number of records to retrieve if want to retrieve a collection of multiple records
1. Apply filters and build rule

    select an existing filter
    save the filter for reuse
    view results of the filter visually or in code view

1. sort records using an attribute

leverage enrichment data in campaign

where we can use the enrichment data: personalize email, other use cases?

## Example

-->