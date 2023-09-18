---
audience: end-user
title: Usar a atividade de fluxo de trabalho Alterar dimensão
description: Saiba como usar a atividade de workflow de alteração de dimensão
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 6%

---


# Mudar dimensão {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Gerar um complemento"
>abstract="Você pode gerar uma transição de saída adicional com a população restante, que foi excluída como uma duplicata. Para fazer isso, ative a opção **Gerar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Alterar atividade da dimensão"
>abstract="Essa atividade permite alterar o targeting dimension à medida que você constrói um público-alvo. Ele desloca o eixo dependendo do template de dados e da dimensão de entrada. Por exemplo, você pode alternar da dimensão &quot;contratos&quot; para a dimensão &quot;clientes&quot;."


A variável **Alterar dimensão** a atividade é um **Direcionamento** atividade. Essa atividade permite alterar o targeting dimension à medida que você constrói um público-alvo. Essa atividade altera o eixo dependendo do template de dados e da dimensão de entrada. Por exemplo, você pode alternar da dimensão &quot;contratos&quot; para a dimensão &quot;clientes&quot;.

Você também pode usar essa atividade para definir as colunas adicionais do novo target e os critérios de desduplicação de dados.

## Configuração

Siga estas etapas para configurar o **Alterar dimensão** atividade:

1. Adicionar um **Alterar dimensão** atividade ao seu fluxo de trabalho.

   ![](../assets/workflow-change-dimension.png)

1. Defina o **Nova dimensão de destino**.

Durante a alteração de dimensão, todos os registros são mantidos.