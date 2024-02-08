---
solution: Journey Optimizer
product: journey optimizer
title: Casos de uso da landing page
description: Descubra os casos de uso mais comuns com landing pages no Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: página de aterrissagem, caso de uso
source-git-commit: 40c1ac49e9c297e0431331df612cc4a1ae804723
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# Como usar uma landing page {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copie o URL com cuidado"
>abstract="Para testar ou aproveitar totalmente a landing page, não é possível copiar e colar esse link diretamente em um navegador da Web ou em seus deliveries. Use o botão **Simular conteúdo** para testá-la e siga as etapas descritas na documentação para usar corretamente a landing page."

Para usar adequadamente a landing page, você deve referenciá-la como um link em um delivery usando a opção dedicada.

>[!CAUTION]
>
>Para aproveitar totalmente a landing page, não é possível copiar e colar o link exibido no painel do delivery publicado diretamente nos seus deliveries ou em uma página da Web.

No [!DNL Adobe Campaign Web] inferface, quatro templates prontos para uso permitem implementar casos de uso diferentes. No entanto, as etapas principais permanecem as mesmas e são detalhadas abaixo.

1. [Criar uma landing page](create-lp.md#create-landing-page) e selecione o template de sua escolha, de acordo com seu caso de uso:

   * [Aquisição](#lp-acquisition)
   * [Assinatura](#lp-subscription)
   * [Cancelamento de assinatura](#lp-unsubscription)
   * [Lista de bloqueios](#lp-denylist)

1. Defina as propriedades e as configurações da landing page.

   ![](assets/lp-uc-properties.png)

1. De acordo com seu caso, selecione o **[!UICONTROL Aquisição]**, **[!UICONTROL Inscrição]**, **[!UICONTROL Cancelar assinatura]** ou **[!UICONTROL ➡ Incluir na lista de bloqueios]** página.

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de landing page.

   ![](assets/lp-uc-form.png)

1. Faça quantas atualizações nos rótulos e campos da landing page forem necessárias. Edite o resto do conteúdo como quiser, salve as alterações e feche.

1. Siga as etapas detalhadas abaixo para cada caso de uso.

1. Edite o **[!UICONTROL Confirmação]** conforme necessário, bem como a **[!UICONTROL Erro]** e **[!UICONTROL Expiração]** páginas. Ele será exibido aos recipients assim que eles enviarem o formulário de registro.

   ![](assets/lp-uc-confirmation-page.png)

1. Teste e [publicar](create-lp.md#publish-landing-page) sua landing page.

1. Criar um [email](../email/create-email.md) delivery para direcionar o tráfego para a landing page.

1. [Inserir um link](../email/message-tracking.md#insert-links) no conteúdo da mensagem. Selecionar **[!UICONTROL Landing page]** como o **[!UICONTROL Tipo de link]** e escolha o [landing page](create-lp.md#configure-primary-page) criado.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Para enviar a mensagem, verifique se a landing page selecionada ainda não expirou. Saiba como atualizar a data de expiração [nesta seção](create-lp.md#create-landing-page).

Depois que eles receberem o email, se os recipients clicarem no link para a landing page e enviarem o formulário da landing page, eles serão direcionados à página de confirmação e qualquer outra ação definida na landing page será aplicada (por exemplo, os usuários assinarão seu serviço ou não receberão mais comunicações sua).

Abaixo estão alguns exemplos de como você pode usar [!DNL Adobe Campaign] landing pages para que seus clientes optem por receber algumas ou todas as suas comunicações.

## Aquisição de perfil {#lp-acquisition}

1. [Criar uma landing page](create-lp.md#create-landing-page). Selecione o **[!UICONTROL Aquisição]** modelo.

1. Defina as propriedades e as configurações da landing page.

   ![](assets/lp-uc-properties.png)

1. Selecione o **[!UICONTROL Aquisição]** para editar seu conteúdo.

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de landing page.

## Assinatura de um serviço {#lp-subscription}

Um dos casos de uso mais comuns consiste em convidar seus clientes para [assinar um serviço](../audience/manage-services.md) (como um boletim informativo ou um evento) por meio de uma landing page. Siga as etapas abaixo.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Comece criando um template de confirmação para os usuários que assinam seu evento, para que você possa selecioná-lo facilmente ao criar o serviço. [Saiba mais](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. Crie um serviço de assinatura, que armazenará os usuários registrados em seu evento. [Saiba como criar um serviço](../audience/manage-services.md)

1. Selecione o template criado como o email de confirmação que os usuários receberão ao assinar.

   ![](assets/lp-uc-subscription-service.png)

1. [Criar uma landing page](create-lp.md#create-landing-page) para permitir que seus destinatários se registrem no evento. Selecione o **[!UICONTROL Inscrição]** modelo.

   <!--![](assets/lp-uc-subscription-template.png)-->

1. Defina as propriedades e as configurações da landing page.

   <!--![](assets/lp-uc-properties.png)-->

1. Selecione o **[!UICONTROL Inscrição]** para editar seu conteúdo.

   ![](assets/lp-uc-subscription-page-edit.png)

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de landing page e expanda a **[!UICONTROL Caixa de seleção 1]** seção.

   No **[!UICONTROL Assinaturas e serviços]** selecione o serviço criado para o evento. Deixe a **[!UICONTROL Inscrever se marcado]** opção ativada.

   ![](assets/lp-uc-subscription-checkbox-1.png)

1. Você pode adicionar uma caixa de seleção extra para oferecer a subscrição ao seu boletim informativo, por exemplo.

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. Faça quantas atualizações nos rótulos e campos da landing page forem necessárias. Edite o resto do conteúdo como quiser, salve as alterações e feche.

1. Edite o **[!UICONTROL Confirmação]** conforme necessário, bem como a **[!UICONTROL Erro]** e **[!UICONTROL Expiração]** páginas. Ele será exibido aos recipients assim que eles enviarem o formulário de registro.

   ![](assets/lp-uc-confirmation-page.png)

1. Teste e [publicar](create-lp.md#publish-landing-page) sua landing page.

1. Criar um **E-mail** delivery para direcionar o tráfego para a landing page de registro. Crie o email para anunciar que as inscrições para o seu evento estão abertas.

1. [Inserir um link](../email/message-tracking.md#insert-links) no conteúdo da mensagem. Selecionar **[!UICONTROL Landing page]** como o **[!UICONTROL Tipo de link]** e escolha o [landing page](create-lp.md#configure-primary-page) que você criou para registro.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Para enviar a mensagem, verifique se a landing page selecionada ainda não expirou. Saiba como atualizar a data de expiração [nesta seção](create-lp.md#create-landing-page).

Depois que eles receberem o email, se seus recipients clicarem no link para a landing page e enviarem o formulário da landing page, eles serão direcionados à página de confirmação e adicionados à lista de subscrição.

## Cancelamento de assinatura {#lp-unsubscription}

1. [Criar uma landing page](create-lp.md#create-landing-page). Selecione o **[!UICONTROL Cancelar assinatura]** modelo.

1. Defina as propriedades e as configurações da landing page.

1. Selecione o **[!UICONTROL Cancelar assinatura]** para editar seu conteúdo.

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de landing page.

## Configuração de páginas de aterrissagem de recusa {#lp-denylist}

Oferecer aos recipients a capacidade de cancelar a inscrição para receber comunicações de uma marca é um requisito legal. Saiba mais sobre a legislação aplicável na [Documentação do Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html#regulations){target="_blank"}.

Portanto, você sempre deve incluir um **link para cancelar inscrição** em cada email enviado aos recipients:

* Ao clicar nesse link, os recipients serão direcionados a uma página de aterrissagem que inclui um botão para confirmar a recusa.
* Ao clicar no botão de recusa, os dados do perfil serão atualizados com essas informações.

Você pode configurar um **[!UICONTROL ➡ Incluir na lista de bloqueios]** página de aterrissagem que permitirá que os usuários recusem todos os deliveries.

Para permitir que os usuários recusem todos os deliveries, é necessário criar e publicar um **[!UICONTROL ➡ Incluir na lista de bloqueios]** página de aterrissagem.

Quando um usuário clica no link da página de aterrissagem, a variável **[!UICONTROL Não entrar mais em contato (por qualquer canal)]** no perfil é selecionada automaticamente.

definir um **[!UICONTROL Opção de não participação]** e optar por atualizar **[!UICONTROL Canal (email)]**: o perfil que marca a caixa de opção de não participação na página de aterrissagem será excluído de todas as suas comunicações.

Depois que a mensagem for recebida, se um recipient clicar no link de cancelamento de inscrição no email, a página de aterrissagem será exibida.

![](assets/lp_opt-out-submit-form.png)

Se o recipient marcar a caixa e enviar o formulário:

* O recipient que recusou a inscrição é redirecionado para a tela de mensagem de confirmação.

* Os dados do perfil são atualizados e não receberão comunicações de sua marca, a menos que você faça a assinatura novamente.

Para verificar se a escolha do perfil correspondente foi atualizada, vá para Profiles e selecione o perfil.







