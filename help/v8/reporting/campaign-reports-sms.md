---
audience: end-user
title: Relatórios de campanha para o canal SMS
description: Entender os relatórios de campanha do canal SMS
badge: label="Beta"
source-git-commit: 5d577c07c4d754e9265482f858c17740f304db42
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 11%

---


# Relatórios de campanha para o canal SMS {#campaign-reports-sms-channel}

Cada relatório de campanha é dividido em widgets diferentes detalhando o sucesso e os erros da campanha. Para o canal SMS, os relatórios e as métricas são detalhados abaixo. Saiba como acessar os relatórios de campanha no [esta página](campaign-reports.md).

## Resumo da entrega {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Visão geral da entrega"
>abstract="A variável **Visão geral da entrega** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre como os visitantes se envolvem com o delivery de SMS."


A variável **[!UICONTROL Visão geral da entrega]** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre como os visitantes se envolvem com o delivery de SMS. As métricas estão detalhadas abaixo.

![](assets/campaign_report_sms_1.png)

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
>abstract="A variável **Estatísticas iniciais do público-alvo** A tabela exibe dados relativos aos seus destinatários"

A variável **[!UICONTROL Estatísticas iniciais do público-alvo]** A tabela exibe dados relativos aos recipients. As métricas estão detalhadas abaixo.


![](assets/campaign_report_sms_2.png)

+++Saiba mais sobre métricas de relatório de campanha por SMS.

* **[!UICONTROL Público inicial]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Rejeitado por regras]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++


### Estatísticas de execução {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Estatísticas de execução"
>abstract="A variável **Estatísticas de execução** a tabela detalha o sucesso do delivery: mensagens a serem entregues, sucesso, erros e novas quarentenas."


A variável **[!UICONTROL Estatísticas de execução]** A tabela detalha o sucesso do delivery. As métricas estão detalhadas abaixo.


![](assets/campaign_report_sms_3.png)

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
>abstract="A variável **Fluxos de clique gerados** A tabela mostra os dados disponíveis relativos a como seus recipients interagiram com seu delivery."

A variável **[!UICONTROL Fluxos de clique gerados]** A tabela exibe dados relativos a como seus recipients interagiram com o delivery. As métricas estão detalhadas abaixo.

![](assets/campaign_report_sms_4.png)

+++Saiba mais sobre métricas de relatório de campanha por SMS.

* **[!UICONTROL Cliques distintos]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Clicks]** : Número total de cliques nos links nos deliveries.

* **[!UICONTROL Reactivity]**: Taxa do número de recipients alvos que clicaram em um delivery em relação ao número estimado de recipients alvos que abriram um delivery.

+++