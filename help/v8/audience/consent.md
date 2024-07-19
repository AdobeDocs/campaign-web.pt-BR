---
audience: end-user
title: Consentimento
description: Saiba mais sobre o consentimento no Adobe Campaign Web
badge: label="Disponibilidade limitada"
source-git-commit: 9a184d7558ca39be3afed4a7217a5e5687799c0d
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 13%

---

# Gerenciar o consentimento {#manage-consent}

## Recomendações gerais {#general-recommendations}

O Adobe Campaign permite coletar dados, inclusive informações pessoais e confidenciais. Portanto, é essencial obter e monitorar o consentimento de seus destinatários em conformidade com as regulamentações de proteção de dados, como o GDPR (Regulamento Geral sobre a Proteção de Dados) e outras leis de privacidade aplicáveis.

* Em primeiro lugar, evite enviar emails não solicitados, notificações por push e mensagens SMS (&quot;spam&quot;). A Adobe acredita fortemente nos princípios da permissão de marketing para promover a fidelidade e o valor vitalício do cliente e, portanto, é estritamente proibido o uso do Adobe Campaign para o envio de mensagens não solicitadas. [Saiba mais](#denylisted-profiles)

* Tenha sempre os destinatários concordando em receber comunicações fornecendo a capacidade de recusar suas entregas<!-- and keep honoring opt-out requests as quickly as possible-->. [Saiba mais](#opt-out)

* Por meio do processo de gerenciamento de assinaturas, você pode gerenciar suas preferências de recipient e rastrear quais recipients aceitaram e que tipo de assinatura. [Saiba mais](../../delivery/using/about-services-and-subscriptions.md)

## Gerenciar recusa {#opt-out}

Fornecer aos recipients a capacidade de cancelar a inscrição para receber comunicações de uma marca é um requisito legal, bem como garantir que essa escolha seja respeitada. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Por que é importante?**

* O não cumprimento desses regulamentos traz riscos legais normativos para sua marca.
* Ele ajuda a evitar o envio de comunicações não solicitadas para seus recipients, o que pode fazer com que eles marquem suas mensagens como spam e prejudiquem sua reputação.

Ao enviar deliveries usando a Adobe Campaign Web, você deve sempre garantir que os clientes possam cancelar a inscrição de comunicações futuras. Após o cancelamento da assinatura, os perfis serão removidos automaticamente do público-alvo de futuras mensagens de marketing.

### Recusa de email {#email-opt-out}

Para fornecer aos destinatários a capacidade de cancelar a inscrição e não receber notificações por email, você sempre deve incluir um **link para cancelar a inscrição** em cada email enviado aos destinatários.

Para fazer isso, siga as etapas abaixo.

1. Crie uma página de aterrissagem externa e hospede-a no sistema de terceiros de sua escolha.

1. Crie um delivery de email. [Saiba como](../email/create-email.md)

1. Insira um link para o seu conteúdo de email. [Saiba como](../email/message-tracking.md#insert-links)

   ![](../email/assets/message-tracking-insert-link.png)

1. No campo **[!UICONTROL Url]**, cole o link para a sua página de aterrissagem de terceiros.

1. Clique no ícone **[!UICONTROL Links]** no painel esquerdo para exibir a lista de todos os URLs do conteúdo a ser rastreado.

1. Clique no ícone de lápis ao lado do novo link para editá-lo.

1. Modifique o **[!UICONTROL Tipo de Rastreamento]** e defina-o como **[!UICONTROL Recusar]**.

   ![](../email/assets/message-tracking-edit-a-link.png)

1. Clique em **[!UICONTROL Salvar]** e envie a mensagem. [Saiba mais](../monitor/prepare-send.md)

1. Depois que a mensagem for recebida, se o recipient clicar no link de cancelamento de inscrição, a página de aterrissagem será exibida.

1. Quando o recipient envia o formulário de landing page, os dados do perfil são atualizados. [Saiba mais](#denylisted-profiles)

<!--Any other option availabe such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Incluir na lista de bloqueios perfis destacados {#denylisted-profiles}

Após o cancelamento de inscrição, os perfis ficam na **inclui na lista de bloqueios** de determinado canal: isso implica que eles não estão mais sendo direcionados por nenhuma entrega.

>[!NOTE]
>
>Incluir na lista de bloqueios Se um perfil na pesquisa do canal de email tiver dois endereços de email, ambos os endereços serão excluídos do delivery.

Incluir na lista de bloqueios Você pode verificar se um perfil está no arquivo de navegação para um ou mais canais na seção **[!UICONTROL Não contatar mais]** da guia **[!UICONTROL Detalhes]** do perfil. [Saiba mais](../audience/about-recipients.md#access)

![](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->



