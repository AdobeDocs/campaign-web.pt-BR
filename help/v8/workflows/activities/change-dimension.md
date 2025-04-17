---
audience: end-user
title: Usar a atividade de fluxo de trabalho Alterar dimensão
description: Saiba como usar a atividade de workflow de alteração de dimensão
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 21%

---

# Mudar dimensão {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Gerar um complemento"
>abstract="É possível gerar uma transição de saída adicional com a população restante, que foi excluída como uma duplicata. Para fazer isso, ative a opção **Gerar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Atividade Mudar dimensão"
>abstract="Essa atividade permite alterar o targeting dimension à medida que você constrói um público-alvo. Ela desloca o eixo dependendo do modelo de dados e da dimensão de entrada. Por exemplo, você pode alternar da dimensão &quot;contratos&quot; para a dimensão &quot;clientes&quot;."

A atividade **Change dimension** é uma atividade **Targeting**. Essa atividade permite alterar o targeting dimension à medida que você constrói seu fluxo de trabalho. Ela desloca o eixo dependendo do modelo de dados e da dimensão de entrada. [Saiba mais sobre dimensões de direcionamento](../../audience/about-recipients.md#targeting-dimensions).

Por exemplo, você pode alternar o targeting dimension de um fluxo de trabalho de &quot;Recipients&quot; para &quot;Aplicativo de assinante&quot; para enviar notificações por push aos recipients direcionados.

>[!IMPORTANT]
>
>Observe que as atividades **[!UICONTROL Alterar Dimensão]** e **[!UICONTROL Alterar Fonte de Dados]** não devem ser adicionadas em uma linha. Se você precisar usar ambas as atividades consecutivamente, inclua uma atividade **[!UICONTROL Enriquecimento]** entre elas. Isso garante a execução adequada e evita possíveis conflitos ou erros.

## Configurar a atividade Change dimension {#configure}

Siga estas etapas para configurar a atividade **Alterar dimensão**:

1. Adicione uma atividade **Change dimension** ao seu fluxo de trabalho.

   ![Captura de tela mostrando a atividade Change dimension adicionada a um fluxo de trabalho](../assets/workflow-change-dimension.png)

1. Defina a **Nova dimensão de destino**. Durante a alteração de dimensão, todos os registros são mantidos. Outras opções ainda não estão disponíveis.

1. Execute o workflow para visualizar o resultado. Compare os dados nas tabelas antes e depois da atividade Change dimension e compare a estrutura das tabelas do workflow.

## Exemplo {#example}

Neste exemplo, envie um delivery SMS para todos os perfis que fizeram uma compra. Primeiro, use uma atividade **[!UICONTROL Build audience]** vinculada a uma dimensão de direcionamento &quot;Purchase&quot; personalizada para direcionar todas as compras que ocorreram.

Em seguida, use uma atividade **[!UICONTROL Change dimension]** para alternar o targeting dimension do fluxo de trabalho para &quot;Recipients&quot;. Isso permite direcionar os recipients que correspondem ao query.

![Captura de tela mostrando um exemplo da atividade Change dimension usada em um fluxo de trabalho](../assets/workflow-change-dimension-example.png)