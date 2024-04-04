---
audience: end-user
title: Criar um público-alvo único para uma entrega
description: Saiba como criar um público-alvo único para uma entrega.
exl-id: 6f2da017-90d6-497d-bbbd-293775da00e9
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 29%

---

# Criar um público-alvo único {#one-time}

Esta seção descreve como criar um público-alvo ao criar um novo delivery. Nesse caso, os perfis a serem incluídos no público-alvo do delivery são direcionados consultando o banco de dados com o modelador de query. O público resultante é usado apenas uma vez para essa entrega. Ela não é salva na lista de públicos-alvo.

Ao definir o target principal de um delivery, você também pode:
* [Selecionar um público existente](add-audience.md) do **[!UICONTROL Públicos-alvo]** lista.
* [Carregar um público-alvo de um arquivo externo](file-audience.md) (somente para emails).

Para criar um novo público-alvo único para um delivery, siga estas etapas:

1. Na seção **Público**, do assistente de criação de entrega, clique no botão **[!UICONTROL Selecionar público-alvo]**.

   ![](assets/segment-builder0.png){zoomable=&quot;yes&quot;}

1. Selecionar **Crie o seu próprio** para abrir o modelador de query, que permite definir o público-alvo filtrando os dados contidos no banco de dados. [Saiba como usar o modelador de consultas](../query/query-modeler-overview.md)

   ![](assets/query-modeler.png){zoomable=&quot;yes&quot;}

1. Quando a consulta estiver pronta, clique em **Confirmar o** para usar o público-alvo resultante como o principal target do seu delivery.

   Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não a receberam. [Saiba mais](control-group.md)
