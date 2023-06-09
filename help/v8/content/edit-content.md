---
audience: end-user
title: Editar o conteúdo do email
description: Saiba como editar o conteúdo de email na interface do Campaign Web
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
badge: label="Alpha" type="Positive"
source-git-commit: 3aee085da2031a497469fa826bbca3498d3dd0aa
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 43%

---

# Configurar o conteúdo do email {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Criar conteúdo de email"
>abstract="Com esta seção, você pode criar o conteúdo do seu email e usar o Designer de email para dar a ele uma aparência refinada."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="Parâmetros de email"
>abstract="Os valores de From name e From email são definidos no template de email. A linha de Assunto pode ser personalizada usando o Editor de expressão."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Anexo de email"
>abstract="Selecione um ou vários arquivos para inserir na mensagem."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Opções de rastreamento"
>abstract="Por padrão, o rastreamento é ativado para a entrega. Você pode desativar esta opção aqui."

O email **[!UICONTROL Editar conteúdo]** permite:
* Definir elementos básicos da mensagem, como o endereço do remetente e a linha de assunto
* Executar ações adicionais, como adicionar anexos ou configurar ofertas
* Acesse o [Email Designer](get-started-email-designer.md#start-authoring) para começar a criar o conteúdo adequado do seu email

Para configurar ou editar o conteúdo de um email, siga as etapas abaixo.

1. Clique em **[!UICONTROL Editar conteúdo]** botão no [painel de delivery de email](../email/create-email.md) tela.

   ![](assets/email-edit-content-button.png)

1. A tela de edição de conteúdo de email é aberta.

   ![](assets/email-edit-content-dashboard.png)

   >[!NOTE]
   >
   >Se estiver configurando um novo email, a variável **[!UICONTROL Do nome]** e **[!UICONTROL Do email]** já estão preenchidos.

1. A variável **[!UICONTROL Do nome]** é definido no template de email. Se quiser modificá-lo, use um nome facilmente identificável pelos recipients, como o nome da sua marca, para aumentar a taxa de abertura dos deliveries.

   >[!NOTE]
   >
   >Para melhorar ainda mais a experiência do recipient, você pode adicionar o nome de uma pessoa, por exemplo &quot;Eve da Luma&quot;.

1. A variável **[!UICONTROL Do email]** O campo de endereço também é definido no template de email. Verifique se o domínio de endereço é o mesmo que o subdomínio que você delegou ao Adobe.

   >[!NOTE]
   >
   >Você pode alterar a parte anterior a &#39;@&#39;, mas não o endereço do domínio.

   <!--In the Reply address text fields, the sender's address is used by default for replies. However, Adobe recommends using an existing real address such as your brand's customer care. In this case, if a recipient sends a reply, the customer care will be able to handle it.-->

1. Defina a **[!UICONTROL Linha de assunto]** do email. Digite o assunto diretamente no campo dedicado ou abra o Editor de expressão para adicionar personalização usando vários atributos e blocos de conteúdo ou ofertas. [Saiba como personalizar conteúdo](../personalization/personalize.md)

1. Se quiser anexar um arquivo ao email, clique no botão **[!UICONTROL Adicionar anexo]** e, em seguida, selecione um ou vários arquivos.

   >[!NOTE]
   >
   >    Para evitar problemas de desempenho, é recomendável não incluir mais de um anexo por email.

   <!--limitation on size + number of files?-->

1. Se desejar enviar ofertas com seu email, selecione-as usando o botão **[!UICONTROL Configurar ofertas.]**

   É possível inseri-los no email usando os campos de personalização. [Saiba como enviar ofertas](offers.md)

1. Clique em **[!UICONTROL Editar corpo do email]** botão para estruturar e projetar o conteúdo do email usando o [Email Designer](#start-authoring). Informações adicionais sobre como criar conteúdo de email estão disponíveis nessas seções:

   * [Criar emails do zero](create-email-content.md)
   * [Estilo do conteúdo](get-started-email-style.md)

   >[!NOTE]
   >
   >Você também pode passar o mouse sobre a pré-visualização do email e selecionar **[!UICONTROL Abrir designer de email]**.

1. Por padrão, o rastreamento é ativado para a entrega. Você pode desativar essa opção na seção **[!UICONTROL Recursos opcionais]**. [Saiba como adicionar links e gerenciar o rastreamento](message-tracking.md)

1. Depois que o conteúdo do email tiver sido definido, use o botão **[!UICONTROL Simular conteúdo]** para verificar como ele é exibido antes de enviá-lo. [Saiba como visualizar e testar seu email](../preview-test/preview-test.md)

