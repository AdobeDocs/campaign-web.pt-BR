---
audience: end-user
title: Monitorar logs do delivery
description: Documentação da Web do Campaign v8
exl-id: 2eb7457e-32f7-4729-99c8-91bf287f0192
source-git-commit: 13765b02288ec4682c5d55603c68f8ea1a5758f8
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 46%

---

# Monitorar logs do delivery {#delivery-logs}

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_preparation_logs"
>title="Logs do delivery"
>abstract="TBC"

Após preparar e enviar um email, os logs do delivery permitem verificar se não há erro. Esses logs podem ser acessados diretamente do painel de mensagens. Eles mostram os detalhes do envio, o target que foi excluído e o motivo, bem como as informações de rastreamento, como aberturas e cliques.

Para visualizar os logs, acesse o painel do delivery e clique no botão **Logs** botão.

Várias guias estão disponíveis:

## Logs

O **Logs** contém todas as mensagens relacionadas ao delivery e às provas. Os ícones especiais permitem identificar erros ou avisos.

Todas as etapas de validação, avisos e erros são listados. Os ícones coloridos mostram o tipo de mensagem:

* O ícone cinza indica uma mensagem informativa.
* O ícone amarelo indica um erro de processamento não crítico.
* O ícone vermelho indica um erro crítico que impede o envio do delivery.

![](assets/logs.png)

## Entregas

O **Deliveries** oferece um histórico de todas as ocorrências do delivery. A lista de mensagens enviadas com os status é armazenada aqui. Assim, você pode exibir o status do delivery para cada recipient.

![](assets/logs2.png)

## Exclusões

O **Logs de exclusão** lista todas as mensagens que foram excluídas do público-alvo enviado e especifica o motivo da falha de envio.

![](assets/logs3.png)

## Causas de exclusão

O **Causas da exclusão** exibe o volume (em número) das mensagens que foram excluídas do público-alvo enviado.

![](assets/logs4.png)

## URLs rastreados

O **URLs rastreados** agrupa os URLs contidos na mensagem enviada, incluindo o tipo de URL e o URL de origem.

![](assets/logs5.png)

## Rastreamento

A guia **Tracking** lista o histórico de rastreamento desse delivery. Esta guia exibe os dados de rastreamento das mensagens enviadas, ou seja, todas as URLs sujeitas ao rastreamento por meio do Adobe Campaign.

>[!NOTE]
>
>Se o rastreamento não estiver ativado para um delivery, essa guia não será exibida.

![](assets/logs6.png)
