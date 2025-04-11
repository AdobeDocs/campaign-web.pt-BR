---
audience: end-user
title: Usar a atividade de fluxo de trabalho Atualizar dados
description: Saiba como usar a atividade de workflow Atualizar dados
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 22%

---

# Atualizar dados {#update-data}

A atividade **Atualizar dados** é uma atividade de **Gerenciamento de Dados**. Ela permite executar uma atualização em massa nos campos no banco de dados. Várias opções permitem personalizar a atualização de dados.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update it if it has already been added. You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely.

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or directly use reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section lets you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.
-->

## Configurar a atividade Update data {#update-data-configuration}

Para configurar a atividade **Atualizar dados**, adicione a atividade ao seu fluxo de trabalho e defina um rótulo.

![Atividade de Atualização de Dados do Fluxo de Trabalho](../assets/workflow-update-data.png)

### Tipo de operação

O campo **Operation type** permite escolher o processo que deve ser executado nos dados no banco de dados:

* **Inserir ou atualizar**: inserir dados ou atualizá-los se os registros já existirem no banco de dados.
* **Inserir**: inserir somente dados. Os registros que já existem não são atualizados. Se os critérios de reconciliação forem definidos, somente os registros não reconciliados serão adicionados.
* **Atualização**: atualiza os dados dos registros que já existem somente no banco de dados.
* **Excluir**: excluir dados.

O campo **Batch size** permite selecionar o número de elementos de transição de entrada a serem atualizados. Por exemplo, se você especificar 500, os primeiros 500 registros processados serão atualizados.

### Identificação de registro

Esta seção permite especificar como identificar os registros no banco de dados:

* Se as entradas de dados se relacionam a uma dimensão de direcionamento existente, selecione a opção **Using the targeting dimension** e a escolha no campo **Targeting dimension to update**.
* Você também pode selecionar **Usando links personalizados** e especificar um ou mais links que habilitarão a identificação dos dados no banco de dados.
* Se o tipo de operação selecionado exigir uma atualização, use a opção **Usando regras de reconciliação**.

### Campos a serem atualizados

Na seção **Campos a serem atualizados**, adicione os campos nos quais a atualização será aplicada. Se necessário, adicione condições para que essa atualização seja realizada. Use o campo **Levar em consideração se** para definir condições. As condições são aplicadas sequencialmente em ordem de lista. Use as setas à direita para alterar a ordem das atualizações. É possível usar o mesmo campo de destino várias vezes.

Vincular campos automaticamente usando o botão **Mapeamento automático**. A vinculação automática detecta campos com o mesmo nome.

Durante um tipo de operação **Inserir ou atualizar**, selecione individualmente a operação a ser aplicada para cada campo. Use o campo **Tipo de operação** para especificar o valor desejado.

### Opções avançadas

A seção **Opções avançadas** permite especificar opções adicionais para lidar com a atualização de dados e o gerenciamento de duplicatas.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

As duas últimas opções permitem executar ações específicas:

* **Gerar uma transição de saída**: cria uma transição de saída que será ativada no final da execução. A atualização normalmente sinaliza o final de um workflow para construção do target e, portanto, a opção não é ativada por padrão.

* **Gerar uma transição de saída para as rejeições**: cria uma transição de saída contendo registros que não foram processados corretamente após a atualização (por exemplo, se houver uma duplicata). A atualização geralmente marca o final de um workflow para construção do target e a opção não é ativada por padrão.