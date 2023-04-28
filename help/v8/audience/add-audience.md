---
audience: end-user
title: Selecionar um público
description: Saiba como selecionar um público
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
badge: label="Alpha" type="Positive"
source-git-commit: cf94ea6f5bbb287c5cd56f5af023a40d1f8538d6
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 25%

---


# Selecione um público existente {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecione um público existente"
>abstract="Os públicos são definidos no Console do Adobe Campaign v8. Se tiver uma integração da Adobe Experience Platform disponível, você também poderá ver públicos definidos pela Platform."

Esta seção explica como selecionar um público-alvo existente ao definir o público-alvo de um delivery de email.

Você também pode:

* Crie um novo público-alvo. [Saiba mais](segment-builder.md)
* Importar um público de um arquivo. [Saiba mais](import-audience.md)
* Usar um público-alvo da Adobe Experience Platform. [Saiba mais](aep-audience.md).


Para selecionar um público-alvo existente para sua mensagem, siga as etapas abaixo:

1. No **Público** seção do assistente de criação de delivery, clique no link **[!UICONTROL Seleção do público-alvo]** botão.

   ![](assets/create-audience.png)

1. Choose **[!UICONTROL Seleção do público-alvo]** para usar um público-alvo existente. Para criar um novo público-alvo a ser usado neste email, escolha **Crie seu próprio**. Consulte esta [seção](segment-builder.md).

   Essa tela exibe todos os públicos-alvo existentes definidos no console Adobe Campaign ou no Adobe Experience Platform.

   ![](assets/create-audience2.png)

   >[!NOTE]
   >
   >Para aproveitar os públicos-alvo do Adobe Experience Platform, é necessário configurar a integração com Destinos. Consulte a [Documentação de destinos](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR){target="_blank"}.

1. Escolha um público-alvo e clique em **Selecionar**.

1. Clique em **Editar regras** se quiser refinar seu público-alvo.

   ![](assets/create-audience3.png)

1. Usando o construtor de regras, você pode enriquecer seu público-alvo com filtros adicionais ou combinando públicos-alvo diferentes. Consulte esta [seção](segment-builder.md).

   ![](assets/create-audience4.png)

1. Clique em **Save**.

Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não recebe a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos, o que não aconteceu. Consulte [seção](control-group.md).