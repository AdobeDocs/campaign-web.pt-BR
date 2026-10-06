---
audience: end-user
title: Introdução a mensagens LINE
description: Saiba como criar e enviar mensagens LINE com a interface do usuário da Web do Adobe Campaign
feature: Line App
topic: Content Management
role: User
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
subfeature_v2:
  - id: d9d413df-4e9e-4906-bbbc-28c06c2ccf59
    internal-label: LINE App
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
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
