---
audience: end-user
title: Selecione um público-alvo existente
description: Saiba como selecionar um público-alvo
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 34%

---


# Selecione um público-alvo já existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecione um público-alvo já existente"
>abstract="Navegue pela lista para selecionar um público-alvo já existente. Use o ícone “Mostrar filtros” para filtrar a lista ou selecione uma pasta específica."

Esta seção explica como selecionar um público-alvo ao definir a população do target de um delivery. Ao definir o target principal de um delivery, você também pode:

* [Criar um público-alvo único](one-time-audience.md) usando o modelador de consultas.
* [Carregar um público-alvo de um arquivo externo](file-audience.md) (somente para emails).

Os públicos-alvo que podem ser direcionados em deliveries podem ser acessados no **Público** menu esquerdo. Eles são originários de várias fontes, como o console do cliente, os workflows de público-alvo da Web do Campaign ou o Adobe Experience Platform. [Saiba como monitorar e gerenciar públicos](manage-audience.md)

Para selecionar um público-alvo existente para sua mensagem, siga as etapas abaixo:

1. No **Público** do assistente de criação de delivery, clique no link **[!UICONTROL Selecionar público]** e escolha

   ![](assets/create-audience.png)

1. Escolha a **[!UICONTROL Selecionar público-alvo]** para usar um público existente. Esta tela exibe todos os públicos-alvo existentes para a pasta atual.

   ![](assets/create-audience2.png)

   Para escolher um público-alvo do Adobe Experience Platform, navegue até o `AEP Audiences folder` na seção de filtro da tela.

   ![](assets/select-audience-folder.png)

1. A seção de filtro permite acessar opções de filtragem para refinar a lista de públicos-alvo. Para fazer isso, clique em **Adicionar regras** para acessar o modelador de consultas, que permite criar filtros avançados para a lista de públicos-alvo. [Saiba como usar o modelador de consultas](../query/query-modeler-overview.md)

   ![](assets/create-audience4.png)

1. Clique em **Confirmar o** para adicionar seu público-alvo como o target principal do delivery. Depois de concluído, ainda é possível refinar o público-alvo usando o modelador de consulta clicando no link **Editar regras** botão.

   ![](assets/refine-audience.png)

   Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não a receberam. [Saiba mais](control-group.md)
