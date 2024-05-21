---
audience: end-user
title: Usar a atividade de fluxo de trabalho Atualizar dados
description: Saiba como usar a atividade de workflow Atualizar dados
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 32%

---

# Atualizar dados {#update-data}

A variável **Atualizar dados** a atividade é um **Gerenciamento de dados** atividade. Ele permite executar uma atualização em massa nos campos no banco de dados. Várias opções permitem personalizar a atualização de dados.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## Configurar a atividade Update data{#update-data-configuration}

Para configurar o **Atualizar dados** atividade, comece adicionando a atividade ao workflow e defina um rótulo.

![](../assets/workflow-update-data.png)

### Tipo de operação

O campo **Operation type** permite escolher o processo que deve ser executado nos dados no banco de dados:

* **Inserir ou atualizar**: inserir dados ou atualizá-los se os registros já existirem no banco de dados.
* **Inserir**: inserir somente dados. Os registros que já existem não são atualizados. Se os critérios de reconciliação forem definidos, somente os registros não reconciliados serão adicionados.
* **Atualizar**: atualizar os dados dos registros que já existem somente no banco de dados.
* **Delete**: excluir dados.

O campo **Batch size** permite selecionar o número de elementos de transição de entrada a serem atualizados. Por exemplo, se o número declarado for 500, os primeiros 500 registros serão atualizados.

### Identificação de registro

Esta seção permite especificar como identificar os registros no banco de dados:

* Se as entradas de dados se relacionam a uma dimensão de direcionamento existente, selecione a variável **Uso da targeting dimension** e selecione-a na caixa **Dimensão de direcionamento a ser atualizada** campo.
* Você também pode selecionar a variável **Uso de links personalizados** e especificar um ou mais links que permitirão a identificação dos dados no banco de dados
* Se o tipo de operação selecionado exigir uma atualização, você deverá usar o **Uso de regras de reconciliação** opção.

### Campos a serem atualizados

No **Campos a serem atualizados** adicione os campos nos quais a atualização será aplicada e, se necessário, adicione condições para que essa atualização seja realizada. Para fazer isso, use o **Levar em consideração se** campo. As condições são aplicadas uma após a outra em ordem de lista. Use as setas à direita para alterar a ordem das atualizações. É possível usar o mesmo campo de destino várias vezes.

É possível vincular campos automaticamente usando a variável **Mapeamento automático** botão. A vinculação automática detecta campos com o mesmo nome.

Durante um **Inserir ou atualizar** tipo de operação, você pode selecionar individualmente a operação a ser aplicada para cada campo. Para fazer isso, selecione o valor desejado na variável **Tipo de operação** campo.

### Opções avançadas

A variável **Opções avançadas** permite especificar as opções adicionais para lidar com a atualização de dados, assim como gerenciar as duplicatas.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

As duas últimas opções permitem executar ações específicas:

* **Gerar uma transição de saída**: cria uma transição de saída que será ativada no final da execução. A atualização normalmente sinaliza o final de um workflow para construção do target e, portanto, a opção não é ativada por padrão.

* **Gerar uma transição de saída para as rejeições**: cria uma transição de saída contendo registros que não foram processados corretamente após a atualização (por exemplo, se houver uma duplicata). A atualização geralmente marca o final de um fluxo de trabalho de direcionamento e, portanto, a opção não é ativada por padrão.
