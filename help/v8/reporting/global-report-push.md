---
audience: end-user
title: Relatórios globais para o canal de push
description: Entender os relatórios globais do canal de push
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 25%

---

# Relatórios globais para o canal de push {#campaign-reports-push}

Os relatórios globais fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até a **[!UICONTROL Relatórios]** no menu **[!UICONTROL Relatórios]** seção. Você pode filtrar seus dados dependendo da data do relatório, pasta ou regras. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-push}

### Visão geral da entrega {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Visão geral da entrega por push"
>abstract="Os KPIs da **Visão geral da entrega por push** fornecem uma análise completa das entregas por push, com insights detalhados e dados específicos. Esses KPIs fornecem detalhes abrangentes sobre o desempenho, a eficácia e os resultados das entregas."

A variável **[!UICONTROL Visão geral da entrega]** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre como seus visitantes se envolvem com cada delivery de notificação por push. As métricas estão detalhadas abaixo.

![](assets/global_report_push_delivery_overview.png){zoom=&quot;yes&quot;}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de cliques]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

+++

### Público-alvo {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="População direcionada por push"
>abstract="O gráfico e a tabela **População direcionada** exibem dados relacionados ao público-alvo das mensagens por push, apresentando informações sobre mensagens a serem entregues e exclusões."

A variável **[!UICONTROL Público-alvo]** A tabela e o gráfico apresentam dados relacionados aos recipients para cada delivery de notificação por push enviado. As métricas estão detalhadas abaixo.

![](assets/global_report_push_targeted_audience.png){zoom=&quot;yes&quot;}

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Exclusão]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de entrega {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Estatísticas da entrega por push"
>abstract="O relatório **Estatísticas gerais** fornece informações sobre notificações por push enviadas, incluindo taxas de sucesso, erros e quarentenas."

A variável **[!UICONTROL Estatísticas de entrega]** A tabela detalha o sucesso de cada delivery de notificação por push. As métricas estão detalhadas abaixo.

![](assets/global_report_push_delivery_statistics.png){zoom=&quot;yes&quot;}

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Total de mensagens]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Rejeições]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (registro inválido, rejeição de mensagem, erro de carga, por exemplo). em relação ao número de mensagens a serem entregues.

  Os tipos de erro de notificações por push estão listados na variável [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Causas de exclusão {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Causas de exclusão de notificações por push"
>abstract="O gráfico e a tabela **Causas de exclusão** ilustram os diversos motivos que impediram os perfis de usuário de receber as notificações por push."

A variável **[!UICONTROL Causas de exclusão]** o gráfico e a tabela exibem os motivos que impediram os perfis de usuário, que foram excluídos dos perfis direcionados, de receber a mensagem.

Os tipos de erro de notificações por push estão listados na variável [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Taxa de transferência de entrega {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Relatório de taxa de transferência de entrega"
>abstract="O relatório de **Taxa de transferência de entrega** apresenta informações detalhadas sobre a taxa de transferência de entrega de notificações por push em toda a plataforma no período especificado."

![](assets/global_report_push_delivery_throughput.png){zoom=&quot;yes&quot;}

A variável **[!UICONTROL Taxa de transferência de entrega]** O relatório do oferece insights abrangentes sobre a eficácia do sistema de delivery de notificações por push, oferecendo um resumo detalhado das taxas de sucesso e erro por um período especificado.
