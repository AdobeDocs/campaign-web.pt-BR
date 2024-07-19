---
audience: end-user
title: Sobre a quarentena
description: Entender o gerenciamento de endereços em quarentena
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: 42e5f3b0ab5d31389b7a9d0544d3d265ec70fffc
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 13%

---

# Quarentena

O Adobe Campaign gerencia endereços em quarentena (email, SMS, notificação por push).

A quarentena se aplica somente a um **endereço de email**, um **número de telefone** ou um **token de dispositivo**, mas não ao próprio perfil. Por exemplo, um perfil cujo endereço de email esteja em quarentena pode atualizar seu perfil e inserir um novo endereço, podendo então ser direcionado em ações de entrega novamente. Da mesma forma, se dois perfis tiverem o mesmo número de telefone, ambos serão afetados se o número estiver em quarentena.


>[!CAUTION]
>
>A quarentena no Adobe Campaign diferencia maiúsculas de minúsculas.

## O que é quarentena?

A quarentena é a maneira de **gerenciar os endereços inválidos nas entregas**.

Se um delivery tiver uma alta taxa de endereços inválidos, ele poderá ser considerado spam. Incluir na lista de bloqueios O gerenciamento desses endereços com quarentena evitará que você seja solicitado pelos provedores de internet a colocar esses endereços em quarentena. Isso é importante para sua reputação.

Quando um endereço é colocado em quarentena no Adobe Campaign, o perfil é excluído automaticamente do público-alvo durante a análise do delivery.

A quarentena ajudará você a reduzir o custo de envio de SMS, excluindo números de telefone incorretos dos deliveries.

## Por que um endereço é enviado para quarentena

Muitos motivos podem enviar um endereço para quarentena:

- Para SMS, números de telefone incorretos
- Para SMS, quando o perfil responder a uma mensagem SMS com uma palavra-chave como &quot;PARAR&quot;
- Para emails, quando a mensagem é relatada como spam. A mensagem é automaticamente redirecionada para uma caixa de entrada técnica gerenciada pelo Adobe. Incluir na lista de bloqueios Em seguida, o endereço de email do usuário é enviado automaticamente para quarentena com o status.
- Um endereço de email pode ser colocado em quarentena, por exemplo, quando a caixa de entrada estiver cheia, se o endereço não existir ou se o servidor de email não estiver disponível.

[Saiba mais sobre falhas de entrega](https://experienceleague.adobe.com/en/docs/campaign-classic/using/sending-messages/monitoring-deliveries/understanding-delivery-failures)

## Onde encontrar os endereços em quarentena

Você pode exibir todos os endereços em quarentena de sua instância no **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]**. Esta seção lista os elementos em quarentena para os canais de email, SMS e notificação por push.

![](assets/quarantine_location.png){zoomable="yes"}

Você também pode ter o relatório sobre a quarentena na sua instância:

![](assets/quarantine_reports.png){zoomable="yes"}

Para cada delivery, você também pode verificar o Delivery summary report: ele mostra o número de endereços em quarentena no target do delivery:

![](assets/quarantine_delivery.png){zoomable="yes"}

Você pode ter mais possibilidades para gerenciar os endereços em quarentena no console do Adobe Campaign. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
