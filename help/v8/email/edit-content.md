---
audience: end-user
title: Edição do conteúdo de email
description: Saiba como editar o conteúdo de email na interface da Web do Campaign
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: df5883f8178bc5287145c587b06dd5664400ed90
workflow-type: tm+mt
source-wordcount: '1229'
ht-degree: 24%

---

# Configurar conteúdo de email {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Definir o conteúdo do email"
>abstract="A tela **Editar conteúdo** permite definir os elementos básicos da mensagem, como o endereço do remetente e o assunto, realizar ações adicionais, como adicionar anexos ou ofertas, e acessar o Designer de email para deixar a mensagem com uma aparência elegante."

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
>abstract="Nesta guia, você encontrará uma lista de idiomas para o envio da entrega. É possível adicionar mais idiomas clicando no botão Adicionar idioma ou duplicando outro idioma por meio dessa guia."

A tela de email **[!UICONTROL Editar conteúdo]** permite:

* Definir elementos básicos da mensagem, como o endereço do remetente e a linha de assunto
* Executar ações adicionais, como adicionar anexos ou configurar ofertas
* Acesse o [Designer de email](get-started-email-designer.md#start-authoring) para começar a criar o conteúdo adequado do seu email
* Adicione variantes de idioma aos deliveries.

>[!NOTE]
>
>Todos os campos de texto editáveis dessa tela podem ser preenchidos usando campos de personalização. [Saiba como personalizar conteúdo](../personalization/personalize.md)

## Configurar o delivery

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

## Editar o corpo do email

1. Clique no botão **[!UICONTROL Editar corpo do email]** para estruturar e projetar o conteúdo do email usando o [Designer de email](get-started-email-designer.md#start-authoring).

   >[!NOTE]
   >
   >Você também pode passar o mouse sobre a visualização do email e selecionar **[!UICONTROL Abrir designer de email]**.


   Informações adicionais sobre como criar conteúdo de email estão disponíveis nessas seções:

   * [Criar emails do zero](create-email-content.md)
   * [Estilizar o conteúdo](get-started-email-style.md)

1. Por padrão, o rastreamento é ativado para a entrega. Você pode desabilitar essa opção na seção **[!UICONTROL Recursos opcionais]**. [Saiba como adicionar links e gerenciar o rastreamento](message-tracking.md)

1. Depois que o conteúdo do email tiver sido definido, use o botão **[!UICONTROL Simular conteúdo]** para verificar como ele é exibido antes de enviá-lo. [Saiba como visualizar e testar seu email](../preview-test/preview-test.md).

## Configurar um delivery multilíngue

Na interface do usuário da Web do Campaign, você pode configurar seus deliveries de email como multilíngues, o que permite enviar mensagens com base no idioma preferencial de um perfil. Quando nenhuma preferência é definida, a mensagem é enviada no idioma padrão.

Em um delivery multilíngue, o gerenciamento de idiomas é baseado em variantes. Cada variante representa um idioma.

Durante a criação do delivery, é possível adicionar o número de variantes correspondentes ao número de idiomas necessários na mensagem. Você também pode definir o idioma padrão ao adicionar novos idiomas.

### Adicionar uma variante de idioma

Para criar variantes de idioma, siga estas etapas:

1. Clique no botão **[!UICONTROL Adicionar idioma]** na seção superior da tela de configuração de email.

   >[!IMPORTANT]
   >
   >O botão **[!UICONTROL Adicionar idioma]** só estará disponível se a dimensão de destino contiver o esquema Idioma. Para saber mais sobre esquemas e dimensões do Target, consulte a [documentação detalhada](https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/audiences/targeting-dimensions){target=_blank}.

   ![](assets/edit-content_2.png){zoomable="yes"}


1. Selecione o idioma a ser adicionado na lista suspensa **[!UICONTROL Idioma]**. Ao adicionar o primeiro idioma, ele é definido como padrão e o conteúdo atual é o padrão. Ao adicionar novos idiomas, o conteúdo é baseado no conteúdo padrão.

   >[!NOTE]
   >
   >Os idiomas disponíveis nessa lista dependem dos valores que foram definidos pelo atributo Language (valores como: sistema, usuário, dbenum etc.) Saiba mais sobre o gerenciamento de enumeração nesta [seção](https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/conf/enumerations){target=_blank}.


   ![](assets/edit-content_3.png){zoomable="yes"}

   Por exemplo, aqui, para inglês (EUA):

   ![](assets/edit-content_8.png){zoomable="yes"}


1. Repita esse processo para adicionar outros idiomas. O painel **[!UICONTROL Idioma]** mostra a lista de idiomas escolhidos, o número de idiomas diferentes e também o idioma padrão.

   Por exemplo, se você tiver escolhido inglês, francês e sueco, poderá ver esses três idiomas conforme mostrado abaixo:

   ![](assets/edit-content_9.png){zoomable="yes"}

   Você pode clicar no botão expandir no canto superior direito para excluir todos os idiomas.

### Definir o conteúdo de email para cada variante

Depois que os idiomas forem definidos, defina o conteúdo do email que será enviado aos perfis com esse idioma preferencial.

Para definir um conteúdo de email, siga estas etapas:

1. Abra o [Designer de email](get-started-email-designer.md#start-authoring) clicando no botão **[!UICONTROL Editar corpo do email]**.

   >[!NOTE]
   >
   >Você também pode passar o mouse sobre a visualização do email e selecionar **[!UICONTROL Abrir designer de email]**.

   ![](assets/edit-content_11.png){zoomable="yes"}


1. Você pode visualizar o delivery clicando no botão **[!UICONTROL Simular conteúdo]** e escolher o perfil e o idioma no qual o email será exibido.

1. Na janela Simular conteúdo, é possível alternar perfis para visualizar o conteúdo do email correspondente ao idioma configurado para esse perfil.

   ![](assets/edit-content_5.png){zoomable="yes"}

### Duplicar ou remover variantes de idioma

Você pode clicar no botão expandir no canto superior direito e clicar no botão **[!UICONTROL Excluir todas as variantes]** para excluir todos os idiomas.

![](assets/edit-content_13.png){zoomable="yes"}

Para remover uma variante de idioma, clique nos três pontos no lado direito da guia e selecione Remover.

Para duplicar uma variante de idioma, clique nos três pontos no lado direito da guia e selecione Duplicar. Se você optar por duplicar um idioma diferente do padrão, o conteúdo duplicado será baseado no idioma escolhido para duplicação.


1. Depois que o conteúdo do email tiver sido definido, use o botão **[!UICONTROL Simular conteúdo]** para verificar como ele é exibido antes de enviá-lo. [Saiba como visualizar e testar seu email](../preview-test/preview-test.md).