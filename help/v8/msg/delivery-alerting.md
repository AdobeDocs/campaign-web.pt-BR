---
audience: end-user
title: Alerta de entrega
description: Saiba como trabalhar com alertas de delivery.
badge: label="Disponibilidade limitada"
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: a28bc98d1735232d8aa0b0daaeca3969913e548c
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 8%

---

# Introdução a alertas de entrega {#gs-delivery-alerting}

Os alertas de delivery são um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre suas execuções de delivery. Os recipients monitoram deliveries em andamento processados pelo Adobe Campaign e tomam as medidas apropriadas se surgirem problemas.

As notificações são personalizadas com base em critérios de alerta específicos definidos pela interface da Web do Adobe Campaign.

Para obter mais informações sobre o gerenciamento de falhas de entrega, consulte a [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

>[!AVAILABILITY]
>
>Esse recurso está na disponibilidade limitada (DL). É restrita aos clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não pode ser implantada em nenhum outro ambiente.

## Conteúdo de notificação por email {#content}

As notificações por email incluem as seguintes seções:

* **Resumo**: exibe o número de entregas que atendem aos seus critérios definidos, com rótulos e cores para cada critério.
* **Detalhes**: lista todos os critérios de entrega definidos para o painel e as entregas correspondentes para cada critério.

![Descrição: esta captura de tela mostra o layout de notificação por email, incluindo as seções de resumo e detalhes.](assets/alerting-email.png)

## Configurar alertas de entrega {#set-up}

Para configurar esses alertas, a interface da Web do Campaign permite criar e gerenciar:

* **Painéis de alertas de entrega**: especifique destinatários, defina critérios de alerta para incluir no painel e acesse um histórico de alertas enviados. [Saiba como trabalhar com painéis](../msg/delivery-alerting-dashboards.md).
* **Critérios de alerta de entrega**: a interface da Web do Campaign fornece critérios de alerta predefinidos, como entregas com baixa taxa de transferência ou entregas cuja preparação falhou. Você pode adicionar esses critérios ao painel ou criar seus próprios critérios para atender às suas necessidades. [Saiba como trabalhar com critérios](../msg/delivery-alerting-criteria.md).

Por exemplo, notifique usuários com direitos administrativos somente sobre deliveries com falha e notifique usuários de marketing sobre deliveries com uma alta taxa de erro de rejeição temporária. Para fazer isso, crie dois painéis separados com os critérios apropriados para cada grupo de recipients.

>[!NOTE]
>
>Para acessar e configurar painéis e critérios de alerta, você deve ter **direitos de administração** ou fazer parte do grupo de segurança **Supervisores de Entrega**. Os usuários padrão não podem acessar painéis na interface do Adobe Campaign, mas podem receber notificações de alerta. [Saiba mais sobre acesso e permissões](../get-started/permissions.md).