---
audience: end-user
title: Relatórios globais para o canal SMS
description: Entender relatórios globais do canal SMS
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '593'
ht-degree: 32%

---

# Relatórios globais para o canal SMS {#campaign-reports-sms}

Os relatórios globais fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até a **[!UICONTROL Relatórios]** no menu **[!UICONTROL Relatórios]** seção. Você pode filtrar seus dados dependendo da data do relatório, pasta ou regras. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-sms}

### Visão geral da entrega {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Visão geral da entrega de SMS"
>abstract="Os KPIs da **Visão geral da entrega de SMS** oferecem um resumo abrangente da entrega de SMS, com insights detalhados e dados específicos. Esses KPIs fornecem informações abrangentes sobre o desempenho, a eficácia e os resultados da entrega."

A variável **[!UICONTROL Visão geral da entrega]** O relatório do oferece indicadores principais de desempenho (KPIs) abrangentes que fornecem insights detalhados sobre os padrões de interação de seus visitantes com cada delivery de SMS. As métricas a seguir são descritas abaixo.

![](assets/global_report_sms_delivery_overview.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Porcentagem de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Taxa de cliques]**: Porcentagem de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Erros]**: Porcentagem de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

+++

### Público-alvo {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="População direcionada por SMS"
>abstract="O gráfico e a tabela **População direcionada** apresentam dados relacionados ao público-alvo de SMS, incluindo informações sobre mensagens a serem entregues e exclusões."

A variável **[!UICONTROL Público-alvo]** A tabela e o gráfico apresentam dados relacionados aos seus recipients para cada delivery de SMS enviado. As métricas estão detalhadas abaixo.

![](assets/global_report_sms_targeted_audience.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Exclusão]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de entrega {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Estatísticas da entrega de SMS"
>abstract="O relatório **Estatísticas de entrega** fornece insights abrangentes sobre o SMS enviado, oferecendo um detalhamento de várias métricas, como taxas de sucesso, ocorrências de erros e o público-alvo colocado em quarentena. Essa apresentação detalhada permite uma análise completa do desempenho geral e dos resultados do processo de entrega de SMS."

A variável **[!UICONTROL Estatísticas de entrega]** A tabela detalha o sucesso de cada delivery de SMS. As métricas estão detalhadas abaixo.

![](assets/global_report_sms_delivery_statistics.png){zoomable=&quot;yes&quot;}

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Total de mensagens]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Rejeições]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

  Os tipos de erro de SMS estão listados no [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Causas da exclusão {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Causas de exclusão de SMS"
>abstract="O gráfico e a tabela **Causas de exclusão** ilustram os diversos motivos que impediram os perfis de usuário de receber as mensagens SMS."

A variável **[!UICONTROL Causas de exclusão]** O gráfico e a tabela exibem os motivos que impediram os perfis de usuário, que foram excluídos dos perfis direcionados, de receber seus deliveries de SMS.

Os tipos de erro estão listados no [Documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png){zoomable=&quot;yes&quot;}

## Taxa de transferência de entrega {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Taxa de transferência de entrega de SMS"
>abstract="O relatório **Taxa de transferência de entrega** fornece insights abrangentes sobre a eficiência do sistema de entrega de mensagens SMS, com uma visão geral detalhada das taxas de sucesso e erros em um período especificado."

![](assets/global_report_sms_delivery_throughput.png){zoomable=&quot;yes&quot;}

A variável **[!UICONTROL Taxa de transferência de entrega]** O relatório do oferece insights abrangentes sobre a eficácia do sistema de delivery de mensagens SMS, oferecendo um resumo detalhado das taxas de sucesso e erro por um período especificado.
