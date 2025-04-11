---
audience: end-user
title: Criar um público-alvo único para uma entrega
description: Saiba como criar um público-alvo único para uma entrega.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 13%

---

# Criar um público-alvo único {#one-time}

Esta seção explica como criar um público-alvo ao criar um novo delivery. Nesse cenário, os perfis incluídos no público-alvo do delivery são direcionados consultando o banco de dados usando o modelador de consultas. O público resultante é usado apenas uma vez para esse delivery e não é salvo na lista de públicos.

Ao definir o target principal de um delivery, você também pode:
* [Selecione um público-alvo](add-audience.md) na lista **[!UICONTROL Públicos-alvo]**.
* [Carregar um público de um arquivo externo](file-audience.md) (somente para emails).

Para criar um novo público-alvo único para um delivery, siga estas etapas:

1. Na seção **Público**, do assistente de criação de entrega, clique no botão **[!UICONTROL Selecionar público-alvo]**.

   [Captura de tela mostrando a seção Público-alvo do assistente de criação de entrega com o botão Selecionar público-alvo realçado](assets/segment-builder0.png){zoomable="yes"}

1. Selecione **Criar o seu próprio** para abrir o modelador de consultas. O modelador de query permite definir o público-alvo filtrando os dados contidos no banco de dados. [Saiba como usar o modelador de consultas](../query/query-modeler-overview.md).

   [Captura de tela mostrando a interface do modelador de consultas](assets/query-modeler.png){zoomable="yes"}

1. Quando a consulta estiver pronta, clique em **Confirmar** para usar o público-alvo resultante como o principal destino da sua entrega.

   Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não receberam. [Saiba mais](control-group.md).