---
audience: end-user
title: Adicionar um público-alvo
description: Documentação da Web do Campaign v8
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: d5fa13813a22b21fdedd90475ee9258f5003e22d
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 7%

---

# Selecionar um público-alvo {#add-audience}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Selecionar um público-alvo existente"
>abstract="Os públicos-alvo são definidos no Console do Adobe Campaign v8. Se tiver uma integração do Adobe Experience Platform disponível, você também poderá ver públicos-alvo definidos pela plataforma."

Esta seção explica como selecionar um público-alvo existente ao definir o público-alvo de um delivery de email. Para criar um novo público-alvo, consulte esta seção [seção](segment-builder.md).

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

Você também pode definir um grupo de controle para medir o impacto de suas campanhas. O grupo de controle não receberá a mensagem. Isso permite comparar o comportamento da população que recebeu a mensagem com o comportamento dos contatos, o que não aconteceu. Consulte [seção](control-group.md).