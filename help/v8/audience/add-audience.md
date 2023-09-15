---
audience: end-user
title: Selecione um público-alvo já existente
description: Saiba como selecionar um público
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Beta"
source-git-commit: d05b6f9fec0e56f90d3fe51014fc11d2ed87bb66
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 57%

---


# Selecione um público-alvo já existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecione um público-alvo já existente"
>abstract="Navegue pela lista para selecionar um público-alvo já existente. Use o ícone “Mostrar filtros” para filtrar a lista ou selecione uma pasta específica."

Esta seção explica como selecionar um público existente ao definir o público-alvo de uma entrega de email.

Você também pode:

* Crie um novo público-alvo. [Saiba mais](segment-builder.md)
* Carregar um público-alvo de um arquivo externo (somente para emails). [Saiba mais](file-audience.md)
* Usar um público da Adobe Experience Platform. [Saiba mais](aep-audience.md).


Para selecionar um público existente para sua mensagem, siga as etapas abaixo:

1. Na seção **Público**, do assistente de criação de entrega, clique no botão **[!UICONTROL Selecionar público-alvo]**.

   ![](assets/create-audience.png)

1. Escolha a **[!UICONTROL Selecionar público-alvo]** para usar um público existente. Para criar um novo público a ser usado neste email, escolha **Criar seu próprio**. Consulte esta [seção](segment-builder.md).

   Esta tela exibe todos os públicos-alvo existentes para a pasta atual.

   ![](assets/create-audience2.png)

   Os públicos-alvo são criados no **Público** menu esquerdo. Eles também podem ser criados no Console do cliente.

   Para usar os públicos da Adobe Experience Platform, é necessário configurar a integração com o Destinations. Consulte a [Documentação de destinos do Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR){target="_blank"}.

   >[!IMPORTANT]
   >
   >Nessa versão do produto, ao criar regras, selecionar o público-alvo de um delivery ou ao criar um público-alvo em um fluxo de trabalho, alguns filtros predefinidos não estão disponíveis na interface. Você ainda pode usá-las. [Saiba mais](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

1. Escolha um público e clique em **Selecionar**.
1. Use o **Mostrar filtros** ícone para exibir opções de filtragem. Clique em **Adicionar regras** para acessar o construtor de regras: o uso do construtor de regras permite que você crie filtros avançados para a lista de públicos-alvo. Saiba como usar o construtor de regras neste [seção](segment-builder.md).

   ![](assets/create-audience4.png)

1. Clique em **Salvar**.

Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não a receberam. Saiba mais [nesta seção](control-group.md).