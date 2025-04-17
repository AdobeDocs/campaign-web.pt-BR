---
audience: end-user
title: Relatórios globais para o canal de push
description: Entender os relatórios globais do canal de push
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 23%

---

# Relatórios globais para o canal de push {#campaign-reports-push}

Os relatórios globais fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até o menu **[!UICONTROL Relatórios]** na seção **[!UICONTROL Relatórios]**. Você pode filtrar seus dados dependendo da data, pasta ou regras do relatório. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-push}

### Visão geral da entrega {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Visão geral da entrega por push"
>abstract="Os KPIs da **Visão geral da entrega por push** fornecem uma análise completa das entregas por push, com insights detalhados e dados específicos. Esses KPIs fornecem detalhes abrangentes sobre o desempenho, a eficácia e os resultados das entregas."

O relatório **[!UICONTROL Visão geral da entrega]** fornece KPIs (indicadores-chave de desempenho) que fornecem informações detalhadas sobre como seus visitantes se envolvem com cada entrega de notificação por push. As métricas estão detalhadas abaixo.

![Métricas de visão geral da entrega, mostrando KPIs relacionados ao desempenho da notificação por push.](assets/global_report_push_delivery_overview.png){zoomable="yes"}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a serem entregues]**: número total de mensagens processadas durante a preparação da entrega.

* **[!UICONTROL Entregues]**: número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de cliques]**: número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de entrega e retorno automático em relação ao número total de mensagens enviadas.

+++

### Público-alvo {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="População direcionada por push"
>abstract="O gráfico e a tabela **População direcionada** exibem dados relacionados ao público-alvo das mensagens por push, apresentando informações sobre mensagens a serem entregues e exclusões."

A tabela e o gráfico **[!UICONTROL Público-alvo]** apresentam dados relacionados aos seus destinatários para cada entrega de notificação por push enviada. As métricas estão detalhadas abaixo.

![Métricas de público-alvo direcionadas, mostrando dados relacionados a destinatários e exclusões para notificações por push.](assets/global_report_push_targeted_audience.png){zoomable="yes"}

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: número total de destinatários direcionados.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* **[!UICONTROL Exclusão]**: número total de endereços ignorados durante a análise ao aplicar as regras: endereço em quarentena, em incluído na lista de bloqueios e motivos semelhantes.

+++

### Estatísticas de entrega {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Estatísticas da entrega por push"
>abstract="O relatório **Estatísticas gerais** fornece informações sobre notificações por push enviadas, incluindo taxas de sucesso, erros e quarentenas."

A tabela **[!UICONTROL Estatísticas de entrega]** detalha o sucesso de cada entrega de notificação por push. As métricas estão detalhadas abaixo.

![Métricas de estatísticas de entrega, mostrando taxas de sucesso, erros e quarentenas para notificações por push.](assets/global_report_push_delivery_statistics.png){zoomable="yes"}

+++Saiba mais sobre Métricas de estatísticas de delivery.

* **[!UICONTROL Total de mensagens]**: número total de mensagens a serem entregues após a preparação da entrega.

* **[!UICONTROL Success]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Devoluções]**: Número total de erros acumulados durante as entregas e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novas quarentenas]**: Número total de endereços colocados em quarentena após uma entrega com falha (registro inválido, rejeição de mensagem, erro de carga e motivos semelhantes) em relação ao número de mensagens a serem entregues.

  Os tipos de erro de notificações por push estão listados na [documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Causas da exclusão {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Causas de exclusão de notificações por push"
>abstract="O gráfico e a tabela **Causas de exclusão** ilustram os diversos motivos que impediram os perfis de usuário de receber as notificações por push."

O gráfico e a tabela **[!UICONTROL Causas da exclusão]** exibem os motivos que impediram os perfis de usuário, que foram excluídos dos perfis direcionados, de receber a mensagem.

Os tipos de erro de notificações por push estão listados na [documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Taxa de transferência de entrega {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Relatório de taxa de transferência de entrega"
>abstract="O relatório de **Taxa de transferência de entrega** apresenta informações detalhadas sobre a taxa de transferência de entrega de notificações por push em toda a plataforma no período especificado."

![Métricas de taxa de transferência de entrega, mostrando taxas de erro e sucesso para notificações por push durante um período especificado.](assets/global_report_push_delivery_throughput.png){zoomable="yes"}

O relatório **[!UICONTROL Taxa de transferência de entrega]** oferece insights abrangentes sobre a eficácia do sistema de entrega de notificações por push, oferecendo um resumo detalhado das taxas de sucesso e erro em um período especificado.