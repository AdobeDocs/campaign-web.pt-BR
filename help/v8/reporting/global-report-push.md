---
audience: end-user
title: Relatórios globais para o canal de push
description: Entender os relatórios globais do canal de push
badge: label="Disponibilidade limitada"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 4%

---

# Relatórios globais para o canal de push {#campaign-reports-push}

Os Relatórios globais fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até a **[!UICONTROL Relatórios]** no menu **[!UICONTROL Relatórios]** seção. Você pode filtrar seus dados dependendo da data do relatório, pasta ou regras. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-push}

### Resumo da entrega {#delivery-overview-push}

A variável **[!UICONTROL Visão geral da entrega]** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre como seus visitantes se envolvem com cada delivery de notificação por push. As métricas estão detalhadas abaixo.

![](assets/global_report_push_delivery_overview.png)

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de cliques]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

+++

### Público-alvo {#delivery-summary-push-initial-target}

A variável **[!UICONTROL Público-alvo]** A tabela e o gráfico apresentam dados relacionados aos recipients para cada delivery de notificação por push enviado. As métricas estão detalhadas abaixo.

![](assets/global_report_push_targeted_audience.png)

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Exclusão]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de entrega {#delivery-summary-push-exec-stats}

A variável **[!UICONTROL Estatísticas de entrega]** A tabela detalha o sucesso de cada delivery de notificação por push. As métricas estão detalhadas abaixo.

![](assets/global_report_push_delivery_statistics.png)

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Total de mensagens]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Rejeições]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (registro inválido, rejeição de mensagem, erro de carga, por exemplo). em relação ao número de mensagens a serem entregues.

  Os tipos de erro de notificações por push estão listados na variável [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Causas de exclusão {#causes-exclusion}

A variável **[!UICONTROL Causas de exclusão]** o gráfico e a tabela exibem os motivos que impediram os perfis de usuário, que foram excluídos dos perfis direcionados, de receber a mensagem.

Os tipos de erro de notificações por push estão listados na variável [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Taxa de transferência de entrega {#delivery-throughput-sms}

![](assets/global_report_push_delivery_statistics.png)

Este relatório fornece detalhes abrangentes sobre a taxa de transferência do delivery em um período especificado.

