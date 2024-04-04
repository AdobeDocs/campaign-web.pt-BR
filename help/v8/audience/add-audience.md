---
audience: end-user
title: Selecione um público-alvo existente
description: Saiba como selecionar um público-alvo
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: b166d06215e06d6426ab9ce9a757fcc041810df9
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Selecione um público-alvo já existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecione um público-alvo já existente"
>abstract="Navegue pela lista para selecionar um público-alvo já existente. Use o ícone “Mostrar filtros” para filtrar a lista ou selecione uma pasta específica."

Esta seção explica como selecionar um público-alvo ao definir a população do target de um delivery. Ao definir o target principal de um delivery, você também pode:
* [Criar um público-alvo único](one-time-audience.md) usando o modelador de consultas.
* [Carregar um público-alvo de um arquivo externo](file-audience.md) (somente para emails).

Os públicos-alvo que podem ser direcionados em deliveries podem ser acessados no **Público** menu esquerdo. Eles são originários de várias fontes, como o console do cliente, os workflows de público-alvo da Web do Campaign ou o Adobe Experience Platform. [Saiba mais sobre públicos-alvo](manage-audience.md)

Para selecionar um público-alvo existente para sua mensagem, siga as etapas abaixo:

1. No **Público** do assistente de criação de delivery, clique no link **[!UICONTROL Selecionar público]** e escolha **[!UICONTROL Selecionar público]**.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

1. Esta tela exibe todos os públicos-alvo existentes para a pasta atual.

   ![](assets/create-audience2.png){zoomable=&quot;yes&quot;}

   Para escolher um público-alvo do Adobe Experience Platform, navegue até o `AEP Audiences folder` na seção de filtro da tela. [Saiba mais sobre públicos da Adobe Experience Platform](manage-audience.md#monitor)

   ![](assets/select-audience-folder.png){zoomable=&quot;yes&quot;}

1. A seção de filtro permite acessar opções de filtragem para refinar a lista de públicos-alvo. Para fazer isso, clique em **Adicionar regras** para acessar o modelador de consultas, que permite criar filtros avançados para a lista de públicos-alvo. [Saiba como usar o modelador de consultas](../query/query-modeler-overview.md)

   Por exemplo, é possível definir uma regra para filtrar a origem dos públicos-alvo, conforme mostrado abaixo:

   ![](assets/filter-on-aep-audience.png){zoomable=&quot;yes&quot;}

1. Clique em **Confirmar o** para adicionar seu público-alvo como o target principal do delivery. Depois de concluído, ainda é possível refinar o público-alvo usando o modelador de consulta clicando no link **Editar regras** botão.

   ![](assets/refine-audience.png){zoomable=&quot;yes&quot;}

   Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não a receberam. [Saiba mais](control-group.md)
