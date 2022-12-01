---
audience: end-user
title: Monitorar logs do delivery
description: Documentação da Web do Campaign v8
source-git-commit: 4ed89d326acd3b7d5d8f14bec68cceda3c8169fb
workflow-type: tm+mt
source-wordcount: '332'
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

Para visualizar os logs, clique no botão **Logs** botão.

![](assets/logs.png)

Várias guias contêm informações (se houver) sobre o Envio de logs, Logs de exclusão, Causas de exclusão, Logs de rastreamento e URLs rastreados.

**Los** guia

O **Logs** contém todas as mensagens relacionadas ao delivery e às provas. Os ícones especiais permitem identificar erros ou avisos.

Todas as etapas de validação, avisos e erros são listados. Os ícones coloridos mostram o tipo de mensagem:

* O ícone cinza indica uma mensagem informativa.
* O ícone amarelo indica um erro de processamento não crítico.
* O ícone vermelho indica um erro crítico que impede o envio do delivery.

**Guia Deliveries**

O **Deliveries** oferece um histórico de todas as ocorrências do delivery. A lista de mensagens enviadas com os status é armazenada aqui. Assim, você pode exibir o status do delivery para cada recipient.

**Exclusões** guia

A guia Exclusion logs lista todas as mensagens que foram excluídas do público-alvo enviado e especifica o motivo da falha de envio.

**Causas da exclusão** guia

O **Causas da exclusão** exibe o volume (em número) das mensagens que foram excluídas do público-alvo enviado.

**URLs rastreados** guia

O **URLs rastreados** exibições de guia

**Guia Rastreamento**

A guia **Tracking** lista o histórico de rastreamento desse delivery. Esta guia exibe os dados de rastreamento das mensagens enviadas, ou seja, todas as URLs sujeitas ao rastreamento por meio do Adobe Campaign. Os dados de rastreamento são atualizados de hora em hora.

>[!NOTE]
>
>Se o rastreamento não estiver ativado para um delivery, essa guia não será exibida.

Os dados de Tracking são interpretados nos relatórios de delivery. Consulte esta seção.



