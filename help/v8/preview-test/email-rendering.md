---
audience: end-user
title: Testar a renderização do email
description: Saiba como testar a renderização do email na interface do Campaign Web
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
badge: label="Alpha" type="Positive"
source-git-commit: 6bd112c3ceb283435809379403c91ac9c8ed2756
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 9%

---


# Testar a renderização do email {#email-rendering}

Antes de enviar o email, verifique se a sua mensagem é exibida aos recipients de forma eficaz em uma variedade de clientes e dispositivos da Web.

Para fazer isso, você pode aproveitar os seus **Litmus** conta em [!DNL Adobe Campaign] para visualizar instantaneamente sua renderização de email em diferentes contextos e verificar a compatibilidade nos principais desktops e aplicativos (webmail, serviço de mensagens, dispositivos móveis etc.).

>[!CAUTION]
>
>Usar a renderização de email no Campaign envia um email de teste para um sistema de terceiros. Conectando sua conta Litmus ao [!DNL Campaign], você reconhece que o Adobe não é responsável por nenhum dado que possa ser enviado a esse terceiro. A política de retenção de dados Litmus se aplica a esses emails, incluindo dados de personalização que podem ser incluídos nessas mensagens de teste. Para acessar ou excluir esses dados, entre em contato diretamente com a Litmus.

Para acessar os recursos de renderização de email, é necessário:

* Ter uma conta Litmus
* Selecionar perfis de teste - Saiba mais em [nesta seção](preview-content.md)

Em seguida, siga as etapas abaixo.

1. No [Editar conteúdo](../content/edit-content.md) na tela ou no [Email Designer](../content/get-started-email-designer.md), clique no link **[!UICONTROL Simular conteúdo]** botão.

1. Selecione o **[!UICONTROL Renderizar email]** botão.

   ![](assets/simulate-rendering-button.png)

1. Clique em **Conectar sua conta Litmus** na seção superior direita.

   ![](assets/simulate-rendering-litmus.png)

1. Insira suas credenciais e faça logon.

   ![](assets/simulate-rendering-credentials.png)

1. Clique em **Executar teste** botão para gerar visualizações de email.

1. Verifique seu conteúdo de email em clientes populares de desktop, móveis e baseados na Web.

   ![](assets/simulate-rendering-previews.png)

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png)

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
