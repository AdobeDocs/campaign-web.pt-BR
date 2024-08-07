---
audience: end-user
title: Usar a atividade do workflow de reconciliação
description: Saiba como usar a atividade de workflow de reconciliação
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 935fba929c26d6d7b3057ee7c24148215a04e45e
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 47%

---

# Reconciliação {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Atividade de reconciliação"
>abstract="A atividade de **Reconciliação** é uma atividade de **Direcionamento** que permite definir o vínculo entre os dados no banco de dados do Adobe Campaign e os dados em uma tabela de trabalho. Por exemplo, a atividade de **Reconciliação** pode ser inserida após uma atividade **Carregar arquivo** para importar dados não padrão para o banco de dados. Nesse caso, a atividade de **Reconciliação** permite definir o vínculo entre os dados no banco de dados do Adobe Campaign e os dados na tabela externa."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Campo de seleção de reconciliação"
>abstract="Campo de seleção de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Condição de criação de reconciliação"
>abstract="Condição de criação de reconciliação"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Complemento de geração de reconciliação"
>abstract="Complemento de geração de reconciliação"

A atividade **Reconciliation** é uma atividade **Targeting** que permite definir o vínculo entre os dados no banco de dados do Adobe Campaign e os dados em uma tabela de trabalho, por exemplo, dados carregados de um arquivo externo.

Por exemplo, a atividade de **Reconciliação** pode ser inserida após uma atividade **Carregar arquivo** para importar dados não padrão para o banco de dados. Nesse caso, a atividade **Reconciliation** permite definir o vínculo entre os dados no banco de dados do Adobe Campaign e os dados na tabela de trabalho.

## Práticas recomendadas {#reconciliation-best-practices}

Embora a atividade **Enrichment** permita a definição de dados adicionais a serem processados no fluxo de trabalho (você pode usar uma atividade **Enrichment** para combinar dados provenientes de vários conjuntos ou para criar links para um recurso temporário), a atividade **Reconciliation** permite vincular dados não identificados aos recursos existentes.

>[!NOTE]
>A operação de reconciliação implica que os dados das dimensões vinculadas já estão no banco de dados.  Por exemplo, se você importar um arquivo de compras que mostre qual produto foi comprado, em que momento, por qual cliente, etc., o produto e o cliente já deverão existir no banco de dados.

## Configurar a atividade de reconciliação {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimensão de direcionamento"
>abstract="Selecione a nova dimensão de direcionamento. Uma dimensão permite definir a população direcionada: destinatários, assinantes de aplicativos, operadores, assinantes etc. Por padrão, a dimensão de direcionamento atual é selecionada."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Regras de reconciliação"
>abstract="Selecione as regras de reconciliação a serem usadas para a desduplicação. Para usar atributos, selecione a opção **Atributos simples** e escolha os campos origem e destino. Para criar sua própria condição de reconciliação usando o modelador de consultas, selecione a opção **Condições de reconciliação avançadas**."
>additional-url="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/query-database/query-modeler-overview" text="Trabalhar com o modelador de consultas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Selecione a dimensão de direcionamento"
>abstract="Selecione a dimensão de direcionamento com a qual seus dados de entrada devem se reconciliar."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html?lang=pt-BR#targeting-dimensions" text="Dimensões de direcionamento"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Manter dados não reconciliados"
>abstract="Por padrão, os dados não reconciliados são mantidos na transição de saída e disponibilizados na tabela de trabalho para uso futuro. Para remover dados não reconciliados, desative a opção **Manter dados não reconciliados**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Atributo de reconciliação"
>abstract="Selecione o atributo a ser usado para reconciliar dados e clique em Confirmar."

Siga estas etapas para configurar a atividade **Reconciliação**:

1. Adicione uma atividade de **Reconciliação** ao seu fluxo de trabalho. Essa atividade deve ser adicionada após uma transição que contém uma população cujo targeting dimension não é diretamente proveniente do Adobe Campaign.

1. Selecione a nova dimensão de direcionamento. Uma dimensão permite definir a população direcionada: destinatários, assinantes de aplicativos, operadores, assinantes etc. [Saiba mais sobre dimensões de direcionamento](../../audience/about-recipients.md#targeting-dimensions).

1. Selecione os campos a serem usados para a reconciliação. É possível usar um ou mais critérios de reconciliação.

   1. Para usar atributos para reconciliar dados, selecione a opção **Atributos simples**. O campo **Source** lista os campos disponíveis na transição de entrada, que devem ser reconciliados. O campo **Destination** corresponde aos campos da targeting dimension selecionada. Os dados são reconciliados quando a origem e o destino são iguais. Por exemplo, selecione os campos **Email** para desduplicar perfis com base em seus endereços de email.

      Para adicionar outro critério de reconciliação, clique no botão **Adicionar regra**. Se várias condições de associação forem especificadas, TODAS elas deverão ser verificadas para que os dados possam ser vinculados.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. Para usar outros atributos para reconciliar dados, selecione a opção **Condições avançadas de reconciliação**. Em seguida, você pode criar sua própria condição de reconciliação usando o modelador de consultas. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md).

1. Você pode filtrar dados para reconciliar usando o botão **Criar filtro**. Isso permite criar uma condição personalizada usando o modelador de consultas. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md)

Por padrão, os dados não reconciliados são mantidos na transição de saída e disponibilizados na tabela de trabalho para uso futuro. Para remover dados não reconciliados, desative a opção **Manter dados não reconciliados**.

## Exemplo {#reconciliation-example}

O exemplo a seguir demonstra um fluxo de trabalho que cria um público-alvo de perfis diretamente de um arquivo importado que contém novos clientes. Ele é composto pelas seguintes atividades:

O fluxo de trabalho de reconciliação foi criado deste modo:

![](../assets/workflow-reconciliation-sample-1.0.png)


Ele é criado com as seguintes atividades:

* Uma atividade [Load file](load-file.md) faz upload de um arquivo contendo dados de perfis que foram extraídos de uma ferramenta externa.

  Por exemplo:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* Uma atividade de **Reconciliação** que identifica os dados recebidos como perfis usando os campos **email** e **Data de nascimento** como critérios de reconciliação.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* Uma atividade [Save audience](save-audience.md) para criar um novo público-alvo com base nessas atualizações. Você também pode substituir a atividade **Salvar público-alvo** por uma atividade **Fim** se nenhum público-alvo específico precisar ser criado ou atualizado. Os perfis de recipient são atualizados em qualquer caso quando você executa o workflow.


## Compatibilidade {#reconciliation-compat}

A atividade **Reconciliation** não existe no console do cliente. Todas as atividades de **Enriquecimentos** criadas no console do cliente com as opções de reconciliação habilitadas são exibidas como atividades de **Reconciliação** na interface do usuário da Web do Campaign.
