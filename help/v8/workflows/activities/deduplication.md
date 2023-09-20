---
audience: end-user
title: Usar a atividade de workflow de desduplicação
description: Saiba como usar a atividade de workflow de desduplicação
badge: label="Beta"
source-git-commit: 690e2a2d17f8201c8dbb070ba936c3db513b8329
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 29%

---


# Desduplicação {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Campos para identificar duplicatas"
>abstract="No **Campos para identificar duplicatas** clique na guia **Adicionar atributo** botão para especificar os campos para os quais os valores idênticos permitem a identificação das duplicatas, como: endereço de email, nome, sobrenome etc. A ordem dos campos permite especificar os que serão processados primeiro."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Atividade de desduplicação"
>abstract="A variável **Desduplicação** A atividade de permite excluir duplicados nos resultados das atividades de entrada. Ele é usado principalmente após atividades de direcionamento e antes de atividades que permitem o uso de dados direcionados."


>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Gerar um complemento"
>abstract="Você pode gerar uma transição de saída adicional com a população restante, que foi excluída como uma duplicata. Para fazer isso, ative a opção **Gerar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Configurações de desduplicação"
>abstract="Para excluir duplicatas nos dados recebidos, defina o método de desduplicação nos campos abaixo. Por padrão, somente um registro é mantido. Você também deve selecionar o modo de desduplicação com base em uma expressão ou um atributo. Por padrão, o registro a ser mantido fora das duplicatas é selecionado aleatoriamente."

A variável **Desduplicação** a atividade é um **Direcionamento** atividade. Essa atividade permite excluir duplicados no(s) resultado(s) das atividades de entrada, por exemplo, perfis duplicados na lista de recipients. A variável **Desduplicação** A atividade é geralmente usada após atividades de direcionamento e antes de atividades que permitem o uso de dados direcionados.

## Configurar a atividade de desduplicação{#deduplication-configuration}

Siga estas etapas para configurar o **Desduplicação** atividade:

![](../assets/workflow-deduplication.png)

1. Adicionar um **Desduplicação** atividade ao seu fluxo de trabalho.

1. No **Campos para identificar duplicatas** clique na guia **Adicionar atributo** botão para especificar os campos para os quais os valores idênticos permitem a identificação das duplicatas, como: endereço de email, nome, sobrenome etc. A ordem dos campos permite especificar os que serão processados primeiro.

1. Selecione o número de **Duplicatas a serem mantidas**. O valor padrão para esse campo é 1. O valor 0 permite manter todas as duplicatas.

   Por exemplo, se os registros A e B forem considerados duplicatas do registro Y, e um registro C for considerado uma duplicata do registro Z:

   * Se o valor do campo for 1: somente os registros Y e Z são mantidos.
   * Se o valor do campo for 0: todos os registros são mantidos.
   * Se o valor do campo for 2: os registros C e Z são mantidos. Os dois registros de A, B e Y são mantidos por acaso ou dependendo do método de desduplicação selecionado posteriormente.

1. Selecione o **Método de desduplicação** para usar:

   * **Seleção aleatória**: seleciona aleatoriamente o registro a ser mantido fora das duplicatas.
   * **Usar uma expressão**: permite manter os registros nos quais o valor da expressão inserida é o menor ou o maior.
   * **Following a list of values**: permite definir uma prioridade de valor para um ou mais campos. Para definir os valores, clique em **Atributo** para selecionar um campo ou criar uma expressão, adicione o(s) valor(es) à tabela apropriada. Para definir um novo campo, clique no botão Add localizado acima da lista de valores.

1. Marque a opção **Generate complement** se desejar explorar a população restante. O complemento consiste de todas as duplicatas. Uma transição adicional será adicionada à atividade.

## Exemplo{#deduplication-example}

No exemplo a seguir, use uma atividade de desduplicação para excluir duplicatas do target antes de enviar um delivery. Os recipients duplicados identificados são adicionados a um público dedicado que pode ser reutilizado se necessário. Escolha o **E-mail** para identificar as duplicatas. Mantenha 1 entrada e selecione a variável **Aleatório** método de desduplicação.

![](../assets/workflow-deduplication-example.png)
