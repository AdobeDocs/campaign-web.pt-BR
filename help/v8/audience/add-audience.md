---
audience: end-user
title: Selecione um público existente
description: Saiba como selecionar um público
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positive"
source-git-commit: d4645689ebaa5439a01b2f558f398cbeb79089a7
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 95%

---


# Selecione um público existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecione um público existente"
>abstract="Os públicos são definidos no Console do Adobe Campaign v8. Se tiver uma integração da Adobe Experience Platform disponível, você também poderá ver públicos definidos pela Platform."

Esta seção explica como selecionar um público existente ao definir o público-alvo de uma entrega de email.

Você também pode:

* Crie um novo público-alvo. [Saiba mais](segment-builder.md)
* Carregar um público-alvo de um arquivo externo. [Saiba mais](file-audience.md)
* Usar um público da Adobe Experience Platform. [Saiba mais](aep-audience.md).


Para selecionar um público existente para sua mensagem, siga as etapas abaixo:

1. Na seção **Público**, do assistente de criação de entrega, clique no botão **[!UICONTROL Selecionar público]**.

   ![](assets/create-audience.png)

1. Escolha a **[!UICONTROL Selecionar público]** para usar um público existente. Para criar um novo público a ser usado neste email, escolha **Criar seu próprio**. Consulte esta [seção](segment-builder.md).

   Essa tela exibe todos os públicos existentes definidos no console do Adobe Campaign ou na Adobe Experience Platform.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Para aproveitar os públicos da Adobe Experience Platform, é necessário configurar a integração com o serviço de Destinos. Consulte a [Documentação de Destinos](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR){target="_blank"}.

1. Escolha um público e clique em **Selecionar**.

1. Clique em **Editar regras** se quiser refinar seu público.

   ![](assets/create-audience3.png)

1. Usando o construtor de regras, você pode enriquecer seu público com filtros adicionais ou combinar públicos diferentes. Consulte esta [seção](segment-builder.md).

   ![](assets/create-audience4.png)

1. Clique em **Salvar**.

Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos que não a receberam. Consulte esta [seção](control-group.md).