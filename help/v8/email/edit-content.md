---
audience: end-user
title: Edição do conteúdo de email
description: Saiba como editar o conteúdo de email na interface da Web do Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: 498162045a2a58a5326a3cf311a153cf9dfef5c3
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 19%

---

# Configurar conteúdo de email {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definir o conteúdo do email"
>abstract="A tela **Editar conteúdo** permite definir elementos básicos da mensagem, como o endereço do remetente e a linha de assunto, executar ações adicionais, como adicionar anexos ou ofertas, e acessar o Designer de email para dar uma aparência mais elegante à mensagem."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Defina as propriedades de email"
>abstract="A seção **Detalhes básicos** permite atualizar o endereço do remetente e o endereço de resposta, bem como definir a linha de assunto, usando o Editor de expressões."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Anexar arquivos a um email"
>abstract="Selecione um ou vários arquivos para inserir na mensagem. Para evitar problemas de desempenho, é recomendável não incluir mais de um anexo por email."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Rastreamento de edições"
>abstract="Por padrão, o rastreamento é habilitado para a entrega, o que significa que todos os links incluídos no conteúdo da mensagem são rastreados. Você pode desabilitar essa opção aqui."
>additional-url="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Adicionar links e rastrear mensagens"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Adicionar idiomas"
>abstract="Nesta guia, você encontrará uma lista de idiomas nos quais o delivery será enviado. Você pode adicionar mais idiomas clicando no botão Adicionar idioma ou duplicando outro idioma por meio dessa guia."

A tela de email **[!UICONTROL Editar conteúdo]** permite:

* Defina elementos básicos da mensagem, como o endereço do remetente e a linha de assunto.
* Executar ações adicionais, como adicionar anexos ou configurar ofertas.
* Acesse o [Designer de email](get-started-email-designer.md#start-authoring) para começar a criar o conteúdo adequado de seu email.

>[!NOTE]
>
>Todos os campos de texto editáveis dessa tela podem ser preenchidos usando campos de personalização. [Saiba como personalizar conteúdo](../personalization/personalize.md)

Para configurar ou editar o conteúdo de um email, siga as etapas abaixo.

1. Clique no botão **[!UICONTROL Editar conteúdo]** da tela [painel de entrega de email](../email/create-email.md).

   ![Captura de tela mostrando o botão Editar conteúdo no painel de entrega de email.](assets/email-edit-content-button.png){zoomable="yes"}

1. A tela de edição de conteúdo de email é aberta.

   ![Captura de tela mostrando o painel de edição de conteúdo de email.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se você estiver configurando um novo email, os campos **[!UICONTROL De nome]** e **[!UICONTROL De email]** já estarão preenchidos.

1. O campo **[!UICONTROL De nome]** está definido no modelo de email. Se quiser modificá-lo, use um nome facilmente identificável pelos recipients, como o nome da sua marca, para aumentar a taxa de abertura dos deliveries.

   >[!NOTE]
   >
   >Para melhorar ainda mais a experiência do recipient, você pode adicionar o nome de uma pessoa, por exemplo, &quot;Eve da Luma&quot;.

1. O campo de endereço **[!UICONTROL Do email]** também é definido no modelo de email. Verifique se o domínio de endereço corresponde ao subdomínio que você delegou à Adobe.

   >[!NOTE]
   >
   >Você pode alterar a parte anterior a &#39;@&#39;, mas não o endereço do domínio.

1. Expanda a seção **[!UICONTROL Responder para campos]**. O nome e os endereços do remetente são usados por padrão para respostas. No entanto, a Adobe recomenda o uso de um endereço real, como o atendimento ao cliente da sua marca. Nesse caso, se um recipient enviar uma resposta, a equipe de atendimento ao cliente poderá resolvê-lo.

   ![Captura de tela mostrando a seção Responder para campos no editor de conteúdo de email.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Defina a **[!UICONTROL Linha de assunto]** do email. Digite o assunto diretamente no campo dedicado ou abra o Editor de Expressão para adicionar a [personalização](../personalization/personalize.md) usando vários atributos, fragmentos de expressão ou ofertas.

1. Para anexar um arquivo ao email, clique no botão **[!UICONTROL Adicionar anexo]** e selecione um ou vários arquivos.

   >[!NOTE]
   >
   >Para evitar problemas de desempenho, é recomendável não incluir mais de um anexo por email.

   <!--limitation on size + number of files?-->

1. Para enviar ofertas com seu email, selecione-as usando o botão **[!UICONTROL Configurar ofertas]**.

   Você pode inseri-los no email usando campos de personalização. [Saiba como enviar ofertas](../msg/offers.md)

1. Clique no botão **[!UICONTROL Editar corpo do email]** para estruturar e projetar o conteúdo do email usando o [Designer de email](get-started-email-designer.md#start-authoring). Informações adicionais sobre como projetar conteúdo de email estão disponíveis nestas seções:

   * [Criar emails do zero](create-email-content.md)
   * [Estilizar o conteúdo](get-started-email-style.md)

   >[!NOTE]
   >
   >Você também pode passar o mouse sobre a visualização do email e selecionar **[!UICONTROL Abrir designer de email]**.

1. Por padrão, o rastreamento é ativado para a entrega. Você pode desabilitar essa opção na seção **[!UICONTROL Recursos opcionais]**. [Saiba como adicionar links e gerenciar o rastreamento](message-tracking.md).

1. Depois que o conteúdo do email tiver sido definido, use o botão **[!UICONTROL Simular conteúdo]** para verificar como ele é exibido antes de enviá-lo. [Saiba como visualizar e testar seu email](../preview-test/preview-test.md).