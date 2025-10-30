---
audience: end-user
title: Relatórios de campanha para o canal de email
description: Saiba mais sobre os relatórios de campanha do canal de email
exl-id: c44c91f8-1f88-4087-8417-34be64a2ab19
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 22%

---

# Relatórios de campanha para o canal de email {#campaign-reports-email-channel}

Cada relatório de campanha é dividido em widgets diferentes detalhando o sucesso e os erros da campanha. Para o canal de email, os relatórios e as métricas são detalhados abaixo. Saiba como acessar seus relatórios de campanha em [esta página](campaign-reports.md).

## Resumo da entrega {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Visão geral da entrega"
>abstract="A **Visão geral da entrega** fornece indicadores principais de desempenho (KPIs) que contêm informações detalhadas sobre o engajamento de visitantes com a entrega de email."

### Visão geral da entrega {#delivery-summary-email-ovv}

O relatório **[!UICONTROL Visão geral da entrega]** fornece KPIs (indicadores-chave de desempenho) que fornecem informações detalhadas sobre como seus visitantes se envolvem com a entrega de email. As métricas estão detalhadas abaixo.

![Captura de tela do relatório de visão geral da entrega](assets/campaign_report_email_1.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Mensagens a serem entregues]**: número total de mensagens processadas durante a preparação da entrega.

* **[!UICONTROL Entregues]**: número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Rejeições]**: total de erros acumulados durante o processamento de entrega e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Total de aberturas]**: número total de recipients alvos que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Total de cliques]**: número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

+++

### Estatísticas iniciais do público-alvo {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Estatísticas iniciais do público-alvo"
>abstract="A tabela Estatísticas iniciais do público-alvo exibe os dados relativos aos destinatários."

A tabela **[!UICONTROL Estatísticas iniciais do público-alvo]** exibe os dados relativos aos seus destinatários. As métricas estão detalhadas abaixo.

![Captura de tela da tabela Estatísticas iniciais de público-alvo de destino](assets/campaign_report_email_2.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Público-alvo inicial]**: número total de destinatários direcionados.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* incluir na lista de bloqueios **[!UICONTROL Rejected by rules]**: Número total de endereços ignorados durante a análise ao aplicar regras: endereço em falta, em quarentena, no, etc.

+++

### Estatísticas de execução {#delivery-summary-email-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_exec_stats"
>title="Estatísticas de execução"
>abstract="A tabela **Estatísticas de execução** detalha o sucesso da entrega: mensagens a serem entregues, sucesso, erros e novas quarentenas."

A tabela **[!UICONTROL Estatísticas de execução]** detalha o sucesso da sua entrega. As métricas estão detalhadas abaixo.

![Captura de tela da tabela Estatísticas de execução detalhando o sucesso da entrega](assets/campaign_report_email_3.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* **[!UICONTROL Success]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros]**: Número total de erros acumulados durante as entregas e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novas quarentenas]**: Número total de endereços colocados em quarentena após uma entrega com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

  Tipos de erro de email listados na [documentação do Adobe Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=pt-BR#email-error-types){target="_blank"}.

+++

### Estatísticas de reação {#delivery-summary-email-reaction-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_reaction_stats"
>title="Estatísticas de reação"
>abstract="A tabela **Estatísticas de reação** mostra os dados disponíveis para a atividade do destinatário da sua entrega: número de aberturas, assinaturas, cancelamentos de assinatura, cliques no link da mirror page."

A tabela **[!UICONTROL Estatísticas de reação]** contém os dados disponíveis para a atividade de destinatário para a entrega. As métricas estão detalhadas abaixo.

![Captura de tela da tabela de estatísticas de Reação contendo os dados disponíveis para a atividade de destinatário para a entrega](assets/campaign_report_email_4.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Aberturas exclusivas]**: número total de destinatários direcionados que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Total de Aberturas]**: Número de destinatários direcionados distintos para este domínio que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Cancelar assinaturas]**: número de destinatários que clicaram em cancelar assinaturas para o período relacionado.

* **[!UICONTROL Mirror page]**: Número de destinatários que clicaram no link da mirror page.

* **[!UICONTROL Encaminhamentos]**: número de destinatários que clicaram e que encaminharam o email.
+++

### Fluxos de cliques gerados {#delivery-summary-email-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_click_streams"
>title="Fluxos de cliques gerados"
>abstract="A tabela **Fluxos de clique gerados** mostra os dados disponíveis relativos a como seus destinatários interagiram com a entrega."

A tabela **[!UICONTROL Fluxos de cliques gerados]** exibe dados relativos a como seus destinatários interagiram com sua entrega. As métricas estão detalhadas abaixo.

![Captura de tela da tabela de fluxos de clique gerados](assets/campaign_report_email_5.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Cliques únicos]**: número total de destinatários únicos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Total de Cliques]**: número total de cliques nos links nas entregas.

* **[!UICONTROL Reatividade]**: taxa do número de recipients alvos que clicaram em uma entrega em relação ao número estimado de recipients alvos que abriram uma entrega.

+++

## Não entregues {#non-deliverables-email}

### Detalhamento de erros por tipo {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_type"
>title="Detalhamento de erros por tipo"
>abstract="A tabela e o gráfico **Detalhamento de erros por tipo** contêm os dados disponíveis para cada tipo de erro encontrado: usuário desconhecido, caixa de entrada cheia, domínio inválido e muito mais."

A tabela e o gráfico **[!UICONTROL Breakdown of errors per type]** contêm os dados disponíveis para possíveis erros encontrados para cada tipo de domínio. As métricas estão detalhadas abaixo.

Os erros exibidos nesse relatório acionam o processo de quarentena. Para obter mais informações sobre o gerenciamento de quarentena, consulte a [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=pt-BR){target="_blank"}.

![Captura de tela do Detalhamento de erros por gráfico de tipo e tabela](assets/campaign_report_email_6.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Usuário desconhecido]**: Tipo de erro gerado durante a entrega para indicar que o endereço de email é inválido.

* **[!UICONTROL Domínio inválido]**: Tipo de erro gerado ao enviar uma entrega para indicar que o domínio do endereço de email está errado ou não existe.

* **[!UICONTROL Caixa de correio cheia]**: Tipo de erro gerado após cinco tentativas de entrega para indicar que a caixa de entrada dos destinatários contém muitas mensagens.

* **[!UICONTROL Conta desabilitada]**: Tipo de erro gerado ao enviar uma entrega para indicar que o endereço não existe mais.

* **[!UICONTROL Recusado]**: Tipo de erro gerado quando um endereço é rejeitado pelo IAP (Provedor de Acesso à Internet), por exemplo, ao seguir uma regra de segurança da aplicação (software antispam).

* **[!UICONTROL Inacessível]**: Tipo de erro que ocorre na cadeia de caracteres de distribuição de mensagens: incidente na retransmissão SMTP, domínio temporariamente inacessível, etc

* **[!UICONTROL Não conectado]**: Tipo de erro para indicar que o celular do recipient está desligado ou sem rede no momento do envio.

+++

### Detalhamento de erros por domínio {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_domain"
>title="Detalhamento de erros por domínio"
>abstract="A tabela e o gráfico **Detalhamento de erros por domínio** exibem os dados disponíveis para cada tipo de erro encontrado, dependendo de cada domínio."

A tabela e o gráfico **[!UICONTROL Breakdown of errors per domain]** contêm os dados disponíveis para possíveis erros encontrados em cada domínio. As métricas são comuns com a tabela e o gráfico **[!UICONTROL Breakdown of errors per type]** detalhados acima.

## Indicadores de rastreamento {#tracking-indicators-email}

### Estatísticas de entrega {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_delivery_statistics_summary"
>title="Estatísticas de entrega"
>abstract="O gráfico **Estatísticas de entrega** detalha o sucesso da entrega e os erros que ocorreram."

As métricas **[!UICONTROL Estatísticas de entrega]** fornecem KPIs (indicadores-chave de desempenho) que fornecem informações detalhadas sobre os dados disponíveis para emails enviados. As métricas estão detalhadas abaixo.

![Captura de tela das métricas de estatísticas de entrega](assets/campaign_report_email_7.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Mensagem(ns) a ser(em) entregue(s)]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Aberturas exclusivas]**: número total de destinatários direcionados que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Total de Aberturas]**: Número de destinatários direcionados distintos para este domínio que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Cliques no link para opção de não participação]**: Número de cliques no link para cancelamento de inscrição.

* **[!UICONTROL Clicks on the mirror link]**: Número de cliques no link para a mirror page.

* **[!UICONTROL Estimativa de encaminhamentos]**: Estimativa do número de emails encaminhados pelos destinatários direcionados.
+++

### Índice de abertura e click-through {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_open_clickthrough"
>title="Índice de abertura e click-through"
>abstract="A tabela **Índice de abertura e click through** exibe dados relativos ao engajamento dos recipients com a entrega."

A tabela **[!UICONTROL Taxa de abertura e de click-through]** exibe os dados relativos aos seus destinatários. As métricas estão detalhadas abaixo.

![Captura de tela da tabela de taxas de abertura e click-through](assets/campaign_report_email_8.png){zoomable="yes"}

+++ Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Enviado]**: Número total de mensagens enviadas.

* **[!UICONTROL Reclamações]**: número e porcentagem de mensagens deste domínio relatadas como indesejáveis pelo destinatário.

* **[!UICONTROL Aberturas Exclusivas]**: Número e porcentagem de destinatários direcionados distintos para este domínio que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Cliques únicos]**: número e porcentagem de recipients alvos distintos que clicaram no mesmo delivery pelo menos uma vez.

* **[!UICONTROL Reatividade bruta]**: porcentagem do número de recipients que clicaram em uma entrega pelo menos uma vez em comparação ao número de recipients que abriram uma entrega pelo menos uma vez.

+++

## Fluxos de clique e URLs {#url-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams"
>title="Fluxos de clique e URLs"
>abstract="O relatório **Fluxos de clique e URLs** fornece indicadores principais de desempenho (KPIs) com informações detalhadas sobre os URLs mais clicados durante uma entrega."

O relatório **[!UICONTROL URLs and click streams]** fornece KPIs (indicadores-chave de desempenho) que fornecem informações detalhadas sobre as URLs com mais cliques durante uma entrega. As métricas estão detalhadas abaixo.

![Captura de tela do relatório de fluxos de clique e URLs](assets/campaign_report_email_9.png){zoomable="yes"}

+++ Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Reatividade]**: taxa do número de recipients alvos que clicaram em uma entrega em relação ao número estimado de recipients alvos que abriram uma entrega.

* **[!UICONTROL Cliques únicos]**: número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Total de Cliques]**: número total de cliques nos links nas entregas.

* **[!UICONTROL Média da plataforma]**: essa taxa média, exibida em cada taxa (reatividade, cliques distintos e cliques acumulados), é calculada para deliveries enviados nos seis meses anteriores. Somente as entregas com a mesma tipologia e no mesmo canal são consideradas. Provas são excluídas.

+++

### Os 10 links mais visitados {#top10-campaign-report-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams_top10"
>title="Os 10 links mais visitados"
>abstract="O gráfico e a tabela **Os 10 links mais visitados** contêm os dados disponíveis relativos ao comportamento do destinatário em cada link."

O gráfico e a tabela **[!UICONTROL Os 10 links mais visitados]** contêm os dados disponíveis para o comportamento do recipient por link. As métricas estão detalhadas abaixo.

![Captura de tela do gráfico dos 10 links mais visitados](assets/campaign_report_email_10.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de campanha de email.

* **[!UICONTROL Cliques]**: número total de cliques nos links nas entregas.

* **[!UICONTROL Porcentagem]**: porcentagem de usuários que interagiram com a entrega.

+++

### Detalhamento dos cliques ao longo do tempo {#campaign-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_urls_click_breakdown"
>title="Detalhamento dos cliques ao longo do tempo"
>abstract="O gráfico **Detalhamento dos cliques ao longo do tempo** mostra os dados disponíveis relativos ao comportamento do recipient em cada link."

O gráfico **[!UICONTROL Breakdown of clicks over time]** contém os dados disponíveis para o comportamento do recipient por link.

![Captura de tela do Detalhamento dos cliques ao longo do gráfico de tempo](assets/campaign_report_email_11.png){zoomable="yes"}

## Atividades do usuário {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_user_activities"
>title="Atividades do usuário"
>abstract="O gráfico **Atividades do usuário** mostra o detalhamento de aberturas e cliques na forma de um gráfico."

O relatório **[!UICONTROL Atividades do usuário]** mostra o detalhamento de aberturas e cliques no formato de um gráfico. As métricas para esse relatório são detalhadas abaixo.

![Captura de tela do relatório de atividades do usuário](assets/campaign_report_email_user_activities.png){zoomable="yes"}{align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Cliques]**: número total de cliques nos links nas entregas.

* **[!UICONTROL Aberturas]**: Número de destinatários de destino distintos para este domínio que abriram uma mensagem pelo menos uma vez.

+++
