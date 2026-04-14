---
audience: end-user
title: Introdução a mensagens do WhatsApp
description: Saiba como criar e enviar mensagens do WhatsApp com a interface da Web do Adobe Campaign
feature: Whatsapp
topic: Content Management
role: User
level: Beginner
hide: true
source-git-commit: f0c22710efcda2f59f75ea26cf239d549ff34f96
workflow-type: tm+mt
source-wordcount: '210'
ht-degree: 1%

---

# Introdução a mensagens do WhatsApp {#get-started-whatsapp}

Você pode enviar mensagens do WhatsApp da **interface da Web do Adobe Campaign** usando a [API da nuvem](https://developers.facebook.com/docs/whatsapp/cloud-api/) da Meta. Use o WhatsApp em deliveries independentes, em workflows de campanha ou em campanhas de marketing internas, junto com seus outros canais.

* **[!UICONTROL Entregas]**: na interface da Web do Adobe Campaign, crie uma entrega autônoma do WhatsApp no menu **[!UICONTROL Entregas]** no painel esquerdo, de modo semelhante a SMS ou push. [Saiba mais](create-whatsapp.md).

* **[!UICONTROL Campanhas]**: na interface da Web do Adobe Campaign, abra uma campanha e adicione uma entrega via WhatsApp pela guia **[!UICONTROL Entregas]** ou orquestre envios com um fluxo de trabalho anexado à campanha. [Saiba mais](../campaigns/create-campaigns.md).

* **[!UICONTROL Fluxos de trabalho]**: na tela de fluxo de trabalho da interface Web do Adobe Campaign, adicione uma atividade de canal do **[!UICONTROL WhatsApp]**, escolha um modelo de entrega e defina o conteúdo e as configurações no painel de entrega. Saiba mais sobre as atividades de canal em [esta seção](../workflows/activities/channels.md).

## Pré-requisitos {#prereq}

Integrar WhatsApp requer o seguinte:

* Conta do Meta Business Manager
* [Conta Comercial do WhatsApp com nome de remetente e número de telefone verificados](https://developers.facebook.com/docs/whatsapp/overview/business-accounts/)
* [Token de autorização do usuário com permissões apropriadas](https://developers.facebook.com/blog/post/2022/12/05/auth-tokens/)
* [Modelos do Meta aprovados](https://developers.facebook.com/docs/whatsapp/message-templates/guidelines/)

Você também precisa confirmar o seguinte antes de continuar:

* [Regras de conteúdo do WhatsApp](https://www.whatsapp.com/legal/messaging-guidelines)
* [Conformidade com as políticas da Meta](https://www.whatsapp.com/legal)
* [Limites de conversa de 24 horas](https://developers.facebook.com/docs/whatsapp/messaging-limits/)


