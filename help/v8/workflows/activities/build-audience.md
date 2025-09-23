---
audience: end-user
title: Usar a atividade de fluxo de trabalho Criar público-alvo
description: Saiba como usar a atividade de fluxo de trabalho Criar público-alvo
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 57%

---

# Criar público-alvo {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Atividade Criar público-alvo"
>abstract="A atividade **Criar público-alvo** permite definir o público-alvo que entrará no fluxo de trabalho. Ao enviar mensagens no contexto de um fluxo de trabalho, o público-alvo da mensagem não é definido na atividade canal, mas na atividade **Criar público-alvo**."

A atividade **Criar público-alvo** é uma atividade de **Direcionamento**. Essa atividade permite definir o público-alvo que entrará no fluxo de trabalho. Ao enviar mensagens no contexto de um fluxo de trabalho, o público-alvo da mensagem não é definido na atividade canal, mas na atividade **Criar público-alvo**.

Para definir a população que servirá de público-alvo, você pode:

* Selecionar um público-alvo já existente, criado como lista no console do cliente.
* Selecionar um público-alvo da Adobe Experience Platform.
* Crie um novo público-alvo com o modelador de consultas definindo e combinando critérios de filtragem.

>[!NOTE]
>
>Os públicos carregados de um arquivo não podem ser direcionados usando uma atividade Criar público. Para fazer isso, você precisa usar uma atividade **Carregar arquivo** seguida por uma atividade **Reconciliação**. [Saiba mais](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configurar a atividade Criar público-alvo {#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_audienceselector"
>title="Público-alvo"
>abstract="Selecione o público-alvo assim como faz ao criar uma nova entrega. "

Siga estas etapas para configurar a atividade **Criar público-alvo**:

![Captura de tela mostrando a interface de configuração de público do fluxo de trabalho.](../assets/workflow-audience.png)

1. Adicione uma atividade **Criar público-alvo**.
1. Defina um rótulo.
1. Defina o tipo de público-alvo: **Crie o seu próprio** ou **Ler público-alvo**.
1. Configure seu público seguindo as etapas detalhadas nas guias abaixo.

>[!BEGINTABS]

>[!TAB Crie o seu próprio (consulta)]

Para criar sua própria query, siga estas etapas:

1. Selecione **Crie sua própria (consulta)**.
1. Escolha a **Dimensão de direcionamento**. O targeting dimension permite definir o público alvo da operação, como recipients, beneficiários de contrato, operadores ou assinantes. Por padrão, o público-alvo é selecionado entre os destinatários. [Saiba mais sobre dimensões de direcionamento](../../audience/targeting-dimensions.md#targeting)
1. Escolha a **Dimensão do filtro** clicando no ícone ao lado da targeting dimension. A dimensão de filtro permite aplicar filtros ao público-alvo fazendo referência a critérios relacionados sem alterar a dimensão de direcionamento principal. [Saiba mais sobre dimensões de direcionamento](../../audience/targeting-dimensions.md#filtering)
1. Clique em **Continuar**.
1. Use o modelador de consultas para definir seu query, da mesma forma que você cria um público-alvo ao criar um novo email. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md)

>[!TAB Ler público-alvo]

Para selecionar um público-alvo existente, siga estas etapas:

1. Selecione **Ler público-alvo**.
1. Clique em **Continuar**.
1. Selecione seu público, da mesma forma que você usa um público ao criar um novo delivery. Consulte esta [seção](../../audience/add-audience.md).

>[!ENDTABS]

## Exemplos {#build-audience-examples}

Este é um exemplo de um fluxo de trabalho com duas atividades de **Criar público-alvo**. A primeira é direcionada ao público-alvo dos jogadores de pôquer, seguida de uma entrega por email. A segunda é direcionada ao público-alvo de clientes VIP, seguida de uma entrega de SMS.

![Captura de tela mostrando um exemplo de fluxo de trabalho com duas atividades de criação de público-alvo direcionadas a públicos-alvo diferentes.](../assets/workflow-audience-example.png)