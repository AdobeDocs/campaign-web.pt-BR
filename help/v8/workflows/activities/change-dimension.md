---
audience: end-user
title: Usar a atividade de fluxo de trabalho Alterar dimensão
description: Saiba como usar a atividade de workflow de alteração de dimensão
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: 52b129be88e48dd70c0f55b404fd3bbe699dbebb
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 26%

---

# Mudar dimensão {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Gerar um complemento"
>abstract="É possível gerar uma transição de saída adicional com a população restante, que foi excluída como uma duplicata. Para fazer isso, ative a opção **Gerar complemento**"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Atividade Mudar dimensão"
>abstract="Essa atividade permite alterar o targeting dimension à medida que você constrói um público-alvo. Ela desloca o eixo dependendo do modelo de dados e da dimensão de entrada. Por exemplo, você pode mudar da dimensão “contratos” para a dimensão “clientes”."

A atividade **Change dimension** é uma atividade **Targeting**. Essa atividade permite alterar o targeting dimension à medida que você constrói seu fluxo de trabalho. Ela desloca o eixo dependendo do modelo de dados e da dimensão de entrada. [Saiba mais sobre targeting dimensions](../../audience/about-recipients.md#targeting-dimensions)

Por exemplo, você pode alternar um targeting dimension de workflow de &quot;Recipients&quot; para &quot;Subscribers application&quot; para enviar notificações por push aos recipients alvos.

>[!IMPORTANT]
>
>Observe que as atividades **[!UICONTROL Alterar Dimensão]** e **[!UICONTROL Alterar Fonte de Dados]** não devem ser adicionadas em uma linha. Se você precisar usar ambas as atividades consecutivamente, certifique-se de incluir uma atividade **[!UICONTROL Enriquecimento]** entre elas. Isso garante a execução adequada e evita possíveis conflitos ou erros.

## Configurar a atividade Change dimension {#configure}

Siga estas etapas para configurar a atividade **Alterar dimensão**:

1. Adicione uma atividade **Change dimension** ao seu fluxo de trabalho.

   ![](../assets/workflow-change-dimension.png)

1. Defina a **Nova dimensão de destino**. Durante a alteração de dimensão, todos os registros são mantidos. Outras opções ainda não estão disponíveis.

1. Execute o workflow para visualizar o resultado. Compare os dados nas tabelas antes e depois da atividade de alteração de dimensão e compare a estrutura das tabelas do workflow.

## Exemplo {#example}

Neste exemplo, queremos enviar um delivery de SMS para todos os perfis que fizeram uma compra. Para fazer isso, primeiro usamos uma atividade **[!UICONTROL Build audience]** vinculada a uma dimensão de direcionamento &quot;Purchase&quot; personalizada para direcionar todas as compras que ocorreram.

Em seguida, usamos uma atividade **[!UICONTROL Change dimension]** para alternar o targeting dimension do workflow para &quot;Recipients&quot;. Isso nos permite direcionar os recipients que correspondem ao query.

![](../assets/workflow-change-dimension-example.png)
