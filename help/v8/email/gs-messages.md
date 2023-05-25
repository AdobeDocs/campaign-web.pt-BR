---
audience: end-user
title: Introdução a mensagens e entregas no Campaign Web v8
description: Saiba como trabalhar com entregas e enviar mensagens usando o Campaign Web
badge: label="Alpha" type="Positive"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: c5a0103cc630e3ec44747211977988145cb75a25
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 34%

---

# Introdução a mensagens no Campaign Web {#gs-messages}

Com o Adobe Campaign, você pode enviar campanhas entre canais, incluindo emails, SMS e notificações por push, e medir sua eficácia usando vários relatórios dedicados. Essas mensagens são projetadas e enviadas por deliveries, além disso podem ser personalizadas para cada recipient. Esses deliveries podem ser independentes ou incluídos no contexto de uma campanha de marketing.

O Adobe Campaign v8 vem com os seguintes canais de entrega:

* **Canal de email**: entregas de email permitem enviar emails personalizados para a população do target. Saiba como criar e enviar um email no [esta página](../email/create-email.md).

* **Canal SMS**: deliveries em canais móveis permitem enviar SMS personalizado para a população do target.  Saiba como criar e enviar SMS no [esta página](../sms/create-sms.md).

* **Canal de aplicativo móvel**: as entregas por aplicativo móvel permitem enviar as notificações para sistemas iOS e Android.  Saiba como criar e enviar notificações por push no [esta página](../push/gs-push.md).

## Criar um delivery {#create-delivery}

Você pode criar deliveries independentes a partir do **[!UICONTROL Entregas]** menu à esquerda, ou crie deliveries no contexto de uma campanha de marketing, no **[!UICONTROL Campanhas]** menu esquerdo.

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
1. Depois que as mensagens forem enviadas, navegue até o **Relatórios** para acessar as métricas principais. Saiba mais sobre relatórios de entrega em [nesta seção](../reporting/reports.md).

>[!TAB Criar um delivery em uma campanha]

Para criar um delivery em uma campanha, siga estas etapas:

1. Crie uma campanha ou abra uma campanha existente. Saiba mais sobre [campanhas de marketing](../campaigns/gs-campaigns.md).
1. Crie um workflow ou abra um workflow existente.
1. Adicionar e configurar um **[!UICONTROL Criar público-alvo]** e clique no link `+`botão.

   ![](assets/add-delivery-in-wf.png)

   A variável **[!UICONTROL Criar público-alvo]** A atividade está detalhada em [nesta seção](../workflows/targeting-activities.md).

1. Selecione uma atividade de delivery: **[!UICONTROL E-mail]**, **[!UICONTROL SMS]**, **[!UICONTROL Notificação por push (Android)]** ou **[!UICONTROL Notificação por push (iOS)]**. Saiba mais sobre as atividades de canal de delivery em um workflow e como definir um conteúdo de delivery neste [seção](../workflows/channel-activities.md).
1. Inicie o fluxo de trabalho e verifique os logs.

Você também pode adicionar deliveries em uma campanha sem criar um fluxo de trabalho. Para fazer isso, navegue até o **[!UICONTROL Entregas]** da campanha e clique no link **[!UICONTROL Criar entrega]** botão.

![](assets/new-campaign-delivery.png)

As etapas de configuração são semelhantes às dos deliveries independentes.

Para obter mais informações sobre como configurar uma campanha e gerenciar deliveries que pertencem a uma campanha, consulte [nesta seção](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Adicionar personalização{#personalization}

As mensagens entregues pelo Adobe Campaign podem ser personalizadas de várias maneiras. [Saiba mais sobre os recursos de personalização](../personalization/personalize.md).

Use o Campaign para criar conteúdo dinâmico e enviar mensagens personalizadas. Os recursos de personalização podem ser combinados para melhorar suas mensagens e criar uma experiência do usuário personalizada.

Você pode personalizar o conteúdo da mensagem ao:

* Inserir **campos de personalização** dinâmicos

   Os campos de personalização são usados na personalização de primeiro nível das mensagens. Você pode selecionar qualquer campo disponível no banco de dados no editor de personalização. Para uma entrega, é possível selecionar qualquer campo relacionado ao recipient, à mensagem ou à entrega. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo de suas mensagens. [Saiba mais](../personalization/personalize.md)

* Inserção de **blocos de conteúdo** predefinidos

   O Campaign vem com um conjunto de blocos de personalização contendo uma renderização específica que você pode inserir nas entregas. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para a mirror page da mensagem. Os blocos de conteúdo estão disponíveis em uma entrada dedicada no editor de personalização. [Saiba mais](../personalization/personalize.md#ootb-content-blocks)

* Criar **conteúdo condicional**

   Configure o conteúdo condicional para adicionar personalização dinâmica com base no perfil do recipient, por exemplo. Blocos de texto e/ou imagens são inseridos quando uma determinada condição é verdadeira. [Saiba mais](../personalization/conditions.md)

* Adicionar **ofertas personalizadas**

   Insira ofertas personalizadas no conteúdo da mensagem, dependendo do local do recipient, do tempo atual ou da última ordem de compra.


## Pré-visualizar e testar seus deliveries

Depois que o conteúdo da mensagem for definido, você poderá pré-visualizá-lo para controlar a renderização das mensagens e verificar as configurações de personalização com perfis de teste. [Saiba mais](../preview-test/preview-test.md)


## Logs de rastreamento e entrega{#gs-tracking-logs}

O monitoramento de entregas após serem enviados é uma etapa essencial para garantir que as campanhas de marketing sejam eficientes e atinjam os clientes. Você pode monitorar após enviar uma entrega, bem como entender como as falhas de entrega e as quarentenas são gerenciadas.
