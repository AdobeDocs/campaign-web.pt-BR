---
audience: end-user
title: Criar a primeira consulta usando o modelador de consultas
description: Saiba como criar sua primeira consulta no Adobe Campaign Web query modeler.
source-git-commit: e78122b0788c04c39eac27231272cb96ad019bdc
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 19%

---

# Criar a primeira consulta {#build-query}

Para começar a criar uma consulta, acesse o modelador de consultas do local de sua escolha, dependendo da ação que deseja executar. O modelador de Consulta é aberto com uma tela em branco. Clique em **+** botão para configurar o primeiro nó do query.

Você pode adicionar dois tipos de elementos:

* **Filtrar componentes** (Condição personalizada, Selecionar público, Filtro predefinido) permitem criar suas próprias regras, selecionar um público ou um filtro predefinido para refinar sua consulta. [Saiba como trabalhar com componentes de filtragem](#filtering)

  Exemplo:

  *Recipients que assinaram o boletim informativo &quot;Esportes&quot;*. *Recipients que vivem em Nova York*, *Recipients que vivem em São Francisco*

* **Operadores de grupo** (AND, OR, EXCEPT) permitem agrupar componentes de filtragem no diagrama para atender às suas necessidades. [Saiba como trabalhar com operadores](#filtering)

  Exemplo:

  *Recipients que assinaram o boletim informativo &quot;Esportes&quot;**E**que vivem em Nova York **OU**São Francisco*.

![](assets/query-add-component.png)

## Adicionar componentes de filtragem {#filtering}

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

1. Clique em **+** no nó desejado e selecione **[!UICONTROL Condição personalizada]**. O painel de propriedades de condição personalizada é aberto no lado direito.

1. No **Atributo** selecione o atributo do banco de dados que deseja utilizar para criar sua condição. A lista de atributos inclui todos os atributos do banco de dados do Campaign, incluindo atributos vinculados à tabela.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >O botão Edit expression permite aproveitar o editor de expressão da Web do Campaign para definir manualmente uma expressão usando campos do banco de dados e funções auxiliares.

1. Selecione o operador a ser aplicado na lista suspensa. Vários operadores estão disponíveis para uso. Observe que os operadores disponíveis na lista suspensa dependem do tipo de dados do atributo.

   +++Lista de operadores disponíveis

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

1. No **Valor** defina o valor esperado. Você também pode usar o editor de expressão da Web do Campaign para definir manualmente uma expressão usando campos do banco de dados e funções auxiliares. Para fazer isso, clique no link **Editar expressão** botão.

   *Exemplo de consulta que retorna todos os perfis com 21 anos ou mais:*

   ![](assets/query-custom-condition.png)

**Condições personalizadas em tabelas distantes (links 1-1 e 1-N)**

As condições personalizadas permitem consultar tabelas distantes vinculadas à tabela Recipients.

Para um **Link 1-1** com outro recurso de banco de dados, selecione o valor diretamente na tabela direcionada.

+++Exemplo de consulta

Aqui, o query é direcionado a recipients cujo país ou região está incluído em determinados valores (reino unido e eua)

![](assets/custom-condition-1-1.png)

+++

Para um **Link 1-N** com outro recurso de banco de dados, é possível definir subcondições nos campos desse segundo recurso.

Por exemplo, você pode selecionar o operador Exists nas compras de perfil para direcionar todos os perfis para os quais existem compras. Depois de concluído, adicione uma condição personalizada na transição de saída e crie um filtro para atender às suas necessidades.

+++Exemplo de consulta

Aqui, o query é direcionado a recipients que fizeram compras relacionadas ao produto BrewMaster, para um valor total de pelo menos 100$.

![](assets/custom-condition-1-N.png)

+++

### Selecionar um público-alvo

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Selecionar público-alvo"
>abstract="Selecionar público-alvo"

Para filtrar sua query usando um público existente, siga estas etapas:

1. Clique em **+** no nó desejado e escolha **[!UICONTROL Selecionar público]**.

1. A variável **Selecionar público** painel de propriedades é aberto no lado direito. Escolha o público-alvo que deseja usar para filtrar o query.

   *Exemplo de consulta retornando todos os perfis que pertencem ao público-alvo &quot;Visitantes do Festival&quot;:*

   ![](assets/query-audience.png)

### Usar um filtro predefinido

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Filtro predefinido"
>abstract="Filtro predefinido"

Para filtrar sua query usando um filtro predefinido, siga estas etapas:

1. Clique em **+** no nó desejado e selecione **[!UICONTROL Filtro predefinido]**.

1. A variável **Filtro predefinido** painel de propriedades é aberto no lado direito. Selecione um filtro predefinido na lista de filtros personalizados ou nos favoritos.

   *Exemplo de consulta que retorna todos os perfis correspondentes ao filtro predefinido &quot;Clientes inativos&quot;:*

   ![](assets/query-predefined-filter.png)

## Combinar componentes de filtragem com operadores {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Grupo"
>abstract="Grupo"

Cada vez que um novo componente de filtragem é adicionado ao query, ele é automaticamente vinculado ao outro componente por um operador AND. Isso significa que os resultados de ambos os componentes de filtragem são combinados nos resultados da consulta.

Neste exemplo, adicionamos novos componentes de filtragem do tipo público-alvo na segunda transição. O componente é vinculado à condição de tipo de filtro predefinida com um operador AND, o que significa que os resultados da consulta incluem recipients direcionados pelo filtro predefinido &quot;Madridians&quot; E pertencentes ao público-alvo &quot;Discount hunters&quot;.

![](assets/query-operator.png)

Para alterar o operador usado para vincular as condições do filtro, clique nele e selecione o operador desejado no painel Grupo que é aberto no lado direito.

Os operadores disponíveis são:

* **E (Interseção)**: combina resultados que correspondem a todos os componentes de filtragem nas transições de saída.
* **OU (União)**: inclui resultados que correspondem a pelo menos um dos componentes de filtragem nas transições de saída.
* **EXCETO (Exclusão)**: exclui resultados que correspondem a todos os componentes de filtragem na transição de saída.

![](assets/query-operator-change.png)

## Verificar e validar sua consulta

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Propriedades da regra"
>abstract="Propriedades da regra"

Depois de criar o query na tela, você pode verificá-lo usando o **Propriedades da regra** painel localizado no lado direito. As operações disponíveis são:

* **Exibir resultados:** Exibe os dados resultantes da sua consulta.
* **Visualização de código**: exibe uma versão baseada em código da consulta no SQL.
* **Calcular**: atualiza e exibe o número de registros direcionados por sua consulta.
* **Selecionar ou salvar filtro**: escolha um filtro predefinido existente para usar na tela ou salve sua consulta como um filtro predefinido para futura reutilização. [Saiba como trabalhar com filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Selecione um filtro predefinido no painel de propriedades Regra para substituir a consulta criada na tela pelo filtro selecionado.
