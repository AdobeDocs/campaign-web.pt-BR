---
audience: end-user
title: Usar a atividade do workflow de reconciliação
description: Saiba como usar a atividade de workflow de reconciliação
badge: label="Disponibilidade limitada"
source-git-commit: 88daf84e617595a80c5cd3fd536969618f0fdcf5
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 20%

---

# Reconciliação {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Atividade de reconciliação"
>abstract="A variável **Reconciliação** a atividade é um **Direcionamento** Atividade que permite vincular dados não identificados aos dados existentes do Campaign. Por exemplo, a variável **Reconciliação** A atividade pode ser colocada após um **Carregar público** atividade para importar dados não padrão para o banco de dados. Neste caso, o **Reconciliação** A atividade permite definir o link entre os dados no banco de dados do Adobe Campaign e os dados na tabela externa."


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



A variável **Reconciliação** a atividade é um **Direcionamento** atividade que permite vincular dados não identificados aos recursos existentes. Por exemplo, a variável **Reconciliação** A atividade pode ser colocada após um **Carregar público** atividade para importar dados não padrão para o banco de dados. Neste caso, o **Reconciliação** A atividade permite definir o link entre os dados no banco de dados do Adobe Campaign e os dados na tabela de trabalho.


## Práticas recomendadas {#reconciliation-best-practices}

Embora a **Enriquecimento** atividade permite definir dados adicionais a serem processados no fluxo de trabalho (você pode usar uma **Enriquecimento** para combinar dados provenientes de vários conjuntos ou para criar links para um recurso temporário), a variável **Reconciliação** A atividade permite vincular dados não identificados aos recursos existentes.

>[!NOTE]
>A operação de reconciliação implica que os dados das dimensões vinculadas já estão no banco de dados.  Por exemplo, se você importar um arquivo de compras que mostre qual produto foi comprado, em que momento, por qual cliente, etc., o produto e o cliente já deverão existir no banco de dados.
>

## Configurar a atividade de reconciliação {#reconciliation-configuration}


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Dimensão de direcionamento"
>abstract="Selecione a nova dimensão do target. Uma dimensão permite definir a população direcionada: recipients, assinantes de aplicativos, operadores, assinantes, etc. Por padrão, o targeting dimension atual é selecionado."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Regras de reconciliação"
>abstract="Selecione os campos de reconciliação a serem usados para a desduplicação. É possível usar um ou mais critérios de reconciliação."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Selecione o targeting dimension"
>abstract="Selecione o targeting dimension para seus dados de entrada com o qual reconciliar."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/about-recipients.html?lang=en#targeting-dimensions" text="Dimensões de direcionamento"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Manter dados não reconciliados"
>abstract="Por padrão, os dados não reconciliados são mantidos na transição de saída e disponibilizados na tabela de trabalho para uso futuro. Para remover dados não reconciliados, desative o **Manter dados não reconciliados** opção."


>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Atributo de reconciliação"
>abstract="Selecione o atributo a ser usado para reconciliar dados e clique em Confirmar."

Siga estas etapas para configurar o **Reconciliação** atividade:

1. Arraste e solte uma **Reconciliação** atividade no seu workflow. Essa atividade deve ser adicionada após uma transição que contém uma população cujo targeting dimension não é diretamente proveniente do Adobe Campaign.

1. Selecione a nova dimensão do target. Uma dimensão permite definir a população direcionada: recipients, assinantes de aplicativos, operadores, assinantes, etc. Saiba mais sobre targeting dimensions em [esta página](../../audience/about-recipients.md#targeting-dimensions).

1. Selecione os campos de reconciliação a serem usados para a desduplicação. É possível usar um ou mais critérios de reconciliação.

   1. Para usar atributos para reconciliar dados, selecione o **Atributos simples** opção. A variável **Origem** field lista os campos disponíveis na transição de entrada, que devem ser reconciliados. A variável **Destino** field corresponde aos campos da targeting dimension selecionada. Os dados são reconciliados quando a origem e o destino são iguais. Por exemplo, selecione a variável **E-mail** para desduplicar perfis com base em seus endereços de email.

      Para adicionar outro critério de reconciliação, clique no link **Adicionar regra** botão. Se várias condições de associação forem especificadas, TODAS elas deverão ser verificadas para que os dados possam ser vinculados.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. Para usar outros atributos para reconciliar dados, selecione o **Condições de reconciliação avançadas** opção. Em seguida, você pode criar sua própria condição de reconciliação usando o modelador de consultas. Saiba como usar o modelador de consultas no [nesta seção](../../query/query-modeler-overview.md).

1. É possível filtrar dados para reconciliar usando o **Criar filtro** botão. Isso permite criar uma condição personalizada usando o [modelador de consultas](../../query/query-modeler-overview.md).

Por padrão, os dados não reconciliados são mantidos na transição de saída e disponibilizados na tabela de trabalho para uso futuro. Para remover dados não reconciliados, desative o **Manter dados não reconciliados** opção.

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

* A **Reconciliação** atividade que identifica os dados recebidos como perfis, usando o **email** e **Data de nascimento** campos como critérios de reconciliação.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* A [Salvar público-alvo](save-audience.md) atividade para criar um novo público-alvo com base nessas atualizações. Também é possível substituir a variável **Salvar público-alvo** atividade por um **Fim** atividade se nenhum público específico precisar ser criado ou atualizado. Os perfis de recipient são atualizados em qualquer caso quando você executa o workflow.


## Compatibilidade {#reconciliation-compat}

A variável **Reconciliação** A atividade não existe no console do cliente. Todos **Enriquecimentos** atividades criadas no console do cliente com as opções de reconciliação ativadas são exibidas como **Reconciliação** atividades na interface do Campaign Web.