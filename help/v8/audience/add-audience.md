---
audience: end-user
title: Selecione um público-alvo existente
description: Saiba como selecionar um público-alvo
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 0830c7d7b7bba10f573ea58fa5aacd5e5e9ddccb
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 36%

---


# Selecione um público-alvo já existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecione um público-alvo já existente"
>abstract="Navegue pela lista para selecionar um público-alvo já existente. Use o ícone “Mostrar filtros” para filtrar a lista ou selecione uma pasta específica."

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Refinar público-alvo"
>abstract="Essas regras só podem ser alteradas no console de desktop."

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Público-alvo adicional"
>abstract="Essas regras só podem ser alteradas no console de desktop."

Esta seção explica como selecionar uma público-alvo existente ao definir a população Direcionamento de um delivery. Ao definir as Direcionamento principais de uma delivery, também é possível:
* [Crie uma público-alvo](one-time-audience.md) única vez usando o modelador de query.
* [Carregue uma público-alvo de um arquivo](file-audience.md) externo (somente para emails).

Audiences que podem ser direcionadas nos deliveries são acessíveis a partir do menu esquerdo público-alvo ****. Eles são originários de diversas fontes, como o console Cliente, Campaign Público-alvo workflows Web ou Adobe Experience Platform. [Saiba mais sobre públicos-alvo](manage-audience.md)

Para selecionar um público-alvo existente para sua mensagem, siga as etapas abaixo:

1. **Na seção Público-alvo** do assistente de criação de delivery, clique na opção **[!UICONTROL Selecionar público-alvo botão]** e escolha **[!UICONTROL Selecionar público-alvo]**.

   ![](assets/create-audience.png){zoomable="yes"}

1. Esta tela exibe todos os públicos-alvo existentes, para a pasta atual.

   ![](assets/create-audience2.png){zoomable="yes"}

   Para escolher um público-alvo de Adobe Experience Platform, navegue até a `AEP Audiences folder` seção de filtro da tela. [Saiba mais sobre públicos-alvo do Adobe Experience Platform](manage-audience.md#monitor)

   ![](assets/select-audience-folder.png){zoomable="yes"}

1. A seção de filtro permite acessar opções de filtragem para refinar os públicos-lista. Para fazer isso, clique **em Adicionar regras** para acessar o modelador de query, que permite criar filtros avançados para as lista de públicos-alvo. [Aprenda a usar o modelador de query](../query/query-modeler-overview.md)

   Por exemplo, você pode definir uma regra para filtrar na origem dos públicos-alvo, conforme mostrado abaixo:

   ![](assets/filter-on-aep-audience.png){zoomable="yes"}

1. Clique **em Confirmar** para adicionar sua público-alvo como a delivery principal Direcionamento. Depois de concluído, você ainda pode refinar os público-alvo usando o modelador query clicando nas **regras** Editar botão.

   ![](assets/refine-audience.png){zoomable="yes"}

   Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não a receberam. [Saiba mais](control-group.md)
