---
audience: end-user
title: Sobre a quarentena
description: Entender o gerenciamento de endereços em quarentena
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 1%

---

# Gerenciamento de quarentena {#quarantines}

O Adobe Campaign gerencia endereços em quarentena para canais de email, push e SMS.

A quarentena se aplica somente a um **endereço de email**, um **número de telefone** ou um **token de dispositivo**, mas não ao próprio perfil. Por exemplo, um perfil cujo endereço de email está em quarentena pode ser atualizado com um novo endereço. O perfil pode então ser direcionado por ações de delivery novamente. Da mesma forma, se dois perfis compartilharem o mesmo número de telefone, ambos serão afetados se o número estiver em quarentena.

>[!CAUTION]
>
>A quarentena no Adobe Campaign diferencia maiúsculas de minúsculas.

## O que é quarentena {#quarantines-what}

A quarentena é o método usado para **gerenciar endereços inválidos nas entregas**.

Se um delivery tiver uma alta taxa de endereços inválidos, ele poderá ser considerado spam. Incluir na lista de bloqueios O gerenciamento desses endereços com quarentena ajuda a impedir que sejam migrados por provedores de internet. Isso é importante para manter sua reputação.

Quando um endereço é colocado em quarentena no Adobe Campaign, o perfil é automaticamente excluído do público-alvo durante a análise do delivery.

A quarentena reduz os custos de envio de SMS, excluindo números de telefone incorretos dos deliveries.

Saiba mais sobre quarentenas na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"}.

## Por que um endereço é enviado para quarentena {#quarantines-why}

Vários motivos podem enviar um endereço para quarentena:

* Para SMS, números de telefone incorretos
* Para SMS, quando o perfil responde a uma mensagem SMS com uma palavra-chave, como &quot;PARAR&quot;
* Para emails, quando a mensagem é relatada como spam. A mensagem é redirecionada automaticamente para uma caixa de entrada técnica gerenciada pela Adobe. Incluir na lista de bloqueios Em seguida, o endereço de email do usuário é enviado automaticamente para quarentena com o status.
* Um endereço de email pode ser colocado em quarentena, por exemplo, quando a caixa de entrada estiver cheia, se o endereço não existir ou se o servidor de email não estiver disponível.

Saiba mais sobre falhas de entrega na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"}.

## Onde encontrar os endereços em quarentena {#quarantines-where}

Você pode exibir todos os endereços em quarentena em sua instância no **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]**. Esta seção lista os elementos em quarentena para os canais de email, SMS e notificação por push.

![Local de quarentena na interface do Adobe Campaign](assets/quarantine_location.png){zoomable="yes"}

Você também pode acessar um relatório sobre a quarentena em sua instância:

![Colocar relatórios em quarentena na interface do Adobe Campaign](assets/quarantine_reports.png){zoomable="yes"}

Para cada delivery, você pode verificar o Relatório de resumo do delivery. Ele mostra o número de endereços em quarentena no target do delivery:

![Relatório de resumo de entrega mostrando endereços em quarentena](assets/quarantine_delivery.png){zoomable="yes"}

Você pode explorar mais opções para gerenciar endereços em quarentena no console do Adobe Campaign. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses).