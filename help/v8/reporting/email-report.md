---
audience: end-user
title: Relatórios de entrega de email
description: Saiba como acessar e usar relatórios do delivery de email
badge: label="Beta"
source-git-commit: bd7d478d76c04d7dd644514ab08641b9e797f715
workflow-type: tm+mt
source-wordcount: '2257'
ht-degree: 29%

---

# Relatório de entrega de emails {#email-report}

A variável **Relatório de entrega de email** O oferece insights e dados abrangentes específicos para o canal de email. Ele fornece informações detalhadas sobre o desempenho, a eficácia e os resultados de suas entregas individuais, fornecendo uma visão geral abrangente.

## Resumo da entrega {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Envio de relatório"
>abstract="he **Enviando** A guia no relatório fornece insights detalhados sobre as interações dos visitantes com os deliveries e quaisquer erros em potencial que possam ter encontrado."

### População do público-alvo inicial  {#email-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="População do público-alvo inicial "
>abstract="A variável **População de público alvo inicial** O gráfico exibe dados relativos aos recipients e mensagens, com base nos resultados da preparação do delivery."

A variável **[!UICONTROL População de público alvo inicial]** O gráfico exibe dados relativos aos recipients. As métricas são calculadas durante a preparação do delivery e mostram: o público inicial, o número de mensagens a serem enviadas e o número de recipients excluídos.

![](assets/reporting_email_1.png){width="50%" align="left" zoomable="yes"}

Passe o mouse sobre uma parte do gráfico para exibir o número exato.

![](assets/reporting_email_1.1.png){width="50%" align="left" zoomable="yes"}


+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Público inicial]**: Número total de recipients alvos.

* **[!UICONTROL Para entregar]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Exclusão]**: número total de recipients excluídos da população do target.
+++

### Estatísticas de entrega {#email-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Estatísticas de entrega"
>abstract="A variável **Estatísticas de entrega** O gráfico detalha o sucesso do delivery e os erros que ocorreram."


A variável **[!UICONTROL Estatísticas de entrega]** O gráfico detalha o sucesso do seu delivery. As métricas estão detalhadas abaixo.

![](assets/reporting_email_2.png){width="50%" align="left" zoomable="yes"}

+++Saiba mais sobre Métricas de relatório da campanha de email.

* **[!UICONTROL Mensagem enviada]**: Número total de mensagens a serem entregues após a preparação do delivery.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros]**: Número total de erros acumulados durante os deliveries e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novos em quarentena]**: Número total de endereços colocados em quarentena após um delivery com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

+++

### Causas de exclusão  {#email-delivery-exclusions}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Estatísticas de entrega"
>abstract="A variável **Causas de exclusão** o gráfico e a tabela mostram o detalhamento por regra de mensagens rejeitadas durante a preparação do delivery."


A variável **[!UICONTROL Causas de exclusão]** o gráfico e a tabela mostram o detalhamento por regra de mensagens rejeitadas durante a preparação do delivery. As regras de exclusão são detalhadas na seção [Documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){_blank}.

![](assets/reporting_email_3.png){align="center" zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL User unknown]** : Tipo de erro gerado durante o delivery para indicar que o endereço de email é inválido.

* **[!UICONTROL invalid domain]** : Tipo de erro gerado ao enviar um delivery para indicar que o domínio do endereço de email está errado ou não existe.

* **[!UICONTROL Caixa de entrada cheia]**: Tipo de erro gerado após cinco tentativas de delivery para indicar que a caixa de entrada dos recipients contém muitas mensagens.

* **[!UICONTROL Account disabled]** : Tipo de erro gerado ao enviar um delivery para indicar que o endereço não existe mais.

* **[!UICONTROL Recusado]**: Tipo de erro gerado quando um endereço é rejeitado pelo IAP (Provedor de Acesso à Internet), por exemplo, ao seguir uma regra de segurança da aplicação (software antispam).

* **[!UICONTROL Unreachable]** : Tipo de erro que ocorre na string de distribuição de mensagens: incidente na retransmissão SMTP, domínio temporariamente inacessível, etc

* **[!UICONTROL Not connected]** : Tipo de erro para indicar que o celular do recipient está desligado ou sem rede no momento do envio.

+++

## Taxa de transferência de delivery {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Widget de taxa de transferência de entrega"
>abstract="A variável **Taxa de transferência de entrega** O relatório do apresenta informações detalhadas sobre a taxa de transferência de delivery de toda a plataforma em um período especificado."

Este relatório apresenta informações detalhadas sobre a taxa de transferência de delivery de toda a plataforma em um período especificado. A métrica primária usada para medir a velocidade de entrega de mensagens é o número de mensagens enviadas por hora.

![](assets/reporting_email_3.1.png){align="center" zoomable="yes"}


## Estatísticas de transmissão {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Widget de estatísticas de transmissão"
>abstract="A variável **Estatísticas de transmissão** O relatório de contém os dados disponíveis para possíveis erros encontrados com cada domínio."

A variável **[!UICONTROL Estatísticas de transmissão]** A tabela contém os dados disponíveis para possíveis erros encontrados com cada domínio. As métricas estão detalhadas abaixo.

![](assets/reporting_email_4.png){align="center" zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Emails processados]**: número total de mensagens processadas pelo servidor de delivery.

* **[!UICONTROL Entregue]**: Porcentagem do número de mensagens processadas com êxito em comparação ao número total de mensagens processadas.

* **[!UICONTROL Devoluções permanentes]**: porcentagem do número de devoluções permanentes, erros permanentes, como um endereço de email errado, em comparação ao número total de mensagens processadas.

* **[!UICONTROL Rejeições temporárias]**: Porcentagem do número de devoluções temporárias, como uma caixa de entrada cheia, em comparação ao número total de mensagens processadas

* **[!UICONTROL Aberturas]**: Porcentagem do número de recipients alvos que abriram uma mensagem pelo menos uma vez em comparação ao número de mensagens processadas com êxito.

* **[!UICONTROL Cliques]**: Porcentagem do número de pessoas que clicaram em um delivery pelo menos uma vez em comparação ao número de mensagens processadas com êxito.

* **[!UICONTROL Cancelamentos de assinatura]**: Porcentagem do número de cliques em um link de cancelamento de subscrição em comparação ao número de mensagens processadas com êxito.
+++

## Não entregues {#non-deliverables-email}

### Detalhamento dos erros por tipo {#email-delivery-breakdown-type}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Detalhamento dos erros por tipo"
>abstract="A variável **Detalhamento de erros por tipo** a tabela e o gráfico contêm os dados disponíveis para cada tipo de erro encontrado: usuário desconhecido, caixa de correio cheia, domínio inválido e muito mais."

A variável **[!UICONTROL Detalhamento de erros por tipo]** a tabela e o gráfico contêm os dados disponíveis para o tipo de erro. As métricas estão detalhadas abaixo.

Os erros exibidos nesse relatório acionam o processo de quarentena. Para obter mais informações sobre gestão de quarentena, consulte [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=pt-BR){target="_blank"}.

![](assets/campaign_report_email_6.png){align="left" zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL User unknown]** : Tipo de erro gerado durante o delivery para indicar que o endereço de email é inválido.

* **[!UICONTROL invalid domain]** : Tipo de erro gerado ao enviar um delivery para indicar que o domínio do endereço de email está errado ou não existe.

* **[!UICONTROL Caixa de entrada cheia]**: Tipo de erro gerado após cinco tentativas de delivery para indicar que a caixa de entrada dos recipients contém muitas mensagens.

* **[!UICONTROL Account disabled]** : Tipo de erro gerado ao enviar um delivery para indicar que o endereço não existe mais.

* **[!UICONTROL Recusado]**: Tipo de erro gerado quando um endereço é rejeitado pelo IAP (Provedor de Acesso à Internet), por exemplo, ao seguir uma regra de segurança da aplicação (software antispam).

* **[!UICONTROL Unreachable]** : Tipo de erro que ocorre na string de distribuição de mensagens: incidente na retransmissão SMTP, domínio temporariamente inacessível, etc

* **[!UICONTROL Not connected]** : Tipo de erro para indicar que o celular do recipient está desligado ou sem rede no momento do envio.

+++


### Detalhamento de erros por domínio {#email-delivery-breakdown-domain}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Detalhamento de erros por domínio"
>abstract="A variável **Detalhamento de erros por domínio** A tabela e o gráfico exibem os dados disponíveis para cada tipo de erro encontrado, dependendo de cada domínio."


A variável **[!UICONTROL Detalhamento de erros por domínio]** A tabela e o gráfico exibem os dados disponíveis para possíveis erros encontrados com cada domínio.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

Clique no ícone ao lado do nome de cada domínio para ver os detalhes.

![](assets/campaign_report_email_6.1.png){align="left" zoomable="yes"}

As métricas disponíveis são as mesmas que para o [Detalhamento por tipo de erro](#email-delivery-breakdown-type) acima descritas.

## Indicadores de rastreamento {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Rastreamento de relatórios"
>abstract="A variável **Rastreamento** A guia no relatório oferece dados valiosos, incluindo o comportamento do recipient por link, o detalhamento de aberturas e cliques, bem como informações detalhadas sobre os URLs clicados com mais frequência durante um delivery."


### Estatísticas de entrega  {#email-tracking-delivery-stats}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Estatísticas de entrega"
>abstract="A variável **Estatísticas de entrega** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre os dados disponíveis para emails enviados: sucesso, aberturas, cliques e muito mais."


A variável **[!UICONTROL Estatísticas de entrega]** O relatório do fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre os dados disponíveis para emails enviados. As métricas estão detalhadas abaixo.

![](assets/reporting_email_5.png){align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Sucesso]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Aberturas distintas]**: número total de recipients alvos que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Opens]**: Número de recipients alvos distintos para este domínio que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Cliques no link para opção de não participação]**: Número de cliques no link unsubscription.

* **[!UICONTROL Clicks on the mirror link]**: Número de cliques no link para a mirror page.

* **[!UICONTROL Estimation of forwards]**: Estimativa do número de emails encaminhados pelos recipients alvos.
+++

### Índice de abertura e click-through {#email-tracking-click-through}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Widget de taxa de abertura e click-through"
>abstract="A variável **Índice de click-through e aberturas** A tabela exibe dados relativos ao envolvimento dos recipients com a entrega."



A variável **[!UICONTROL Índice de click-through e aberturas]** A tabela exibe dados relativos aos recipients. As métricas estão detalhadas abaixo.

![](assets/reporting_email_6.png){align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Enviado]**: Número total de mensagens enviadas.

* **[!UICONTROL Complaints]**: Número de mensagens deste domínio relatadas como indesejáveis pelo recipient.

* **[!UICONTROL Opens]**: Número de recipients alvos distintos para este domínio que abriram uma mensagem pelo menos uma vez.

* **[!UICONTROL Clicks]**: Número de recipients alvos distintos que clicaram no mesmo delivery pelo menos uma vez.

* **[!UICONTROL Raw reactivity]**: Porcentagem do número de recipients que clicaram em um delivery pelo menos uma vez em comparação ao número de recipients que abriram um delivery pelo menos uma vez.
+++

## Fluxos de clique e URLs {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="Fluxos de clique e URLs"
>abstract="A variável **Fluxos de clique e URLs** O relatório de fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre os URLs que foram mais clicados durante um delivery."


A variável **[!UICONTROL Fluxos de clique e URLs]** O relatório de fornece indicadores principais de desempenho (KPIs) que fornecem informações detalhadas sobre os URLs que foram mais clicados durante um delivery.

![](assets/reporting_email_7.png){align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Reactivity]**: Taxa do número de recipients alvos que clicaram em um delivery em relação ao número estimado de recipients alvos que abriram um delivery.

* **[!UICONTROL Cliques distintos]**: Número total de recipients distintos que clicaram em um delivery pelo menos uma vez.

* **[!UICONTROL Clicks]** : Número total de cliques nos links nos deliveries.

* **[!UICONTROL Platform average]**: Essa taxa média, exibida em cada taxa (reatividade, cliques distintos e cliques acumulados), é calculada para deliveries enviados nos seis meses anteriores. Somente os deliveries com a mesma tipologia e no mesmo canal são considerados. Provas são excluídas.

+++

### Os 10 links mais visitados {#email-tracking-top10}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_top10"
>title="Os 10 links mais visitados"
>abstract="A variável **Os 10 links mais visitados** gráfico e tabela contêm os dados disponíveis para o comportamento do recipient por link."


A variável **[!UICONTROL Os 10 links mais visitados]** o gráfico e a tabela contêm os dados disponíveis para o comportamento do recipient por link.

![](assets/reporting_email_8.png){align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Clicks]** : Número total de cliques nos links nos deliveries.

* **[!UICONTROL Porcentagem]**: Porcentagem de usuários que interagiram com o delivery.

+++

### Detalhamento de cliques ao longo do tempo {#email-tracking-breakdown-over-time}


>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams_breakdown"
>title="Detalhamento de cliques ao longo do tempo"
>abstract="A variável **Detalhamento dos cliques ao longo do tempo** o gráfico mostra os dados disponíveis para o comportamento do recipient por link."


A variável **[!UICONTROL Detalhamento dos cliques ao longo do tempo]** o gráfico contém os dados disponíveis para o comportamento do recipient por link.

![](assets/reporting_email_9.png){align="center"}

## Atividades do usuário {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget de atividades do usuário"
>abstract="A variável **Atividades do usuário** o gráfico mostra o detalhamento de aberturas e cliques no formulário de um gráfico. Você pode escolher o período para direcionar dados: último dia ou hora ou 30 minutos."

A variável **[!UICONTROL Atividades do usuário]** O relatório mostra o detalhamento de aberturas e cliques no formulário de um gráfico. Você pode escolher o período para direcionar dados: último dia ou hora ou 30 minutos.

![](assets/reporting_email_10.png){align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Clicks]** : Número total de cliques nos links nos deliveries.

* **[!UICONTROL Opens]**: Número de recipients alvos distintos para este domínio que abriram uma mensagem pelo menos uma vez.

+++

## Estatísticas de rastreamento {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widget de Estatísticas de rastreamento"
>abstract="A variável **Estatísticas de rastreamento** O gráfico fornece estatísticas sobre aberturas e cliques. Você tem a opção de selecionar o intervalo de tempo específico para direcionar dados."

A variável **[!UICONTROL Estatísticas de rastreamento]** O gráfico fornece estatísticas sobre aberturas e cliques. Você tem a opção de selecionar o intervalo de tempo específico para direcionar dados.

![](assets/reporting_email_11.png){align="center"}

+++Saiba mais sobre Métricas de relatório de delivery de email.

* **[!UICONTROL Clicks]** : Número total de cliques nos links nos deliveries.

* **[!UICONTROL Opens]**: Número de recipients alvos distintos para este domínio que abriram uma mensagem pelo menos uma vez.

+++

## Detalhamento de aberturas {#breakdown-opens}

### Detalhamento de aberturas por dispositivo {#breakdown-opens-devices}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Detalhamento por dispositivo"
>abstract="A variável **Detalhamento por dispositivo** O relatório mostra o detalhamento de aberturas por dispositivo para o período. Para cada categoria, dois gráficos são usados. O primeiro exibe estatísticas referentes a aberturas em um computador e dispositivos móveis. O segundo exibe o número exato e a porcentagem de cada tipo de dispositivo."

A variável **Detalhamento por dispositivo** Este relatório mostra o detalhamento de aberturas por dispositivo no período: computadores pessoais, dispositivos Android, dispositivos Apple ou outros.

Para cada categoria, dois gráficos são usados. O primeiro exibe estatísticas referentes a aberturas em um computador e dispositivos móveis. O segundo exibe o número exato e a porcentagem de cada tipo de dispositivo.

![](assets/reporting_email_13.png){align="center"}


### Detalhamento de aberturas por SO {#breakdown-opens-os}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Detalhamento por sistema operacional"
>abstract="A variável **Detalhamento por SO** mostra o detalhamento de aberturas por sistema operacional para o período relacionado. O primeiro gráfico exibe estatísticas referentes a aberturas em um computador e dispositivos móveis. O segundo exibe o número e a porcentagem exatos de cada SO."

A variável **Detalhamento por SO** Este relatório mostra o detalhamento de aberturas por sistema operacional para o período: sistemas Windows, sistemas Android, sistemas iOS ou outros.

Para cada categoria, dois gráficos são usados. O primeiro exibe estatísticas referentes a aberturas em um computador e sistemas operacionais móveis. O segundo exibe o número e a porcentagem exatos de cada sistema operacional.

![](assets/reporting_email_13.1.png){align="center"}

### Detalhamento de aberturas por navegador {#breakdown-opens-browser}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_browser"
>title="Detalhamento por navegador"
>abstract="A variável **Detalhamento por navegador** mostra o detalhamento de aberturas por navegador para o período. O primeiro gráfico exibe estatísticas referentes a aberturas em um computador e dispositivos móveis. O segundo exibe o número e a porcentagem exatos de cada navegador."

A variável **Detalhamento por navegador** Esse relatório mostra o detalhamento de aberturas por navegador: Chrome, Safari, Internet Explorer e muito mais.

Para cada categoria, dois gráficos são usados. O primeiro exibe estatísticas referentes a aberturas em um computador e sistemas operacionais móveis. O segundo exibe o número e a porcentagem exatos de cada navegador.

![](assets/reporting_email_13.2.png){align="center"}


## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Relatório de hotclicks"
>abstract="A variável **Hotclicks** report apresenta o conteúdo de email (HTML e/ou texto) com a porcentagem de cliques nos links, em cada link. Blocos de personalização, links de unsubscription, links de mirror pages e links de ofertas são considerados no total de cliques acumulados, mas não são exibidos no relatório."

Este relatório mostra o conteúdo da mensagem (HTML e/ou texto) com a porcentagem de cliques nos links, em cada link. Blocos de personalização, links de unsubscription, links de mirror pages e links de ofertas são considerados no total de cliques acumulados, mas não são exibidos no relatório.

![](assets/reporting11.png)
