---
audience: end-user
title: Usar a atividade de workflow Criar público
description: Saiba como usar a atividade de workflow Criar público
badge: label="Alpha" type="Positive"
source-git-commit: 79e839a99b41f8ae918a5651990149c864f201e7
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 15%

---


# Criar público-alvo {#build-audience}

Esta atividade permite definir um público-alvo. Você pode selecionar um público existente ou usar o construtor de regras para definir sua própria consulta.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuração

Siga estas etapas para configurar o **Criar público-alvo** atividade:

1. Adicione uma atividade Build audience.
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
