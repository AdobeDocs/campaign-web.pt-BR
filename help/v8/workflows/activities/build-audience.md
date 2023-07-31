---
audience: end-user
title: Usar a atividade de fluxo de trabalho Criar público-alvo
description: Saiba como usar a atividade de fluxo de trabalho Criar público-alvo
badge: label="Alfa"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 100%

---


# Criar público-alvo {#build-audience}

A atividade **Criar público-alvo** é uma atividade de **Direcionamento**. Essa atividade permite definir o público-alvo que entrará no fluxo de trabalho. Ao enviar mensagens no contexto de um fluxo de trabalho de campanha, o público-alvo da mensagem não é definido na atividade de canal, mas na atividade **Criar público-alvo**.

Para definir o público-alvo, você pode:

* Selecionar um público-alvo já existente, criado como lista no console do cliente.
* Selecionar um público-alvo da Adobe Experience Platform.
* Criar um público-alvo novo com o criador de regras definindo e combinando critérios de filtro.

>[!NOTE]
>
>Nesse contexto, não é possível carregar um público-alvo de um arquivo. Para isso, você precisa criar uma entrega independente. [Saiba mais](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuração

Siga estas etapas para configurar a atividade **Criar público-alvo**:

1. Adicione uma atividade **Criar público-alvo**.
1. Defina um rótulo.
1. Defina o tipo de público-alvo: **Crie o seu próprio** ou **Ler público-alvo**.

Para criar sua própria consulta, siga estas etapas adicionais:

1. Selecione **Crie sua própria (consulta)**.
1. Escolha a **Dimensão de direcionamento**. A dimensão de direcionamento permite definir a população-alvo da operação: destinatários, beneficiários de contrato, operadores, assinantes, etc. Por padrão, o público-alvo é selecionado entre os destinatários. Consulte a [Documentação v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Clique em **Continuar**.
1. Use o criador de regras para definir sua consulta, da mesma forma que você cria um público-alvo ao criar um novo email. Consulte esta [seção](../../audience/segment-builder.md).

Para selecionar um público-alvo existente, siga estas etapas:

1. Selecione **Ler público-alvo**.
1. Clique em **Continuar**.
1. Selecione seu público-alvo, da mesma forma que você usa um público-alvo ao criar um novo email. Consulte esta [seção](../../audience/add-audience.md).

## Exemplo

Este é um exemplo de um fluxo de trabalho com duas atividades de **Criar público-alvo**. A primeira é direcionada ao público-alvo dos jogadores de pôquer, seguida de uma entrega por email. A segunda é direcionada ao público-alvo de clientes VIP, seguida de uma entrega de SMS.

![](../assets/workflow-audience-example.png)