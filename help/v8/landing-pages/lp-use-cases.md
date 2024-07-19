---
solution: Campaign, Campaign v8 Web User Interface
title: Casos de uso da landing page
description: Descubra os casos de uso mais comuns com landing pages na interface da Web do Campaign
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: página de aterrissagem, caso de uso
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: e5a17ad1f8316d201dc3b4bc6ce20d61aea7a9c9
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 9%

---

# Como usar uma página de destino {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="Copie o URL com cuidado"
>abstract="Para testar ou aproveitar totalmente sua página de destino, você não deve copiar e colar o link diretamente em um navegador da web ou em suas entregas. Em vez disso, use a função **Simular conteúdo** para testá-lo e siga as etapas descritas na documentação para usar corretamente a sua página de destino."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="Copie o URL com cuidado"
>abstract="Ao criar uma página de destino, quatro modelos prontos para uso permitem implementar diferentes casos de uso: adicionar ou atualizar um perfil no banco de dados do Campaign, assinar um serviço para os clientes, cancelar a assinatura de um serviço ou recusar usuários."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html?lang=pt-BR#create-landing-page" text="Criar uma landing page"

Para usar adequadamente a landing page, você deve referenciá-la como um link em um delivery usando a opção dedicada.

>[!CAUTION]
>
>Para aproveitar totalmente a landing page, não é possível copiar e colar o link exibido no painel do delivery publicado diretamente nos seus deliveries ou em uma página da Web. Saiba como fazer isso corretamente nesta seção.

Na inferface [!DNL Adobe Campaign Web], quatro modelos prontos para uso permitem implementar casos de uso diferentes. No entanto, as etapas principais permanecem as mesmas e são detalhadas abaixo.

1. [Crie uma página de aterrissagem](create-lp.md#create-landing-page) e selecione o modelo de sua escolha, de acordo com seu caso de uso.

1. Defina as propriedades e as configurações da landing page.

   ![](assets/lp-uc-properties.png){zoomable="yes"}

1. De acordo com seu caso, selecione a página **[!UICONTROL Aquisição]**, **[!UICONTROL Assinatura]**, **[!UICONTROL Cancelar assinatura]** ou **[!UICONTROL Incluir na lista de bloqueios]**.

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de landing page.

   ![](assets/lp-uc-form.png){zoomable="yes"}

1. Edite o conteúdo de acordo com o template selecionado:

   * [Aquisição](#lp-acquisition)
   * [Assinatura](#lp-subscription)
   * [Cancelamento de assinatura](#lp-unsubscription)
   * [Lista de bloqueios](#lp-denylist)

1. Modifique o restante do conteúdo conforme necessário, salve as alterações e feche o.

1. Edite a página **[!UICONTROL Confirmação]** conforme necessário, bem como as páginas **[!UICONTROL Erro]** e **[!UICONTROL Expiração]**. A página **[!UICONTROL Confirmação]** será exibida para os destinatários assim que eles enviarem o formulário.

   ![](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [Testar](create-lp.md#test-landing-page) e [publicar](create-lp.md#publish-landing-page) sua landing page.

1. Crie uma entrega de [email](../email/create-email.md) para direcionar o tráfego para a página de aterrissagem.

1. [Insira um link](../email/message-tracking.md#insert-links) no conteúdo da mensagem. Selecione **[!UICONTROL Página de aterrissagem]** como o **[!UICONTROL Tipo de link]** e escolha a página de aterrissagem criada.

   ![](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >Para enviar a mensagem, verifique se a landing page selecionada ainda não expirou. [Saiba mais](create-lp.md#create-landing-page)

Depois que receberem o email, se os recipients clicarem no link para a landing page e enviarem o formulário:

* Eles serão direcionados para a página de confirmação.

* Qualquer outra ação definida na página de aterrissagem será aplicada. Por exemplo, os usuários serão inscritos em seu serviço ou não receberão mais comunicações de você.

Abaixo estão alguns exemplos de como você pode usar as páginas de aterrissagem do [!DNL Adobe Campaign] nos diferentes casos de uso possíveis.

## Aquisição de perfil {#lp-acquisition}

O primeiro template permite adicionar ou atualizar um perfil no banco de dados do Campaign.

1. Ao [criar sua página de aterrissagem](create-lp.md#create-landing-page), selecione o modelo **[!UICONTROL Aquisição]**.

1. Nas propriedades da página de aterrissagem, selecione a opção **[!UICONTROL Pre-fill with the data referenced in the form]** para pré-carregar qualquer informação existente do perfil e evitar a criação de duplicatas.

1. Selecione a página **[!UICONTROL Aquisição]** para editar seu conteúdo.

1. Edite os campos de texto conforme necessário, de acordo com as informações que deseja coletar em seus perfis.

1. Além disso, você pode adicionar uma caixa de seleção que convida os clientes a assinar o serviço de boletim informativo. [Saiba como criar um serviço](../audience/manage-services.md)

   ![](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. Ajuste o conteúdo conforme necessário e salve as alterações.

1. Revise e [publique](create-lp.md#publish-landing-page) sua landing page.

1. Crie um [email](../email/create-email.md) e [adicione um link](../email/message-tracking.md#insert-links) à sua página de aterrissagem.

Depois que eles receberem o email, se os recipients clicarem no link para a landing page e enviarem o formulário, o perfil deles será adicionado ao banco de dados do Campaign ou atualizado com as informações fornecidas.

![](assets/lp-uc-profile-updated.png){zoomable="yes"}

Se optarem por receber seu boletim informativo, serão inscritos no serviço correspondente.

![](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## Assinatura de um serviço {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="Definir a landing page da sua assinatura"
>abstract="Uma página de assinatura permite que seus clientes assinem um serviço."

Um dos casos de uso mais comuns consiste em convidar seus clientes a [assinar um serviço](../audience/manage-services.md) (como um boletim informativo ou um evento) por meio de uma página de aterrissagem. Siga as etapas abaixo.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Comece criando um template de confirmação para os usuários que assinam seu evento, para que você possa selecioná-lo facilmente ao criar o serviço. [Saiba mais](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. Crie um serviço de assinatura, que armazenará os usuários registrados em seu evento. [Saiba como criar um serviço](../audience/manage-services.md)

1. Selecione o template criado como o email de confirmação que os usuários receberão ao assinar.

   ![](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [Crie uma página de aterrissagem](create-lp.md#create-landing-page) para permitir que seus destinatários se registrem no evento. Selecione o modelo de **[!UICONTROL Assinatura]**.

1. Selecione a página **[!UICONTROL Assinatura]** para editar seu conteúdo.

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de página de aterrissagem e expanda a seção **[!UICONTROL Caixa de seleção 1]**.

1. No campo **[!UICONTROL Assinaturas e serviços]**, selecione o serviço criado para o evento. Deixe a opção **[!UICONTROL Assinar se marcada]** habilitada.

   ![](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Ajuste o conteúdo conforme necessário e salve as alterações.

1. Revise e [publique](create-lp.md#publish-landing-page) sua landing page.

1. Crie um [email](../email/create-email.md) e [adicione um link](../email/message-tracking.md#insert-links) para direcionar tráfego para a página de aterrissagem de registro.

1. Crie o email para anunciar que as inscrições para o seu evento estão abertas.

Depois que eles receberem o email, se seus recipients clicarem no link para a landing page e enviarem o formulário, eles serão direcionados à página de confirmação e adicionados à lista de subscrição.

## Cancelamento de assinatura {#lp-unsubscription}

Você pode permitir que seus clientes cancelem a assinatura de um serviço usando uma landing page.

1. Certifique-se de ter criado um modelo de confirmação para os usuários que cancelaram a assinatura do serviço, para que você possa selecioná-lo facilmente ao criar o serviço. [Saiba mais](../audience/manage-services.md#create-confirmation-message)

1. Em seu [serviço de assinatura](../audience/manage-services.md), selecione o modelo que você criou como o email de confirmação que os usuários receberão ao cancelar a assinatura.

1. [Criar uma página de aterrissagem](create-lp.md#create-landing-page). Selecione o modelo **[!UICONTROL Unsubscription]**.

1. Selecione a página **[!UICONTROL Cancelar assinatura]** para editar seu conteúdo.

1. O conteúdo da página é exibido. Selecione a parte correspondente ao formulário de landing page.

1. Você pode adicionar uma seção **[!UICONTROL Caixa de seleção]**, selecionar o serviço e a opção **[!UICONTROL Cancelar inscrição se marcada]**.

   ![](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. Você também pode expandir a seção **[!UICONTROL Chamada para ação]** e selecionar a opção **[!UICONTROL Atualizações adicionais]**. Selecione o serviço e marque a opção **[!UICONTROL Recusar]**.

   ![](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. Ajuste o conteúdo conforme necessário e salve as alterações.

1. Revise e [publique](create-lp.md#publish-landing-page) sua landing page.

1. Crie um [email](../email/create-email.md) e [adicione um link](../email/message-tracking.md#insert-links) à página de aterrissagem.

Depois que eles receberem o email, se os recipients clicarem no link para a landing page e enviarem o formulário, eles serão direcionados à página de confirmação do cancelamento de subscrição e serão removidos do serviço de subscrição correspondente.

## Lista de bloqueios {#lp-denylist}

Oferecer aos recipients a capacidade de cancelar a inscrição para receber comunicações de uma marca é um requisito legal. Portanto, você sempre deve incluir um **link para cancelar a inscrição** em cada email enviado aos recipients. Ao clicar nesse link, os recipients serão direcionados a uma página de aterrissagem que inclui um botão para confirmar a recusa.

Incluir na lista de bloqueios Você pode configurar uma **[!UICONTROL página de aterrissagem de]** que permitirá que os usuários recusem todas as entregas.

1. Ao [criar sua página de aterrissagem](create-lp.md#create-landing-page), selecione o **[!UICONTROL modelo de Inclui na lista de bloqueios]**.

1. Selecione a **[!UICONTROL página de Inclui na lista de bloqueios]** para editar seu conteúdo.

1. Expanda a seção **[!UICONTROL Chamada para ação]** e selecione a opção **[!UICONTROL Atualizações adicionais]**.

1. Na lista suspensa correspondente, selecione **[!UICONTROL Canal (email)]** para permitir que seus destinatários recusem apenas comunicações por email. Você também pode selecionar **[!UICONTROL Por todos os canais]** para escolher todos eles em todas as comunicações em todos os canais.

   ![](assets/lp-uc-denylist.png){zoomable="yes"}

1. Ajuste o conteúdo conforme necessário e salve as alterações.

1. Revise e [publique](create-lp.md#publish-landing-page) sua landing page.

1. Crie um [email](../email/create-email.md) e [adicione um link](../email/message-tracking.md#insert-links) à sua página de aterrissagem para permitir que os usuários recusem o recebimento de comunicações.

Depois que receberem o email, se os recipients clicarem no link para a landing page e enviarem o formulário, eles serão direcionados à página de confirmação do incluo na lista de bloqueios e seu perfil será atualizado com as informações fornecidas.

Para verificar se a escolha do perfil correspondente foi atualizada, navegue até o menu **[!UICONTROL Perfis]** e selecione esse perfil.

Por exemplo, se você optou por atualizar a opção **[!UICONTROL Canal (email)]** na página de aterrissagem, a opção **[!UICONTROL Não contatar mais por email]** será marcada.

![](assets/lp-uc-denylist-profile.png){zoomable="yes"}

Este perfil não receberá comunicações por email da sua marca, a menos que faça a assinatura novamente.
