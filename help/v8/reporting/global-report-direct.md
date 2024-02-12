---
audience: end-user
title: Relatórios globais para o canal de correspondência direta
description: Saiba mais sobre Relatórios globais para o canal de correspondência direta
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 5%

---

# Relatórios globais para o canal de correspondência direta {#global-report-direct}

Os Relatórios globais fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até a **[!UICONTROL Relatórios]** no menu **[!UICONTROL Relatórios]** seção. Você pode filtrar seus dados dependendo da data do relatório, pasta ou regras. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-direct}

### Visão geral da entrega {#delivery-overview-direct}

A variável **[!UICONTROL Visão geral da entrega]** O apresenta as principais métricas de desempenho (KPIs) com informações detalhadas sobre a interação de seus visitantes com cada delivery de email. As métricas estão descritas abaixo.

![](assets/global_report_email_delivery_overview.png){zoom=&quot;yes&quot;}{align="center"}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a entregar]**: Número total de mensagens processadas durante a preparação do delivery.

* **[!UICONTROL Entregue]**: Número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de delivery e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Cancelamentos de assinatura]**: Número de recipients que clicaram em unsubscriptions.
+++

### Público-alvo {#delivery-summary-direct-initial-target}

A tabela e o gráfico para **[!UICONTROL Público-alvo]** mostre dados relacionados aos seus recipients, com as métricas detalhadas fornecidas abaixo.

![](assets/global_report_email_targeted_audience.png){zoom=&quot;yes&quot;}{align="center"}

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: Número total de recipients alvos.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Exclusão]**: Número total de endereços ignorados durante a análise ao aplicar as regras: endereço em falta, em quarentena, na inclui na lista de bloqueios, etc.

+++

### Estatísticas de entrega {#delivery-summary-direct-exec-stats}

A variável **[!UICONTROL Estatísticas de entrega]** A tabela fornece um detalhamento do sucesso de cada delivery de correspondência direta, com métricas detalhadas descritas abaixo.

![](assets/global_report_email_delivery_statistics.png){zoom=&quot;yes&quot;}{align="center"}

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Rejeições]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

+++

### Causas de exclusão {#causes-exclusion}

![](assets/global_report_email_exclusions.png){zoom=&quot;yes&quot;}{align="center"}

O gráfico e a tabela de Exclusões ilustram os motivos que impediram os perfis de usuário, excluídos dos perfis direcionados, de receber a mensagem.

## Taxa de transferência de entrega {#delivery-throughput}

Este relatório fornece detalhes abrangentes sobre a taxa de transferência do delivery em um período especificado. A métrica principal usada para medir a velocidade de entrega de mensagens é o número de mensagens enviadas por hora.

## Não entregues {#non-deliverables-direct}

### Detalhamento de erros por tipo {#delivery-summary-direct-breakdown-per-type}

A variável **[!UICONTROL Detalhamento de erros por tipo]** A tabela e o gráfico apresentam os dados relacionados a possíveis erros ocorridos em vários domínios, com as métricas específicas fornecidas abaixo.

Os erros exibidos nesse relatório acionam o processo de quarentena. Para obter mais informações sobre gestão de quarentena, consulte [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++Saiba mais sobre Detalhamento de erros por tipo de métrica.

* **[!UICONTROL Usuário desconhecido]**: Tipo de erro gerado durante o delivery para indicar que o endereço é inválido.

* **[!UICONTROL Domínio inválido]**: Tipo de erro gerado ao enviar um delivery para indicar que o domínio do endereço está errado ou não existe.

* **[!UICONTROL Caixa de entrada cheia]**: Tipo de erro gerado após cinco tentativas de delivery para indicar que a caixa de entrada dos recipients contém muitas mensagens.

* **[!UICONTROL Conta desabilitada]**: Tipo de erro gerado ao enviar um delivery para indicar que o endereço não existe mais.

* **[!UICONTROL Recusado]**: Tipo de erro gerado quando um endereço é rejeitado pelo IAP (Provedor de Acesso à Internet), por exemplo, ao seguir uma regra de segurança da aplicação (software antispam).

* **[!UICONTROL Inacessível]**: Tipo de erro que ocorre na cadeia de caracteres de distribuição de mensagens: incidente na retransmissão SMTP, domínio temporariamente inacessível, etc

* **[!UICONTROL Não conectado]**: Tipo de erro para indicar que o celular do recipient está desligado ou sem rede no momento do envio.

+++

### Detalhamento de erros por domínio {#delivery-summary-email-breakdown-per-domain}

A variável **[!UICONTROL Detalhamento de erros por domínio]** A tabela e o gráfico mostram os dados relacionados a possíveis erros em cada domínio. As métricas são comuns com **[!UICONTROL Detalhamento de erros por tipo]** tabela e gráfico detalhados acima.

