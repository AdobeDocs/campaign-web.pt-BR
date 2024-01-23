---
audience: end-user
title: Usar um público-alvo da Adobe Experience Platform
description: Saiba como usar um público-alvo da Adobe Experience Platform
badge: label="Disponibilidade limitada"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 703196ad2bb504eb1d50008af110f952d8045eaa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 28%

---

# Usar um público-alvo da Adobe Experience Platform{#aep-audience}

Os conectores de Destino e Origem do Cloud Service gerenciado da Adobe Campaign permitem uma integração perfeita entre o Adobe Campaign e o Adobe Experience Platform.

Depois de criar um público-alvo do Adobe Experience Platform e disponibilizá-lo no console do cliente, você pode usá-lo da mesma forma que faria para um público-alvo do Campaign personalizar e enviar mensagens.

>[!NOTE]
>
>Para usar os públicos da Adobe Experience Platform no Campaign, você precisa configurar a integração com Fontes e Destinos do Adobe. Consulte [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

Para selecionar o público de um delivery, você também pode:

* Crie um novo público-alvo. [Saiba mais](../query/query-modeler-overview.md)
* Carregar um público-alvo de um arquivo externo. [Saiba mais](file-audience.md)
* Use um público existente do Campaign. [Saiba mais](add-audience.md).

Para selecionar um público-alvo da Adobe Experience Platform para o seu delivery, siga as etapas abaixo:

1. Na seção **Público**, do assistente de criação de entrega, clique no botão **[!UICONTROL Selecionar público-alvo]**.

   ![](assets/create-audience.png)

1. Escolha a **[!UICONTROL Selecionar público-alvo]** para usar um público existente. Para criar um novo público-alvo a ser usado neste email, escolha **Criar seu próprio**. Consulte esta [seção](../query/query-modeler-overview.md).

   Essa tela exibe todos os públicos-alvo existentes definidos no console do cliente Adobe Campaign para a pasta atual. Para escolher um público-alvo do Adobe Experience Platform, navegue até o `AEP Audiences folder` na seção de filtro da tela.

   ![](assets/select-audience-folder.png)

   Você também pode definir uma regra para filtrar a origem dos públicos-alvo, conforme abaixo:

   A seção de filtro permite acessar opções de filtragem para refinar a lista de públicos-alvo. Para fazer isso, clique em **Adicionar regras** para acessar o modelador de consultas, que permite criar filtros avançados para a lista de públicos-alvo. [Saiba como usar o modelador de consultas](../query/query-modeler-overview.md)

   ![](assets/filter-on-aep-audience.png)

1. Escolha um público-alvo e clique em **Selecionar**.

1. Clique em **Editar regras** se quiser refinar seu público-alvo.

   ![](assets/refine-audience.png)

1. Com o modelador de query, você pode enriquecer o público-alvo com filtros adicionais ou combinando públicos-alvo diferentes. Consulte esta [seção](../query/query-modeler-overview.md).

1. Clique em **Salvar**.
