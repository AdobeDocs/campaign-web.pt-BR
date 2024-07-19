---
audience: end-user
title: Relatórios de campanha para o canal de correspondência direta
description: Entender os relatórios de campanha do canal de correspondência direta
exl-id: 7817d4c5-1f97-4b17-8a5f-f1a5b8701fe9
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 21%

---

# Relatórios de campanha para o canal de correspondência direta {#campaign-reports-direct-mail}

Cada relatório de campanha é dividido em widgets diferentes detalhando o sucesso e os erros da campanha. Para o canal de correspondência direta, os relatórios e as métricas são detalhados abaixo. Saiba como acessar seus relatórios de campanha em [esta página](campaign-reports.md).

## Resumo da entrega {#delivery-summary-direct}

### Visão geral da entrega {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_delivery_overview_direct_mail"
>title="Visão geral da entrega"
>abstract="A **Visão geral da entrega** apresenta métricas principais de desempenho (KPIs) com informações detalhadas sobre as interações de visitantes com cada entrega de correspondência direta. As métricas estão descritas abaixo."

A **[!UICONTROL Visão geral da entrega]** apresenta as principais métricas de desempenho (KPIs), que fornecem insights detalhados sobre a interação de seus visitantes com cada entrega de correspondência direta. As métricas estão descritas abaixo.

![](assets/direct-mail-campaign-overview.png){zoomable="yes"}{align="center"}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a serem entregues]**: número total de mensagens processadas durante a preparação da entrega.

* **[!UICONTROL Entregues]**: número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de entrega e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de cliques]**: número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

+++

### Estatísticas iniciais do público-alvo {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_target_audience_direct_mail"
>title="Estatísticas iniciais do público-alvo"
>abstract="Os dados de destinatários e as informações da mensagem são exibidos na tabela **Estatísticas iniciais do público-alvo**, que reflete a análise de preparação da entrega."

A tabela **[!UICONTROL Estatísticas iniciais do público-alvo]** exibe os dados relativos aos seus destinatários. As métricas são calculadas durante a preparação do delivery e mostram: o público inicial, o número de mensagens a serem enviadas e o número de recipients excluídos.

![](assets/direct-mail-campaign-target-audience.png){zoomable="yes"}

+++Saiba mais sobre as métricas de Estatísticas iniciais de público-alvo.

* **[!UICONTROL Público-alvo inicial]**: número total de destinatários direcionados.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* incluir na lista de bloqueios **[!UICONTROL Rejected by rules]**: Número total de endereços ignorados durante a análise ao aplicar regras: endereço em falta, em quarentena, no, etc.

+++

### Estatísticas de execução {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_execution_statistics_direct_mail"
>title="Estatísticas de entrega"
>abstract="A tabela **Estatísticas de execução** detalha o sucesso da entrega de correspondência direta e os erros que ocorreram."

![](assets/direct-mail-campaign-exec.png)

A tabela **[!UICONTROL Estatísticas de execução]** fornece um detalhamento do sucesso de cada delivery de correspondência direta, com métricas detalhadas descritas abaixo.

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* **[!UICONTROL Success]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros]**: Número total de erros acumulados durante as entregas e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novas quarentenas]**: Número total de endereços colocados em quarentena após uma entrega com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

+++

### Fluxos de cliques gerados {#click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_clicks_direct_mail"
>title="Fluxos de cliques gerados"
>abstract="A tabela **Fluxos de clique gerados** mostra os dados disponíveis relativos a como seus destinatários interagiram com a entrega."

![](assets/direct-mail-campaign-clicks.png){zoomable="yes"}{align="center"}

A tabela **Fluxos de cliques gerados** ilustra os motivos que impediram os perfis de usuário, excluídos dos perfis direcionados, de receber a mensagem.

+++Saiba mais sobre Métricas de fluxos de clique gerados.

* **[!UICONTROL Cliques únicos]**: número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Total de cliques]**: número total de cliques nos links nas entregas.

* **[!UICONTROL Reatividade]**: taxa do número de recipients alvos que clicaram em uma entrega em relação ao número estimado de recipients alvos que abriram uma entrega.

+++
