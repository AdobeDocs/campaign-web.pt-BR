---
audience: end-user
title: Relatórios globais para o canal SMS
description: Entender os relatórios globais do canal SMS
badge: label="Disponibilidade limitada"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 4%

---

# Relatórios globais para o canal SMS {#campaign-reports-sms}

Os Relatórios globais fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até a **[!UICONTROL Relatórios]** no menu **[!UICONTROL Relatórios]** seção. Você pode filtrar seus dados dependendo da data do relatório, pasta ou regras. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-sms}

### Visão geral da entrega {#delivery-overview-sms}

A variável **[!UICONTROL Visão geral da entrega]** O relatório do oferece indicadores principais de desempenho (KPIs) abrangentes que fornecem insights detalhados sobre os padrões de interação de seus visitantes com cada delivery de SMS. As métricas a seguir são descritas abaixo.

![](assets/global_report_sms_delivery_overview.png)

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Porcentagem de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Taxa de cliques]**: Porcentagem de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Erros]**: Porcentagem de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

+++

### Público-alvo {#delivery-summary-sms-initial-target}

A variável **[!UICONTROL Público-alvo]** A tabela e o gráfico apresentam dados relacionados aos seus recipients para cada delivery de SMS enviado. As métricas estão detalhadas abaixo.

![](assets/global_report_sms_targeted_audience.png)

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Exclusão]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de entrega {#delivery-summary-sms-exec-stats}

A variável **[!UICONTROL Estatísticas de entrega]** A tabela detalha o sucesso de cada delivery de SMS. As métricas estão detalhadas abaixo.

![](assets/global_report_sms_delivery_statistics.png)

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Total de mensagens]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Rejeições]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

  Os tipos de erro de SMS estão listados no [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causas de exclusão {#causes-exclusion}

A variável **[!UICONTROL Causas de exclusão]** O gráfico e a tabela exibem os motivos que impediram os perfis de usuário, que foram excluídos dos perfis direcionados, de receber seus deliveries de SMS.

Os tipos de erro estão listados no [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Taxa de transferência de entrega {#delivery-throughput-sms}

![](assets/global_report_sms_delivery_throughput.png)

Este relatório fornece detalhes abrangentes sobre a taxa de transferência do delivery em um período especificado.
