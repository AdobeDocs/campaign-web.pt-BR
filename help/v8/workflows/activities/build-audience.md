---
audience: end-user
title: Usar a atividade de fluxo de trabalho Criar público-alvo
description: Saiba como usar a atividade de fluxo de trabalho Criar público-alvo
badge: label="Beta"
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 75%

---

# Criar público-alvo {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Atividade criar público-alvo"
>abstract="A atividade **Criar público-alvo** permite definir o público-alvo que entrará no fluxo de trabalho. Ao enviar mensagens no contexto de um fluxo de trabalho, o público-alvo da mensagem não é definido na atividade canal, mas na atividade **Criar público-alvo**."


A atividade **Criar público-alvo** é uma atividade de **Direcionamento**. Essa atividade permite definir o público-alvo que entrará no fluxo de trabalho. Ao enviar mensagens no contexto de um fluxo de trabalho, o público-alvo da mensagem não é definido na atividade canal, mas na atividade **Criar público-alvo**.

Para definir o público-alvo, você pode:

* Selecionar um público-alvo já existente, criado como lista no console do cliente.
* Selecionar um público-alvo da Adobe Experience Platform.
* Criar um público-alvo novo com o criador de regras definindo e combinando critérios de filtro.

>[!NOTE]
>
>Nesse contexto, não é possível carregar um público-alvo de um arquivo. Para isso, você precisa criar um delivery de email independente. [Saiba mais](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurar a atividade Criar público{#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Selecione o targeting dimension"
>abstract="A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, o público-alvo é selecionado entre os destinatários."


Siga estas etapas para configurar a atividade **Criar público-alvo**:

![](../assets/workflow-audience.png)

1. Adicione uma atividade **Criar público-alvo**.
1. Defina um rótulo.
1. Defina o tipo de público-alvo: **Crie o seu próprio** ou **Ler público-alvo**.

Para criar sua própria consulta, siga estas etapas adicionais:

1. Selecione **Crie sua própria (consulta)**.
1. Escolha a **Dimensão de direcionamento**. A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, o público-alvo é selecionado entre os destinatários. Saiba mais sobre Targeting dimensions em [nesta seção](../../audience/about-recipients.md#targeting-dimensions).
1. Clique em **Continuar**.
1. Use o criador de regras para definir sua consulta, da mesma forma que você cria um público-alvo ao criar um novo email. Consulte esta [seção](../../audience/segment-builder.md).

Para selecionar um público-alvo existente, siga estas etapas:

1. Selecione **Ler público-alvo**.
1. Clique em **Continuar**.
1. Selecione seu público-alvo, da mesma forma que você usa um público-alvo ao criar um novo email. Consulte esta [seção](../../audience/add-audience.md).

>[!IMPORTANT]
>
>Se quiser usar um **[!UICONTROL Criar público-alvo]** atividade direcionada a um público-alvo Experience Platform, é necessário adicionar um **[!UICONTROL Alterar dimensão]** atividade após, para garantir que o targeting dimension do público-alvo seja definido como &quot;Recipient&quot;. Um exemplo de workflow está disponível na parte inferior desta página.

## Exemplos{#build-audience-examples}

Este é um exemplo de um fluxo de trabalho com duas atividades de **Criar público-alvo**. A primeira é direcionada ao público-alvo dos jogadores de pôquer, seguida de uma entrega por email. A segunda é direcionada ao público-alvo de clientes VIP, seguida de uma entrega de SMS.

![](../assets/workflow-audience-example.png)

Este é outro exemplo de fluxo de trabalho em que um público-alvo do Adobe Experience Platform é combinado com um público-alvo do Adobe Campaign. Para permitir que esses públicos sejam combinados, uma variável **[!UICONTROL Alterar dimensão]** A atividade com a dimensão de direcionamento &quot;Recipient&quot; é adicionada após o público-alvo da Adobe Experience Platform. [Saiba como configurar uma atividade de Change dimension](change-dimension.md)

![](../assets/workflow-audience-aep.png)
