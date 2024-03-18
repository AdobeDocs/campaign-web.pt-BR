---
audience: end-user
title: Relatórios de campanha para o canal SMS
description: Entender os relatórios de campanha do canal SMS
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 20%

---

# Relatórios de campanha para o canal SMS {#campaign-reports-sms-channel}

Cada relatório de campanha é dividido em widgets diferentes detalhando o sucesso e os erros da campanha. Para o canal SMS, os relatórios e as métricas são detalhados abaixo. Saiba como acessar os relatórios de campanha no [esta página](campaign-reports.md).

## Resumo da entrega {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Visão geral da entrega"
>abstract="O relatório **Visão geral da entrega** fornece indicadores principais de desempenho (KPIs) com informações detalhadas sobre o engajamento de visitantes com a entrega por SMS."


A variável **[!UICONTROL Visão geral da entrega]** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre como os visitantes se envolvem com o delivery de SMS. As métricas estão detalhadas abaixo.

![](assets/campaign_report_sms_1.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de relatório de campanha por SMS.

* **[!UICONTROL Total enviado]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Cliques distintos]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

+++


### Estatísticas iniciais do público-alvo {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Estatísticas iniciais do público-alvo"
>abstract="A tabela **Estatísticas iniciais do público-alvo** exibe dados relativos aos destinatários"

A variável **[!UICONTROL Estatísticas iniciais do público-alvo]** A tabela exibe dados relativos aos recipients. As métricas estão detalhadas abaixo.


![](assets/campaign_report_sms_2.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de relatório de campanha por SMS.

* **[!UICONTROL Público inicial]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Rejeitado por regras]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++


### Estatísticas de execução {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Estatísticas de execução"
>abstract="A tabela **Estatísticas de execução** detalha o sucesso da entrega: mensagens a serem entregues, sucesso, erros e novas quarentenas."


A variável **[!UICONTROL Estatísticas de execução]** A tabela detalha o sucesso do delivery. As métricas estão detalhadas abaixo.


![](assets/campaign_report_sms_3.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de relatório de campanha por SMS.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

  Os tipos de erro de SMS estão listados no [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Fluxos de cliques gerados {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Fluxos de cliques gerados"
>abstract="A tabela **Fluxos de clique gerados** mostra os dados disponíveis relativos a como seus destinatários interagiram com a entrega."

A variável **[!UICONTROL Fluxos de clique gerados]** A tabela exibe dados relativos a como seus recipients interagiram com o delivery. As métricas estão detalhadas abaixo.

![](assets/campaign_report_sms_4.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de relatório de campanha por SMS.

* **[!UICONTROL Cliques distintos]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Cliques]**: Número total de cliques nos links nos deliveries.

* **[!UICONTROL Reatividade]**: Taxa do número de recipients alvos que clicaram em um delivery em relação ao número estimado de recipients alvos que abriram um delivery.

+++
