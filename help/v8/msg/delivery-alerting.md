---
audience: end-user
title: Alertas de entrega
description: Saiba como trabalhar com alertas de delivery.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 2%

---

# Introdução a alertas de entrega {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Alertas de entrega"
>abstract="Os Alertas de delivery agora estão disponíveis no Campaign. Esse recurso é um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre as execuções de delivery."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

O Alertas de delivery é um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre suas execuções de delivery. Os recipients podem monitorar deliveries em andamento processados pelo Adobe Campaign e tomar as medidas apropriadas caso surjam problemas.

As notificações podem ser personalizadas com base em critérios de alerta específicos definidos pela interface da Web do Adobe Campaign.

Para obter mais informações sobre como gerenciar falhas de delivery, consulte o [Documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## Conteúdo de notificação por email {#content}

As notificações por email incluem as seguintes seções:

* **Resumo**: exibe o número de deliveries que atendem aos critérios definidos, com rótulos e cores para cada critério.
* **Detalhes**: lista todos os critérios de delivery definidos para o painel e os deliveries correspondentes para cada critério.

![](assets/alerting-email.png)

## Configurar alertas de entrega {#set-up}

Para ajudar você a configurar esses alertas, a interface da Web do Campaign permite criar e gerenciar:

* **Painéis de alertas de entrega**: especifique os recipients, defina critérios de alerta para incluir no painel e acesse um histórico de alertas enviados. [Saiba como trabalhar com painéis](../msg/delivery-alerting-dashboards.md)
* **Critérios de alerta de entrega**: a interface do usuário da Web do Campaign fornece critérios de alerta predefinidos (deliveries com baixa taxa de transferência, deliveries cuja preparação falhou...) que podem ser adicionados ao painel. Você também pode criar seus próprios critérios para atender às suas necessidades. [Saiba como trabalhar com critérios](../msg/delivery-alerting-criteria.md)

Digamos que você queira notificar os usuários com direitos administrativos somente sobre deliveries com falha e os usuários de marketing sobre deliveries com uma alta taxa de erro de rejeição temporária. Para fazer isso, crie dois painéis separados com os critérios apropriados para cada grupo de recipients.

>[!NOTE]
>
>Para acessar e configurar painéis e critérios de alerta, você deve ter **direitos de administração** ou fazer parte do **Supervisores de entrega** grupo de segurança. Os usuários padrão não podem acessar painéis na interface do Adobe Campaign, mas podem receber notificações de alerta. [Saiba mais sobre acesso e permissões](../get-started/permissions.md)
