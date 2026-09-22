---
audience: end-user
title: Introdução a mensagens LINE
description: Saiba como criar e enviar mensagens LINE com a interface do usuário da Web do Adobe Campaign
feature: Line App
topic: Content Management
role: User
level: Beginner
source-git-commit: 1c4cdd5164d0cf572e9b88881bbe240b06308866
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 12%
---
# Introdução a mensagens LINE {#get-started-line}

O LINE é um aplicativo para mensagens instantâneas, chamadas de voz e vídeo gratuitas, disponível em todos os dispositivos móveis e para PC. Você pode usar o Adobe Campaign para enviar mensagens LINE. Use o LINE em deliveries independentes ou em workflows, junto com seus outros canais.

![Exemplo de mensagem LINE recebida em um dispositivo móvel](assets/line-message.png)

* **[!UICONTROL Entregas]**: crie uma entrega LINE autônoma a partir do menu **[!UICONTROL Entregas]** no painel esquerdo, semelhante a SMS ou push. [Saiba mais](send-line.md).

* **[!UICONTROL Fluxos de trabalho]**: na tela do fluxo de trabalho, adicione uma atividade de canal **[!UICONTROL LINE]**, escolha um modelo de entrega e defina o conteúdo e as configurações no painel de entrega. Saiba mais sobre as atividades de canal em [esta seção](../workflows/activities/channels.md).

  >[!NOTE]
  >
  >Na atividade **[!UICONTROL Criar público]** que alimenta sua atividade de canal **[!UICONTROL LINE]**, altere o targeting dimension para **[!UICONTROL Assinaturas de visitantes]**. Habilite **[!UICONTROL Mostrar todos os esquemas]** no painel lateral. O seletor de template do delivery só fica disponível depois que esse targeting dimension é definido.
