---
audience: end-user
title: Consentimento
description: Saiba mais sobre o consentimento no Adobe Campaign Web
badge: label="Disponibilidade limitada"
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 8%

---

# Gerenciar o consentimento {#manage-consent}

## Recomendações gerais {#general-recommendations}

O Adobe Campaign permite coletar dados, inclusive informações pessoais e confidenciais. É essencial obter e monitorar o consentimento dos destinatários em conformidade com as regulamentações de proteção de dados, como o GDPR (Regulamento Geral sobre a Proteção de Dados) e outras leis de privacidade aplicáveis.

* Primeiro, evite enviar emails não solicitados, notificações por push e mensagens SMS (&quot;spam&quot;). A Adobe apoia fortemente os princípios da permissão de marketing para promover a fidelidade e o valor vitalício do cliente. O Adobe é estritamente proibido de usar o Adobe Campaign para enviar mensagens não solicitadas. [Saiba mais](#denylisted-profiles)

* Sempre verifique se os destinatários concordam em receber comunicações, fornecendo a capacidade de recusar suas entregas<!-- and keep honoring opt-out requests as quickly as possible-->. [Saiba mais](#opt-out)

* Use o processo de gerenciamento de assinaturas para gerenciar as preferências dos destinatários e rastrear quais destinatários aceitaram tipos específicos de assinaturas. [Saiba mais](../../delivery/using/about-services-and-subscriptions.md)

## Gerenciar recusa {#opt-out}

Oferecer aos recipients a capacidade de cancelar a inscrição para receber comunicações de uma marca é um requisito legal. É igualmente necessário garantir que esta escolha seja respeitada. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**Por que é importante?**

* O não cumprimento desses regulamentos traz riscos legais normativos para sua marca.
* Ajuda a evitar o envio de comunicações não solicitadas para os recipients, o que pode levá-los a marcar suas mensagens como spam e prejudicar sua reputação.

Ao enviar deliveries usando a Adobe Campaign Web, certifique-se de que os clientes possam cancelar a inscrição de comunicações futuras. Após o cancelamento da assinatura, os perfis serão removidos automaticamente do público-alvo de futuras mensagens de marketing.

### Recusa de email {#email-opt-out}

Para permitir que os destinatários cancelem a inscrição do recebimento de notificações por email, inclua um **link para cancelar a inscrição** em cada email enviado aos destinatários.

Siga estas etapas:

1. Crie uma página de aterrissagem externa e hospede-a no sistema de terceiros de sua escolha.

1. Crie um delivery de email. [Saiba como](../email/create-email.md)

1. Insira um link em seu conteúdo de email. [Saiba como](../email/message-tracking.md#insert-links)

   ![Inserir link no conteúdo do email](../email/assets/message-tracking-insert-link.png)

1. No campo **[!UICONTROL Url]**, cole o link para a sua página de aterrissagem de terceiros.

1. Clique no ícone **[!UICONTROL Links]** no painel esquerdo para exibir a lista de todas as URLs do seu conteúdo a serem rastreadas.

1. Clique no ícone de lápis ao lado do novo link para editá-lo.

1. Modifique o **[!UICONTROL Tipo de Rastreamento]** e defina-o como **[!UICONTROL Recusar]**.

   ![Editar tipo de rastreamento para recusa](../email/assets/message-tracking-edit-a-link.png)

1. Clique em **[!UICONTROL Salvar]** e envie a mensagem. [Saiba mais](../monitor/prepare-send.md)

1. Depois que a mensagem for recebida, se o recipient clicar no link de cancelamento de inscrição, a página de aterrissagem será exibida.

1. Quando o recipient envia o formulário de landing page, os dados do perfil são atualizados. [Saiba mais](#denylisted-profiles)

<!--Any other option available such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Incluir na lista de bloqueios perfis destacados {#denylisted-profiles}

Após o cancelamento de inscrição, os perfis são adicionados ao **incluo na lista de bloqueios** para um determinado canal. Isso significa que eles não serão mais direcionados por nenhum delivery.

>[!NOTE]
>
>Incluir na lista de bloqueios Se um perfil na pesquisa do canal de email tiver dois endereços de email, ambos os endereços serão excluídos do delivery.

Incluir na lista de bloqueios Você pode verificar se um perfil está no arquivo de navegação para um ou mais canais na seção **[!UICONTROL Não contatar mais]** da guia **[!UICONTROL Detalhes]** do perfil. [Saiba mais](../audience/about-recipients.md#access)

incluir na lista de bloqueios ![Verificar status da pesquisa em detalhes do perfil](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more about quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->