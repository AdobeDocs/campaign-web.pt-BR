---
audience: end-user
title: Usar a atividade de fluxo de trabalho Enriquecimento
description: Saiba como usar a atividade de fluxo de trabalho Enriquecimento
exl-id: 02f30090-231f-4880-8cf7-77d57751e824
source-git-commit: fa2d596a36652f504112c7a8543453d845462021
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 47%

---

# Enriquecimento {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment"
>title="Atividade de enriquecimento"
>abstract="A atividade **Enriquecimento** permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente, ela é usada em um fluxo de trabalho após atividades de segmentação."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Atividade de enriquecimento"
>abstract="Depois que os dados de enriquecimento tiverem sido adicionados ao fluxo de trabalho, eles poderão ser usados nas atividades adicionadas após a atividade Enriquecimento para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades, ou para criar mensagens e campanhas de marketing personalizadas que tenham mais probabilidade de ressoar com seu público-alvo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_reconciliation"
>title="Reconciliação de enriquecimento"
>abstract="reconciliação de enriquecimento"

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_simplejoin"
>title="Definição do link"
>abstract="Associação simples"

>[!CONTEXTUALHELP]
>id="acw_targetdata_personalization_enrichmentdata"
>title="Dados de enriquecimento"
>abstract="Selecione os dados a serem usados para enriquecer seu fluxo de trabalho. Você pode selecionar dois tipos de dados de enriquecimento: um único atributo de enriquecimento da dimensão do público-alvo ou um link de coleção, que é um link com uma cardinalidade 1-N entre tabelas."

A atividade **Enriquecimento** é uma atividade de **Direcionamento**. Ela permite aprimorar os dados direcionados com informações adicionais do banco de dados. Normalmente, ela é usada em um fluxo de trabalho após atividades de segmentação.

Os dados de Enriquecimento podem vir:

* **Da mesma tabela de trabalho** como o direcionado para o seu fluxo de trabalho:

  *Direcione um grupo de clientes e adicione o campo &quot;Data de nascimento&quot; à tabela de trabalho atual*.

* **De outra tabela de trabalho**:

  *Direcione um grupo de clientes e adicione os campos &quot;Quantidade&quot; e &quot;Tipo de produto&quot; da tabela &quot;Compra&quot;*.

Após adicionar os dados de enriquecimento ao workflow, eles poderão ser usados nas atividades adicionadas após o **Enriquecimento** atividade para segmentar clientes em grupos distintos com base em seus comportamentos, preferências e necessidades ou para criar mensagens e campanhas de marketing personalizadas com maior probabilidade de repercutir com seu público-alvo.

Por exemplo, você pode adicionar à tabela de trabalho do fluxo de trabalho as informações relacionadas às compras dos clientes e usar esses dados para personalizar emails com a compra mais recente ou a quantidade gasta nessas compras.

## Adicionar uma atividade Enrichment {#enrichment-configuration}

Siga estas etapas para configurar a atividade **Enriquecimento**:

1. Adicione atividades como **Criar público-alvo** e **Combinar**.
1. Adicione uma atividade **Enriquecimento**
1. Se várias transições tiverem sido configuradas no seu fluxo de trabalho, você poderá usar o **[!UICONTROL Conjunto principal]** para definir qual transição deve ser usada como conjunto principal para enriquecer com dados.

## Adicionar dados de enriquecimento {#enrichment-add}

1. Clique em **Adicionar dados de enriquecimento** e selecione o atributo a ser usado para enriquecer os dados.

   Você pode selecionar dois tipos de dados de enriquecimento: um único atributo de enriquecimento da target dimension ou um link de coleção. Cada um desses tipos é detalhado nos exemplos abaixo:
   * [Atributo único de enriquecimento](#single-attribute)
   * [Link da coleção](#collection-link)

   >[!NOTE]
   >
   >A variável **Botão Editar expressão** na tela seleção de atributo, você pode criar expressões avançadas para selecionar o atributo. [Saiba como trabalhar com o editor de expressão](../../query/expression-editor.md)

   ![](../assets/workflow-enrichment1.png)

## Criar vínculos entre tabelas {#create-links}

A variável **[!UICONTROL Definição de link]** permite criar um link entre os dados da tabela de trabalho e o banco de dados do Adobe Campaign. Por exemplo, se carregar dados de um arquivo que contenha o número da conta, o país e o e-mail dos recipients, será necessário criar um link para a tabela do país para atualizar essas informações em seus perfis.

Há vários tipos de links disponíveis:

* **[!UICONTROL Link simples de cardinalidade 1]**: cada registro do conjunto principal pode ser associado a um e a somente um registro dos dados vinculados.
* **[!UICONTROL Link simples de cardinalidade 0 ou 1]**: cada registro do conjunto principal pode ser associado a 0 ou 1 registro dos dados vinculados, mas não a mais de um.
* **[!UICONTROL Link de coleção de cardinalidade N]**: cada registro do conjunto principal pode ser associado a 0, 1 ou mais registros (N) dos dados vinculados.

Para criar um link, siga estas etapas:

1. No **[!UICONTROL Definição de link]** clique na guia **[!UICONTROL Adicionar link]** botão.

   ![](../assets/workflow-enrichment-link.png)

1. No **Tipo de relação** escolha o tipo de link que deseja criar.

1. Identifique o target ao qual deseja vincular o conjunto principal:

   * Para vincular uma tabela existente no banco de dados, escolha **[!UICONTROL Esquema de banco de dados]** e selecione a tabela desejada na **[!UICONTROL Esquema do Target]** campo.
   * Para vincular com dados a partir da transição de entrada, escolha **Esquema temporário** e selecione a transição cujos dados deseja usar.

1. Defina os critérios de reconciliação para corresponder os dados do conjunto principal com o esquema vinculado. Há dois tipos de associações disponíveis:

   * **Junção simples**: selecione um atributo específico para corresponder aos dados dos dois schemas. Clique em **Adicionar associação** e selecione o **Origem** e **Destino** atributos a serem usados como critérios de reconciliação.
   * **Junção avançada**: crie uma associação usando condições avançadas. Clique em **Adicionar associação** e clique no link **Criar condição** botão para abrir o modelador de consultas.

Um exemplo de fluxo de trabalho usando links está disponível na [Exemplos](#link-example) seção.

## Exemplos {#example}

### Atributo único de enriquecimento {#single-attribute}

Nesse caso, estamos apenas adicionando um atributo único de enriquecimento, por exemplo, a data de nascimento. Siga estas etapas:

1. Clique no campo **Atributo**.
1. Selecione um campo simples da dimensão de direcionamento (data de nascimento, em nosso exemplo).
1. Clique em **Confirmar**.

![](../assets/workflow-enrichment2.png)

### Link de coleção {#collection-link}

Neste caso de uso mais complexo, selecionaremos um link de coleção, que é um link com uma cardinalidade 1-N entre tabelas. Vamos recuperar as três compras mais recentes que custam menos de US$ 100. Para isso, é necessário definir:

* um atributo de enriquecimento: o campo **Valor total**
* o número de linhas a serem recuperadas: 3
* um filtro: filtrar itens que custam mais de US$ 100
* uma classificação: classificação decrescente no campo **Data do pedido**.

#### Adicionar o atributo {#add-attribute}

É aqui que você seleciona o link de coleção para usar como dados de enriquecimento.

1. Clique no campo **Atributo**.
1. Clique em **Exibir atributos avançados**.
1. Selecione o campo **Valor total** na tabela **Compras**.

![](../assets/workflow-enrichment3.png)

#### Definir as configurações de coleção{#collection-settings}

Em seguida, defina como os dados são coletados e o número de registros a serem recuperados.

1. Selecione **Coletar dados** no menu suspenso **Selecione como os dados são coletados**.
1. Digite &quot;3&quot; no campo **Linhas a serem recuperadas (Colunas a serem criadas)**.

![](../assets/workflow-enrichment4.png)

Se quiser, por exemplo, obter o valor médio das compras de um cliente, selecione **Dados agregados** em vez disso, e depois selecione **Média** no menu suspenso **Função de agregação**.

![](../assets/workflow-enrichment5.png)

#### Definir os filtros{#collection-filters}

Aqui, definimos o valor máximo do atributo de enriquecimento. Filtramos itens maiores que US$ 100. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md)

1. Clique em **Editar filtros**.
1. Adicione os dois filtros a seguir: **Valor total** existe E **Valor total** é menor que 100. O primeiro filtra os valores NULL, pois seriam exibidos como o maior valor.
1. Clique em **Confirmar**.

![](../assets/workflow-enrichment6.png)

#### Definir a classificação{#collection-sorting}

Agora precisamos aplicar a classificação para recuperar as três compras **mais recentes**.

1. Ative a opção **Habilitar classificação**.
1. Clique no campo **Atributo**.
1. Selecione o campo **Data do pedido**.
1. Clique em **Confirmar**.
1. Selecione **Decrescente** no menu suspenso **Classificar**.

![](../assets/workflow-enrichment7.png)


### Enriquecimento com dados vinculados {#link-example}

O exemplo abaixo mostra um fluxo de trabalho configurado para criar um link entre duas transições. A primeira transição é direcionada a dados de perfil usando uma atividade de Query, enquanto a segunda transição inclui dados de compra armazenados em um arquivo carregado por meio de uma atividade Load file.

* O primeiro **Enriquecimento** atividade vincula nosso conjunto principal (dados do **Query** atividade ) com o schema da variável **Carregar arquivo** atividade. Isso nos permite corresponder cada perfil direcionado pelo query com os dados de compra correspondentes.
* Um segundo **Enriquecimento** atividade é adicionada para enriquecer dados da tabela de workflow com os dados de compra provenientes de **Carregar arquivo** atividade. Isso nos permite usar esses dados em outras atividades do, por exemplo, para personalizar mensagens enviadas aos clientes com informações sobre suas compras.

  ![](../assets/workflow-enrichment-example.png)





<!--

Add other fields
use it in delivery


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
