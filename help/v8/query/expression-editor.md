---
audience: end-user
title: Criar a primeira consulta usando o modelador de consultas
description: Saiba como criar sua primeira consulta no Adobe Campaign Web query modeler.
source-git-commit: e620df0ff9af0d32fc353a904e3dde37501495d0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 79%

---

# Editar expressões {#expression}

A edição de uma expressão envolve a inserção manual de condições para formar uma regra. Esse modo permite usar funções avançadas. Essas funções permitem manipular os valores usados para realizar consultas específicas, como manipular datas, strings, campos numéricos, classificação etc.

Essas operações estão disponíveis no botão Editar expressão do modelador de consultas, disponível para os campos Atributo e Valor ao configurar uma condição personalizada.

![](assets/edit-expression.png)

O editor de expressão fornece:

* Um campo de entrada no qual a expressão é definida.
* A lista dos campos disponíveis que podem ser usados na expressão e correspondem à dimensão de dimensionamento da query.
* A lista de funções disponíveis, classificadas por categoria.

Edite a expressão inserindo uma expressão diretamente no campo de entrada ou usando as listas de campos e funções disponíveis. Para fazer isso, coloque o cursor na inexpressão onde deseja adicionar o elemento e clique duas vezes no campo ou expressão desejada.

É possível usar variáveis de eventos de workflows para criar uma expressão. Para obter mais informações, consulte xxxx.

## Sintaxe da expressão {#expression-syntax}

### Sintaxe padrão {#standard-syntax}

As expressões padrão são formadas por uma ou várias condições que respeitam os seguintes elementos de sintaxe:

* Cada condição assume a forma de **&lt;value1> &lt;comparison operator> &lt;value2>** em que:

   * **&lt;value1>** é um campo ou uma função. Por exemplo, **@created** para a data em que um perfil foi criado ou **Year(@created)** para o ano em que um perfil foi criado.
   * **&lt;comparison operator=&quot;&quot;>** é um dos operadores listados na seção Operadores de comparação. Esse operador define o método de comparação entre **&lt;value1>** e **&lt;value2>**.
   * **&lt;value2>** é um campo, uma função ou um valor inserido manualmente.

  >[!NOTE]
  >
  >Os dados dos tipos **&lt;value1>** e **&lt;value2>** devem ser idênticos. Por exemplo, se **&lt;value1>** for uma data, **&lt;value2>** também deverá ser uma data.

* Se quiser usar várias condições, elas poderão ser combinadas usando operadores lógicos.

   * **[!UICONTROL E]**: duas condições são cruzadas.
   * **[!UICONTROL OU]**: duas condições são combinadas.

Por exemplo:

```
Year(@created) = Year(GetDate()) AND Month(@created) = Month(GetDate())
```

Neste exemplo, os perfis cuja data de criação é no mês e ano atuais são direcionados.

### Sintaxe JavaScript {#javascript-syntax}

Ao definir as condições de visibilidade de um bloco de tipo de texto do editor de conteúdo HTML, você deve usar uma expressão com a sintaxe de tipo JavaScript.

As expressões JavaScript são constituídas por uma ou várias condições e usam os seguintes elementos de sintaxe:

* Cada condição assume a forma de **&lt;context> &lt;comparison operator> &lt;value2>** em que:

   * **&lt;context>** é um campo ou uma função que permite especificar o contexto. Por exemplo, **context.perfil.@email** para um endereço de email do perfil ou **context.perfil.firstName.length()** para o número de caracteres do nome do perfil.
   * **&lt;comparison operator=&quot;&quot;>** é um dos operadores listados na seção Operadores de comparação. Esse operador define o método de comparação entre **&lt;context>** e **&lt;value2>**.
   * **&lt;value2>** é um campo, uma função ou um valor inserido manualmente.

  >[!NOTE]
  >
  Os dados dos tipos **&lt;context>** e **&lt;value2>** devem ser idênticos. Por exemplo, se **&lt;context>** for uma data, **&lt;value2>** também deverá ser uma data.

* Se quiser usar várias condições, elas poderão ser combinadas usando operadores lógicos.

   * **[!UICONTROL &amp;&amp;]**: duas condições são cruzadas.
   * **[!UICONTROL ||]**: duas condições são combinadas.

Por exemplo:

```
context.profile.age > 21 && context.profile.firstName.length() > 0
```

Neste exemplo, perfis com mais de 21 anos e cujo nome foi fornecido (simbolizado pelo fato de o campo **firstName** contém pelo menos um caractere).

## Operadores de comparação {#comparison-operators}

Para algumas regras, o Editor de consultas permite escolher um valor para definir sua condição.

As condições devem ser vinculadas a valores usando um dos operadores a seguir.

<table> 
 <thead> 
  <tr> 
   <th> Operador<br /> </th> 
   <th> Sintaxe padrão<br /> </th> 
   <th> Sintaxe JavaScript<br /> </th> 
   <th> Descrição<br /> </th> 
   <th> Exemplo<br /> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <span class="uicontrol">Equal to</span> <br /> </td> 
   <td> =<br /> </td> 
   <td> ==<br /> </td> 
   <td> O primeiro valor deve ser completamente idêntico ao segundo.<br /> </td> 
   <td> <strong>@lastName = Martin</strong> recupera perfis cujo sobrenome é 'Martin', com apenas esses caracteres idênticos.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Greater than</span> <br /> </td> 
   <td> &gt;<br /> </td> 
   <td> &gt;<br /> </td> 
   <td> O primeiro valor deve ser categoricamente maior que o segundo.<br /> </td> 
   <td> <strong>@age &gt; 50</strong> recupera perfis mais antigos que '50', então '51', '52' etc.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Less than</span> <br /> </td> 
   <td> &lt;<br /> </td> 
   <td> &lt;<br /> </td> 
   <td> O primeiro valor deve ser categoricamente menor que o segundo.<br /> </td> 
   <td> <strong>@created &lt; DaysAgo(100)</strong> recupera todos os perfis criados no banco de dados há menos de 100 dias.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Greater than or equal to</span> <br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> O primeiro valor deve ser maior que ou igual ao segundo valor.<br /> </td> 
   <td> <strong>@age &gt;= 30</strong> recupera perfis com 30 anos ou mais.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Less than or equal to</span> <br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> O primeiro valor deve ser menor que ou igual ao segundo.<br /> </td> 
   <td> <strong>@age &lt;= 60</strong> recupera perfis com 60 anos ou menos.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Different </span> <br /> </td> 
   <td> !=<br /> </td> 
   <td> !=<br /> </td> 
   <td> O primeiro valor deve ser diferente do segundo.<br /> </td> 
   <td> <strong>@language != English</strong> recupera perfis que não foram definidos como falantes do inglês.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Contains</span> <br /> </td> 
   <td> IN<br /> </td> 
   <td> N/A<br /> </td> 
   <td> O primeiro valor deve conter o segundo.<br /> </td> 
   <td> <strong>@domain IN mail</strong>. Aqui, todos os nomes de domínios com o valor 'mail' são retornados no resultado. Consequentemente, o nome de domínio 'gmail.com' fará parte dos resultados retornados.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Like</span> <br /> </td> 
   <td> LIKE<br /> </td> 
   <td> N/A<br /> </td> 
   <td> <span class="uicontrol">Like</span> é muito semelhante ao operador <span class="uicontrol">Contains</span>. Permite inserir um caractere curinga <span class="uicontrol">%</span> no valor que está sendo pesquisado.<br /> </td> 
   <td> <strong>@lastName LIKE Mart%n</strong>. Aqui, o caractere de substituição <strong>%</strong> serve como "joker" para encontrar o nome "Martin" no caso hipotético de a ortografia não estar correta.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Not like</span> <br /> </td> 
   <td> NOT<br /> </td> 
   <td> N/A<br /> </td> 
   <td> É semelhante a <span class="uicontrol">Like</span>. Permite que você não recupere o valor inserido. Aqui o valor inserido também deve conter o caractere curinga <span class="uicontrol">%</span>.<br /> </td> 
   <td> <strong>@lastName NOT Smi%h</strong>. Aqui, os destinatários correspondem ao nome 'Smi%h' (então Smith, etc.) não são retornados como resultado.<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Is empty</span> <br /> </td> 
   <td> IS NULL<br /> </td> 
   <td> N/A<br /> </td> 
   <td> O primeiro valor deve corresponder a um valor vazio.<br /> </td> 
   <td> <strong>@mobilePhone IS NULL</strong> recupera todos os perfis cujo número de telefone celular não foi fornecido.<br /> </td> 
  </tr> 
 </tbody> 
</table>