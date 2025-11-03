---
title: Trabalhar com o GenStudio for Performance Marketing no Adobe Campaign
description: Saiba como trabalhar com o GenStudio for Performance Marketing no Adobe Campaign
feature: Email Design
topic: Content Management, Artificial Intelligence
badge: label="Disponibilidade limitada" type="Informative"
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 8%

---

# Trabalhar com o GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Usar um modelo criado com o GenStudio"
>abstract="Graças à integração perfeita com o Adobe GenStudio for Performance Marketing, você pode importar facilmente um modelo do GenStudio aprimorado com a tecnologia de IA da Adobe."

## Introdução ao GenStudio {#gs-genstudio}

O [Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} é um aplicativo generativo de IA que permite que as equipes de marketing criem seus próprios anúncios e emails para impulsionar campanhas de marketing personalizadas e impactantes que seguem os padrões da sua marca e estão em conformidade com as políticas da sua empresa. Ao utilizar a tecnologia de IA do Adobe, ele fornece um conjunto abrangente de ferramentas que simplificam as complexidades da criação e do gerenciamento de conteúdo para que os criadores possam se concentrar na inovação.

>[!AVAILABILITY]
>
>Esse recurso está disponível somente para o canal de email.

Para aprimorar a eficiência do marketing e manter a consistência da marca, você pode integrar perfeitamente as experiências do [!DNL **GenStudio for Performance Marketing**] com o [!DNL **Adobe Campaign**]. Isso permite que você aproveite a criação de conteúdo com recursos de orquestração avançada do [!DNL GenStudio].[!DNL Adobe Campaign]

>[!INFO]
>
>Para ir além, confira esta [visão geral](https://business.adobe.com/br/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} e uma [demonstração](https://business.adobe.com/br/products/genstudio-for-performance-marketing.html#demo){target="_blank"} de [!DNL Adobe GenStudio for Performance Marketing].

## Usar os recursos do GenStudio no Adobe Campaign {#use-genstudio}

A integração do [!DNL GenStudio for Performance Marketing] e do [!DNL Adobe Campaign] permite que os profissionais de marketing da sua empresa trabalhem melhor em conjunto para simplificar processos.

Por exemplo, um profissional de marketing técnico, que usa o [!DNL Adobe Campaign] para desenvolver e automatizar campanhas de email, pode colaborar com um profissional de marketing de desempenho que cria conteúdo usando o [!DNL GenStudio].

Com essa integração, ambos podem trabalhar em conjunto para integrar facilmente o conteúdo sob a marca do [!DNL GenStudio] ao [!DNL Adobe Campaign], fornecendo emails envolventes direcionados a segmentos específicos de clientes e impulsionando as vendas.

### Exportar um modelo do HTML do Adobe Campaign para o GenStudio {#export-from-campaign-to-genstudio}

Primeiro, você pode exportar um modelo do HTML [!DNL Adobe Campaign] incluindo as diretrizes da sua marca para [!DNL GenStudio for Performance Marketing]. Siga as etapas abaixo.

1. No [!DNL Adobe Campaign], acesse o conteúdo do seu email. [Saiba como](../email/create-email.md#create-content)

1. No Designer Email, selecione **[!UICONTROL Exportar HTML]** no botão **[!UICONTROL Mais]**.

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Carregar este modelo exportado do HTML em [!DNL GenStudio for Performance Marketing]. <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >Saiba como carregar um modelo do HTML no [!DNL GenStudio] na seção dedicada do [Guia do Usuário do Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}.<!--GenStudio doc to be updated with Campaign-->

1. No GenStudio, use esse template para criar várias variações de email com prompts de IA e salvá-las.

   >[!NOTE]
   >
   >Saiba como criar experiências de email na [seção](https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"} dedicada do GenStudio.

### Aproveitar as experiências do GenStudio no Adobe Campaign {#leverage-genstudio-experiences}

Para aproveitar as variações de email do [!DNL GenStudio] que você acabou de criar importando-as para o [!DNL Adobe Campaign], siga as etapas abaixo.

1. Em [!DNL Adobe Campaign], [crie uma entrega de email](../email/create-email.md).

1. No painel de delivery de email, clique no botão **[!UICONTROL Editar conteúdo]**. [Saiba mais](../email/create-email.md#create-content)

1. Na página inicial do Designer de Email, selecione **[!UICONTROL Importar HTML]** e clique no botão **[!UICONTROL Adobe GenStudio for Performance Marketing]**.

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Navegue pelas experiências do GenStudio para começar a criar o conteúdo. Você pode filtrar as experiências em vários critérios, como produtos, personas, marcas ou até mesmo cores.

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Selecione uma experiência e clique em **[!UICONTROL Usar]**.

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Selecione a pasta na qual deseja importar a experiência do GenStudio.

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. O conteúdo selecionado é exibido no Designer de email.

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >As experiências do GenStudio [criadas a partir de um [!DNL Adobe Campaign] modelo](#export-from-ajo-to-genstudio) são importadas diretamente para o Designer de email. As experiências do GenStudio criadas sem um modelo [!DNL Adobe Campaign] são importadas para o [modo de compatibilidade](../email/existing-content.md).

   Use as [ferramentas de edição de conteúdo de email](../email/create-email-content.md) e os [campos de personalização](../personalization/personalize.md) para editar seu email conforme desejado. Salve o conteúdo.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->