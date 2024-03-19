---
audience: end-user
title: Relatórios de campanha para o canal de correspondência direta
description: Entender os relatórios de campanha do canal de correspondência direta
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 9%

---

# Relatórios de campanha para o canal de correspondência direta {#campaign-reports-direct-mail}

Cada relatório de campanha é dividido em widgets diferentes detalhando o sucesso e os erros da campanha. Para o canal de correspondência direta, os relatórios e as métricas são detalhados abaixo. Saiba como acessar os relatórios de campanha no [esta página](campaign-reports.md).

## Resumo da entrega {#delivery-summary-direct}

### Visão geral da entrega {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_delivery_overview_direct_mail"
>title="Visão geral da entrega"
>abstract="A variável **Visão geral da entrega** O apresenta as principais métricas de desempenho (KPIs) com informações detalhadas sobre a interação de seus visitantes com cada delivery de correspondência direta. As métricas estão descritas abaixo."

A variável **[!UICONTROL Visão geral da entrega]** O apresenta as principais métricas de desempenho (KPIs) com informações detalhadas sobre a interação de seus visitantes com cada delivery de correspondência direta. As métricas estão descritas abaixo.

![](assets/direct-mail-campaign-overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de cliques]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

+++

### Estatísticas iniciais do público-alvo {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_target_audience_direct_mail"
>title="Estatísticas iniciais do público-alvo"
>abstract="Os dados do recipient e as informações da mensagem são exibidos no **Estatísticas iniciais do público-alvo** tabela, que reflete a análise de preparação do delivery."

A variável **[!UICONTROL Estatísticas iniciais do público-alvo]** A tabela exibe dados relativos aos recipients. As métricas são calculadas durante a preparação do delivery e mostram: o público inicial, o número de mensagens a serem enviadas e o número de recipients excluídos.

![](assets/direct-mail-campaign-target-audience.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre as métricas de Estatísticas iniciais de público-alvo.

* **[!UICONTROL Público inicial]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Rejeitado por regras]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de execução {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_execution_statistics_direct_mail"
>title="Estatísticas de entrega"
>abstract="A variável **Estatísticas de execução** A tabela detalha o sucesso do delivery de correspondência direta e os erros que ocorreram."

![](assets/direct-mail-campaign-exec.png)

A variável **[!UICONTROL Estatísticas de execução]** A tabela fornece um detalhamento do sucesso de cada delivery de correspondência direta, com métricas detalhadas descritas abaixo.

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

+++

### Fluxos de cliques gerados {#click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_clicks_direct_mail"
>title="Fluxos de cliques gerados"
>abstract="A tabela **Fluxos de clique gerados** mostra os dados disponíveis relativos a como seus destinatários interagiram com a entrega."

![](assets/direct-mail-campaign-clicks.png){zoomable=&quot;yes&quot;}{align="center"}

A variável **Fluxos de clique gerados** A tabela ilustra os motivos que impediram os perfis de usuário, excluídos dos perfis direcionados, de receber a mensagem.

+++Saiba mais sobre Métricas de fluxos de clique gerados.

* **[!UICONTROL Cliques únicos]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Total de cliques]**: Número total de cliques nos links nos deliveries.

* **[!UICONTROL Reatividade]**: Taxa do número de recipients alvos que clicaram em um delivery em relação ao número estimado de recipients alvos que abriram um delivery.

+++
