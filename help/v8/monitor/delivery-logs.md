---
audience: end-user
title: Monitorar logs da entrega
description: Saiba como monitorar logs da entrega
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 71%

---

# Monitorar logs da entrega {#delivery-logs}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Logs de entrega"
>abstract="Os logs de entrega mostram os detalhes do envio. Eles mostram os detalhes do envio, o público-alvo que foi excluído e o motivo, e as informações de rastreamento, como aberturas e cliques."

Depois que a entrega estiver preparada e você clicar no botão **Enviar**, navegue até os logs de entrega para verificar os dados de avisos, erros, status, exclusões e rastreamento. Esses logs podem ser acessados diretamente do painel de mensagens. Eles mostram os detalhes do envio, o público-alvo que foi excluído e o motivo, e as informações de rastreamento, como aberturas e cliques.

Para visualizar os logs, acesse o painel da entrega e clique no botão **Logs**.

As seguintes guias estão disponíveis:

* [Logs](#logs-tab)
* [Entregas](#deliveries-tab)
* [Exclusões](#exclusion-tab)
* [Causas da exclusão](#exclusion-causes)
* [URLs rastreados](#tracked-urls)
* [Rastreamento](#tracking)

## Logs {#logs-tab}

A guia **Logs** contém todas as mensagens relacionadas à entrega e às provas. Ícones específicos permitem identificar erros ou avisos.

Todas as etapas de validação, avisos e erros são listados. Os ícones coloridos mostram o tipo de mensagem:

* O ícone cinza indica uma mensagem informativa.
* O ícone amarelo indica um erro de processamento não crítico.
* O ícone vermelho indica um erro crítico que impede o envio do delivery. Erros críticos devem ser corrigidos para que o delivery seja enviado.

![](assets/logs.png){zoomable="yes"}


## Entregas {#deliveries-tab}

A guia **Logs de envio** contém o histórico de todas as ocorrências da entrega. A lista de mensagens enviadas com os status é armazenada aqui. Assim, você pode exibir o status da entrega para cada destinatário.

![](assets/logs2.png){zoomable="yes"}

## Exclusões {#exclusion-tab}

A guia **Logs excluídos** lista todas as mensagens excluídas do público-alvo e especifica o motivo da falha no envio.

![](assets/logs3.png){zoomable="yes"}

## Causas da exclusão {#exclusion-causes-tab}

A guia **Causas de exclusão** exibe, para cada causa possível, o número de mensagens que foram excluídas do destino.

![](assets/logs4.png){zoomable="yes"}

## URLs rastreados {#tracked-urls-tab}

A guia **URLs rastreadas** reagrupa as URLs contidas nas mensagens enviadas, incluindo o tipo de URL e a URL de origem.

![](assets/logs5.png){zoomable="yes"}

## Rastreamento {#tracking-tab}

A guia **Rastreamento** lista o histórico de rastreamento dessa entrega. Esta guia exibe os dados de rastreamento das mensagens enviadas, ou seja, todas as URLs sujeitas ao rastreamento pelo Adobe Campaign.


![](assets/logs6.png){zoomable="yes"}

>[!NOTE]
>
>Se o rastreamento não estiver ativado para uma entrega, essa guia não será exibida.