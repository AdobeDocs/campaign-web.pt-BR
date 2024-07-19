---
audience: end-user
title: Testar a renderização do email
description: Saiba como testar a renderização de email na interface da Web do Campaign
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 3%

---


# Testar a renderização do email {#email-rendering}

Antes de enviar o email, verifique se a sua mensagem é exibida aos recipients de forma eficaz em uma variedade de clientes e dispositivos da Web.

Para fazer isso, você pode aproveitar sua conta do **Litmus** no [!DNL Adobe Campaign] para visualizar instantaneamente sua renderização de email em diferentes contextos e verificar a compatibilidade nos principais desktops e aplicativos (webmail, serviço de mensagens, celular etc.).

>[!CAUTION]
>
>Usar a renderização de email no Campaign envia uma prova para um sistema de terceiros. Ao conectar sua conta Litmus com [!DNL Campaign], você reconhece que o Adobe não é responsável por nenhum dado que possa ser enviado a terceiros. A política de retenção de dados Litmus se aplica a esses emails, incluindo dados de personalização que podem ser incluídos nessas provas. Para acessar ou excluir esses dados, entre em contato diretamente com a Litmus.

Para acessar os recursos de renderização de email, é necessário:

* Ter uma conta Litmus
* Selecionar perfis e/ou perfis de teste - Saiba mais em [esta seção](preview-content.md)

Em seguida, siga as etapas abaixo.

1. Na tela [Editar conteúdo](../email/edit-content.md) ou no [Designer de email](../email/get-started-email-designer.md), clique no botão **[!UICONTROL Simular conteúdo]**.

1. Selecione o botão **[!UICONTROL Renderizar email]**.

   ![](assets/simulate-rendering-button.png){zoomable="yes"}

1. Clique em **Conectar sua conta Litmus** na seção superior direita.

   ![](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. Insira suas credenciais e faça logon.

   ![](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. Clique no botão **Executar teste** para gerar visualizações de email.

1. Verifique seu conteúdo de email em clientes populares de desktop, móveis e baseados na Web.

   ![](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
