---
audience: end-user
title: Introdução a mensagens e entregas no Campaign Web v8
description: Saiba como trabalhar com entregas e enviar mensagens usando o Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 38%

---

# Introdução a mensagens no Campaign Web {#gs-messages}

Com o Adobe Campaign, você pode enviar campanhas entre canais, incluindo emails, SMS e notificações por push, e medir sua eficácia usando vários relatórios dedicados. Essas mensagens são projetadas e enviadas por deliveries, além disso podem ser personalizadas para cada recipient. Esses deliveries podem ser independentes ou incluídos no contexto de uma campanha de marketing.

O Adobe Campaign v8 vem com os seguintes canais de entrega:

* **Canal de email**: entregas de email permitem enviar emails personalizados para a população do target. Saiba como criar e enviar um email no [esta página](../email/create-email.md).

* **Canal SMS**: deliveries em canais móveis permitem enviar SMS personalizado para a população do target.  Saiba como criar e enviar SMS no [esta página](../sms/create-sms.md).

* **Canal de aplicativo móvel**: as entregas por aplicativo móvel permitem enviar as notificações para sistemas iOS e Android.  Saiba como criar e enviar notificações por push no [esta página](../push/gs-push.md).

## Criar um delivery

Você pode criar deliveries independentes a partir do **Entrega** ou crie deliveries no contexto de uma campanha de marketing.

>[!BEGINTABS]

>[!TAB Criar um delivery independente]

Para criar um delivery independente, siga estas etapas:

1. Navegue até o **[!UICONTROL Entregas]** no menu de navegação esquerdo e clique no botão **[!UICONTROL Criar entrega]** botão.
1. Escolha um canal para a entrega. Saiba mais sobre canais de entrega e como definir um conteúdo de entrega nestas seções:

   * [Canal de email](../email/create-email.md)
   * [Canal de notificação por push](../push/gs-push.md)
   * [Canal de SMS](../sms/create-sms.md)

1. Defina o público do delivery para o target principal e o grupo de controle. Saiba mais sobre públicos-alvo na [nesta seção](../audience/about-audiences.md).
1. Definir o conteúdo da mensagem.
1. (opcional) Defina a programação de delivery. Se nenhuma programação for definida, as mensagens serão enviadas imediatamente após clicar no **[!UICONTROL Enviar]** botão.
1. Clique em  **[!UICONTROL Revisar e enviar]** botão para verificar suas configurações.
1. Use o  **[!UICONTROL Simular conteúdo]** botão para testar o delivery e as configurações de personalização. Saiba mais sobre a simulação de mensagens em [nesta seção](../preview-test/preview-test.md).
1. Clique em  **[!UICONTROL Preparar]** botão para calcular a população do target e gerar as mensagens. A etapa de preparação pode levar alguns minutos. Quando a preparação estiver concluída, as mensagens estarão prontas para envio. Em caso de erro, navegue até a janela **Logs** para verificar alertas e avisos.
1. Verifique os resultados e clique no botão  **[!UICONTROL Enviar]** botão para iniciar o envio de mensagens.
1. Depois que as mensagens forem enviadas, navegue até a seção Relatórios para acessar as métricas principais. Saiba mais sobre relatórios de entrega em [nesta seção](../reporting/reports.md).

>[!TAB Criar um delivery em uma campanha]

Para criar um delivery em uma campanha, siga estas etapas:

1. Crie uma campanha ou abra uma campanha existente.

Para obter mais informações sobre como configurar uma campanha,

>[!ENDTABS]


## Escolha como enviar suas mensagens{#gs-send-msg}

Depois que a mensagem for criada e o conteúdo testado, você poderá escolher como deseja enviá-la.

O Campaign oferece um conjunto de recursos para:

* Enviar mensagens manualmente para o target principal

* Enviar mensagens associadas a uma [campanha de marketing](../campaigns/gs-campaigns.md)

* Enviar mensagens por meio de um [fluxo de trabalho](../workflows/channel-activities.md)


## Adicionar personalização{#personalization}

As mensagens entregues pelo Adobe Campaign podem ser personalizadas de várias maneiras


## Logs de rastreamento e entrega{#gs-tracking-logs}

O monitoramento de entregas após serem enviados é uma etapa essencial para garantir que as campanhas de marketing sejam eficientes e atinjam os clientes. Você pode monitorar após enviar uma entrega, bem como entender como as falhas de entrega e as quarentenas são gerenciadas.
