---
audience: end-user
title: Usar a atividade de workflow de desduplicação
description: Saiba como usar a atividade de workflow de desduplicação
badge: label="Beta"
source-git-commit: bf98ca98510f51fb7496a380f6547b0d3e954006
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 23%

---


# Desduplicação {#deduplication}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Fork activity"
>abstract="The Deduplication activity allows you to..."
-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Gerar um complemento"
>abstract="Você pode gerar uma transição de saída adicional com a população restante, que foi excluída como uma duplicata. Para fazer isso, ative a opção **Gerar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configurações de desduplicação"
>abstract="Para excluir duplicatas nos dados recebidos, defina o método de desduplicação nos campos abaixo. Por padrão, somente um registro é mantido. Você também deve selecionar o modo de desduplicação com base em uma expressão ou um atributo. Por padrão, o registro a ser mantido fora das duplicatas é selecionado aleatoriamente."

A variável **Desduplicação** a atividade é um **Direcionamento** atividade. Essa atividade permite excluir duplicados no(s) resultado(s) das atividades de entrada. A variável **Desduplicação** A atividade é geralmente usada após atividades de direcionamento e antes de atividades que permitem o uso de dados direcionados.

## Configuração

Siga estas etapas para configurar o **Desduplicação** atividade:

1. Adicionar um **Desduplicação** atividade ao seu fluxo de trabalho.

   ![](../assets/workflow-deduplication.png)

1. No **Campos para identificar duplicatas** clique na guia **Adicionar atributo** botão para especificar os campos para os quais os valores idênticos permitem a identificação das duplicatas: endereço de email, nome, sobrenome etc. A ordem dos campos permite especificar os que serão processados primeiro.

1. Selecione o número de **Duplicatas a serem mantidas**. O valor padrão para esse campo é 1. O valor 0 permite manter todas as duplicatas.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. Selecione o **Método de desduplicação** para usar:

   * **Seleção aleatória**: seleciona aleatoriamente o registro a ser mantido fora das duplicatas.
   * **Usar uma expressão**: permite manter os registros nos quais o valor da expressão inserida é o menor ou o maior. ++ Expressão ++ Classificação
   * **Following a list of values**: permite definir uma prioridade de valor para um ou mais campos. Para definir os valores, clique em **Atributo** para selecionar um campo ou criar uma expressão, adicione o(s) valor(es) à tabela apropriada. Para definir um novo campo, clique no botão Add localizado acima da lista de valores. ++ Classificar

1. Marque a opção **Generate complement** se desejar explorar a população restante. O complemento consiste de todas as duplicatas. Uma transição adicional será adicionada à atividade.

## Exemplo

