---
audience: end-user
title: Alerta de entrega
description: Saiba como trabalhar com alertas de delivery.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: dfd5f2e000b02d4382eaac0c9bb00fe940a99f79
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 19%

---

# Introdução a alertas de entrega {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Alerta de entrega"
>abstract="Os alertas de entrega agora estão disponíveis no Campaign. Esse recurso é um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre as execuções de entrega."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

O Alerta de entrega é um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre suas execuções de entrega. Os recipients podem monitorar deliveries em andamento processados pelo Adobe Campaign e tomar as medidas apropriadas caso surjam problemas.

As notificações podem ser personalizadas com base em critérios de alerta específicos definidos pela interface da Web do Adobe Campaign.

Para obter mais informações sobre como gerenciar falhas de entrega, consulte a [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Conteúdo de notificação por email {#content}

As notificações por email incluem as seguintes seções:

* **Resumo**: exibe o número de entregas que atendem aos seus critérios definidos, com rótulos e cores para cada critério.
* **Detalhes**: lista todos os critérios de entrega definidos para o painel e as entregas correspondentes para cada critério.

![](assets/alerting-email.png)

## Configurar alertas de entrega {#set-up}

Para ajudar você a configurar esses alertas, a interface da Web do Campaign permite criar e gerenciar:

* **Painéis de alertas de entrega**: especifique destinatários, defina critérios de alerta para incluir no painel e acesse um histórico de alertas enviados. [Saiba como trabalhar com painéis](../msg/delivery-alerting-dashboards.md)
* **Critérios de alerta de entrega**: a interface da Web do Campaign fornece critérios de alerta predefinidos (entregas com baixa taxa de transferência, entregas cuja preparação falhou...) que você pode adicionar ao seu painel. Você também pode criar seus próprios critérios para atender às suas necessidades. [Saiba como trabalhar com critérios](../msg/delivery-alerting-criteria.md)

Digamos que você queira notificar os usuários com direitos administrativos somente sobre deliveries com falha e os usuários de marketing sobre deliveries com uma alta taxa de erro de rejeição temporária. Para fazer isso, crie dois painéis separados com os critérios apropriados para cada grupo de recipients.

>[!NOTE]
>
>Para acessar e configurar painéis e critérios de alerta, você deve ter **direitos de administração** ou fazer parte do grupo de segurança **Supervisores de Entrega**. Os usuários padrão não podem acessar painéis na interface do Adobe Campaign, mas podem receber notificações de alerta. [Saiba mais sobre acesso e permissões](../get-started/permissions.md)
