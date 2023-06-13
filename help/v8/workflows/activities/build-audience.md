---
audience: end-user
title: Usar a atividade de workflow Criar público
description: Saiba como usar a atividade de workflow Criar público
badge: label="Alpha" type="Positive"
source-git-commit: bbebd9dc462a189618cbf6e71467bb0935e1317a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 9%

---


# Criar público-alvo {#build-audience}

A variável **Criar público-alvo** a atividade é um **Direcionamento** atividade. Essa atividade permite definir o público-alvo que entrará no fluxo de trabalho. Ao enviar mensagens no contexto de um workflow de campanha, o público-alvo da mensagem não é definido na atividade de canal, mas no **Criar público-alvo** atividade.

Para definir a população do público-alvo, é possível:

* Selecione um público existente, criado como uma lista no console do cliente.
* Selecione um público-alvo do Adobe Experience Platform.
* Crie um novo público-alvo com o construtor de regras definindo e combinando critérios de filtragem.

>[!NOTE]
>
>Nesse contexto, não é possível carregar um público-alvo de um arquivo. Para isso, você precisa criar um delivery independente. [Saiba mais](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuração

Siga estas etapas para configurar o **Criar público-alvo** atividade:

1. Adicionar um **Criar público-alvo** atividade.
1. Defina um rótulo.
1. Defina o tipo de público-alvo: **Crie o seu próprio** ou **Ler público**.

Para criar sua própria query, siga estas etapas adicionais:

1. Selecionar **Crie o seu próprio (consulta)**.
1. Escolha o **Dimensão de direcionamento**. O targeting dimension permite definir o público alvo da operação: recipients, beneficiários de contrato, operadores, assinantes etc. Por padrão, o target é selecionado dos recipients. Consulte a [Documentação do v8](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Clique em **Continue**.
1. Use o construtor de regras para definir seu query, da mesma forma que você cria um público-alvo ao criar um novo email. Consulte esta [seção](../../audience/segment-builder.md).

Para selecionar um público existente, siga estas etapas:

1. Selecionar **Ler público**.
1. Clique em **Continue**.
1. Selecione seu público, da mesma forma que você usa um público ao criar um novo email. Consulte esta [seção](../../audience/add-audience.md).

## Exemplo

Este é um exemplo de um fluxo de trabalho com dois **Criar público-alvo** atividades. O primeiro é direcionado ao público-alvo dos jogadores de pôquer, seguido de um delivery por email. O segundo é direcionado ao público-alvo de clientes VIP, seguido de um delivery de SMS.

![](../assets/workflow-audience-example.png)