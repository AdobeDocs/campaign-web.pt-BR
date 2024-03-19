---
audience: end-user
title: Relatórios de campanha para o canal push
description: Entender os relatórios de campanha do canal push
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 19%

---

# Relatórios de campanha para o canal push {#campaign-reports-push-channel}

Cada relatório de campanha é dividido em widgets diferentes detalhando o sucesso e os erros da campanha. Para o canal de push, os relatórios e as métricas são detalhados abaixo. Saiba como acessar os relatórios de campanha no [esta página](campaign-reports.md).

## Resumo da entrega {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Visão geral da entrega"
>abstract="O relatório **Visão geral da entrega** fornece indicadores principais de desempenho (KPIs) com informações detalhadas sobre o engajamento de visitantes com a entrega de notificações por push."

A variável **[!UICONTROL Visão geral da entrega]** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre como seus visitantes se envolvem com a entrega de notificação por push. As métricas estão detalhadas abaixo.

![](assets/campaign-reporting-push-summary.png){zoomable=&quot;yes&quot;}


+++Saiba mais sobre métricas de relatório de campanha por push.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de cliques]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

+++

### Estatísticas iniciais do público-alvo {#delivery-summary-push-initial-target}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Estatísticas iniciais do público-alvo"
>abstract="A tabela **Estatísticas iniciais do público-alvo** exibe dados relativos aos destinatários"

A variável **[!UICONTROL Estatísticas iniciais do público-alvo]** A tabela exibe dados relativos aos recipients. As métricas estão detalhadas abaixo.

![](assets/campaign-reporting-push-target.png){zoomable=&quot;yes&quot;}


+++Saiba mais sobre métricas de relatório de campanha por push.

* **[!UICONTROL Público inicial]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Rejeitado por regras]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de execução {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Estatísticas de execução"
>abstract="A tabela **Estatísticas de execução** detalha o sucesso da entrega: mensagens a serem entregues, sucesso, erros e novas quarentenas."

A variável **[!UICONTROL Estatísticas de execução]** A tabela detalha o sucesso do delivery. As métricas estão detalhadas abaixo.

![](assets/campaign-reporting-push-exec.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de relatório de campanha por push.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (registro inválido, rejeição de mensagem, erro de carga, por exemplo). em relação ao número de mensagens a serem entregues.

  Os tipos de erro de notificações por push estão listados na variável [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Fluxos de cliques gerados {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Fluxos de cliques gerados"
>abstract="A tabela **Fluxos de clique gerados** mostra os dados disponíveis relativos a como seus destinatários interagiram com a entrega."

A variável **[!UICONTROL Fluxos de clique gerados]** A tabela exibe dados relativos a como seus recipients interagiram com o delivery. As métricas estão detalhadas abaixo.

![](assets/campaign-reporting-push-clicks.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de relatório de campanha por push.

* **[!UICONTROL Cliques únicos]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Total de cliques]**: Número total de cliques nos links nos deliveries.

* **[!UICONTROL Reatividade]**: Taxa do número de recipients alvos que clicaram em um delivery em relação ao número estimado de recipients alvos que abriram um delivery.

+++
