---
audience: end-user
title: Criar a primeira consulta usando o modelador de consultas
description: Saiba como criar sua primeira consulta no Adobe Campaign Web query modeler.
source-git-commit: a974221fa5b46ea9463c98724b1f49a7edb0adb7
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 20%

---

# Criar a primeira consulta {#build-query}

Para começar a criar uma consulta, acesse o modelador de consultas do local de sua escolha, dependendo da ação que deseja executar. O modelador de Consulta é aberto com uma tela em branco. Clique no botão + para adicionar o primeiro nó do query.

![](assets/query-add-component.png)

Você pode adicionar dois tipos de elementos:

* Os componentes de filtragem (Condição personalizada, Selecionar público, Filtro predefinido) permitem criar suas próprias regras, selecionar um público ou um filtro predefinido para refinar sua consulta.

  Exemplo *Recipients que assinaram o boletim informativo &quot;Esportes&quot;*. *Recipients que vivem em Nova York*, *Recipients que vivem em São Francisco*

* Os operadores de grupo (AND, OR, EXCEPT) permitem agrupar componentes de filtragem no diagrama para atender às suas necessidades.

  Exemplo: *Recipients que assinaram o boletim informativo &quot;Esportes&quot;**E**que vivem em Nova York **OU**São Francisco*.

As etapas detalhadas sobre como adicionar e combinar componentes de filtragem e operadores de grupo estão disponíveis abaixo.

## Adicionar componentes de filtragem

Os componentes de filtragem permitem refinar a consulta usando:

* **Condições personalizadas**: filtre sua consulta criando sua própria condição com atributos do banco de dados e expressões avançadas.
* **Públicos-alvo**: filtre sua consulta usando um público-alvo existente.
* **Filtro predefinido**: filtre sua query usando os filtros predefinidos existentes.

### Configurar uma condição personalizada

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Condição personalizada"
>abstract="Condição personalizada"

Para filtrar sua consulta usando uma condição personalizada, siga estas etapas:

1. Clique no botão + no nó desejado e selecione **[!UICONTROL Condição personalizada]**.
1. O painel de propriedades de condição personalizada é aberto no lado direito. No campo Atributo, selecione o atributo do banco de dados que você deseja utilizar para criar sua condição.

   Os atributos disponíveis representam todos os campos do banco de dados do Campaign, incluindo campos de tabelas vinculadas à tabela Recipients.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >O botão Edit expression permite aproveitar o editor de expressão da Web do Campaign para definir manualmente uma expressão usando campos do banco de dados e funções auxiliares.

1. Selecione o operador a ser aplicado na lista suspensa.

   +++Lista de operadores disponíveis

   >[!NOTE]
   >
   >Os operadores disponíveis na lista suspensa dependem do tipo de dados do atributo selecionado.

   | Operador | Finalidade | Exemplo |
   |  ---  |  ---  |  ---  |
   | Igual a | Retorna um resultado idêntico aos dados inseridos na segunda coluna de valor. | Last name (@lastName) equal to &#39;Jones&#39;, retornará apenas destinatários cujo sobrenome seja Jones. |
   | Diferente de | Retorna todos os valores não idênticos ao valor inserido. | Idioma (@language) a ser igual a &#39;English&#39; |
   | Maior que | Retorna um valor maior que o valor digitado. | Idade (@age) maior que 50</strong>, retornará todos os valores maiores que &#39;50&#39;, ou seja, &#39;51&#39;, &#39;52&#39; etc. |
   | Menor que | Retorna um valor menor que o valor digitado. | Data de criação (@created) antes de &#39;DaysAgo(100)&#39;</strong>, retornará todos os destinatários criados menos de 100 dias atrás. |
   | Maior que ou igual a | Retorna todos os valores iguais ou maiores que o valor digitado. | Age (@age) greater than or equal to &#39;30&#39;</strong>, retornará todos os destinatários com 30 anos ou mais. |
   | Menor que ou igual a | Retorna todos os valores iguais ou inferiores ao valor inserido. | Age (@age) less than or equal to &#39;60&#39;</strong>, retornará todos os destinatários com 60 anos ou menos. |
   | Incluído em | Retorna resultados incluídos nos valores indicados. Esses valores devem ser separados por vírgula. | Birth date (@birthDate) is included in &#39;12/10/1979,12/10/1984&#39; retornará os destinatários nascidos entre essas datas. |
   | Não está em | Funciona como o operador Is included in. Aqui, queremos excluir destinatários com base nos valores inseridos. | A data de nascimento (@birthDate) não está incluída em &#39;12/10/1979,12/10/1984&#39;. Ao contrário do exemplo anterior, os destinatários nascidos nessas datas não serão retornados. |
   | Está vazio | Nesse caso, o resultado que estamos procurando corresponde a um valor vazio na segunda coluna de valor. | Mobile (@mobilePhone) is empty retorna todos os destinatários que não têm número de celular. |
   | Não está vazio | Funciona de forma inversa ao operador Is empty. Não é necessário inserir dados na segunda coluna de valor. | O email (@email) não está vazio. |
   | Inicia com | Retorna os resultados iniciando com o valor inserido. | Account # (@account) starts with &#39;32010&#39;. |
   | Não começa com | Retorna os resultados que não começam com o valor inserido | Account # (@account) não começa com &#39;20&#39; |
   | Contém | Retorna os resultados contendo pelo menos o valor inserido. | Email domain (@domain) contains &#39;mail&#39; (O domínio de email () contém &#39;mail&#39;)</strong>, retornará todos os nomes de domínio que contêm &#39;mail&#39;. Assim, o domínio &quot;gmail.com&quot; também será retornado. |
   | Não contém | Retorna resultados não contendo o valor digitado. | O domínio de email (@domain) não contém &#39;vo&#39;</strong>. Nesse caso, nomes de domínio que contêm &#39;vo&#39; não serão retornados. O nome de domínio &#39;voila.fr&#39; não aparecerá nos resultados. |
   | Como | Like é muito semelhante ao operador Contains. Permite inserir um caractere curinga % no valor. | Sobrenome (@lastName) como &#39;Jon%s&#39;. Aqui, o caractere curinga é usado como &quot;joker&quot; para localizar o nome &quot;Jones&quot;, o operador esqueceu a letra ausente entre o &#39;n&#39; e o &#39;s&#39;. |
   | Not like | Like é muito semelhante ao operador Contains. Permite inserir um caractere curinga % no valor. | Sobrenome (@lastName) diferente de &#39;Smi%h&#39;. Aqui, os destinatários que têm &#39;Smi%h&#39; como sobrenome não serão retornados. |

+++

1. No campo Value, selecione o valor esperado.

   Você também pode usar o editor de expressão da Web do Campaign para definir manualmente uma expressão usando campos do banco de dados e funções auxiliares. Para fazer isso, clique no botão Edit expression.

   *Exemplo: a consulta retorna todos os perfis com 21 anos ou mais*

   ![](assets/query-custom-condition.png)

<!--
querying linked tables
collect additional information on the targeted population, e.g. contract numbers, subscriptions to newsletters or origin.
Select the type of data you want to add. This can be data belonging to the filtering dimension or data stored in linked tables. Select the table which contains the information you want to collect and click Next.

aggregates: Define a calculation mode for the field to be added, such as an aggregate for example.-->

### Selecionar um público-alvo

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Selecionar público-alvo"
>abstract="Selecionar público-alvo"

Para filtrar sua query usando um público existente, siga estas etapas:

1. Clique no botão + no nó desejado e selecione **[!UICONTROL Selecionar público]**.

1. O painel Selecionar propriedades do público-alvo é aberto no lado direito. Selecione o público-alvo que deseja aproveitar para filtrar seu query.

   *Exemplo: consulta que retorna todos os perfis que pertencem ao público-alvo do &quot;Festival Goers&quot;*

   ![](assets/query-audience.png)

### Usar um filtro predefinido

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro predefinido"
>abstract="Filtro predefinido"

Para filtrar sua query usando um filtro predefinido, siga estas etapas:

1. Clique no botão + no nó desejado e selecione **[!UICONTROL Filtro predefinido]**.

1. O painel Selecionar propriedades do público-alvo é aberto no lado direito. Selecione um filtro predefinido na lista de filtros personalizados ou nos favoritos.

   *Exemplo: a consulta retorna todos os perfis correspondentes ao filtro predefinido &quot;Clientes inativos&quot;.*

   ![](assets/query-predefined-filter.png)

## Combinar componentes de filtragem com operadores

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Grupo"
>abstract="Grupo"

Ao adicionar um componente de filtragem ao seu query, uma nova transição é criada automaticamente na tela de query e o novo componente de filtragem é vinculado ao primeiro por um operador AND. Isso significa que os resultados de ambos os componentes de filtragem são combinados nos resultados da consulta.

Neste exemplo, um novo componente de filtragem do tipo público-alvo é adicionado à tela. Ele é automaticamente adicionado em uma nova transição e vinculado à condição de tipo de filtro predefinida com um operador AND. Nesse caso, os resultados da consulta incluem recipients direcionados pelo filtro predefinido &quot;Madridians&quot; E pertencentes ao público &quot;Discount hunters&quot;.

![](assets/query-operator.png)

Para alterar o operador usado para vincular condições de filtragem, clique nele e selecione o operador desejado em Você pode alterar o operador clicando nele e selecionando o operador desejado no painel Grupo que é aberto no lado direito.

![](assets/query-operator-change.png)

Os operadores disponíveis são:

* E (Interseção): combina resultados de todos os componentes de filtragem nas transições de saída.
* OU (União): inclui resultados de pelo menos um dos componentes do filtro nas transições de saída.
* EXCEPT (Exclusão): exclui os resultados de todos os componentes de filtragem na transição de saída.

## Verificar e validar sua consulta

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propriedades da regra"
>abstract="Propriedades da regra"

Depois de criar o query na tela, você pode verificá-lo usando o painel de propriedades Regra localizado no lado direito. As operações disponíveis são as seguintes:

* **Exibir resultados:** exibe os dados resultantes do query.
* **Visualização de código**: exibe uma versão baseada em código da consulta no SQL.
* **Calcular**: atualiza e exibe o número de registros direcionados por sua consulta.
* **Selecionar ou salvar filtro**: escolha um filtro predefinido existente para usar na tela ou salve sua consulta como um filtro predefinido para futura reutilização. [Saiba como trabalhar com filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Selecione um filtro predefinido no painel de propriedades Regra para substituir a consulta criada na tela pelo filtro selecionado.
