---
audience: end-user
title: Relatórios globais para o canal de correspondência direta
description: Saiba mais sobre Relatórios globais para o canal de correspondência direta
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: 98a0ce67682f8e1ab412be91b5af01e35c638f99
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 32%

---

# Relatórios globais para o canal de correspondência direta {#global-report-direct}

Os relatórios globais de correspondência direta fornecem aos usuários uma visão geral abrangente das métricas de tráfego e engajamento no nível do canal.

Navegue até o menu **[!UICONTROL Relatórios]** na seção **[!UICONTROL Relatórios]**. Você pode filtrar seus dados dependendo da data do relatório, pasta ou regras. [Saiba mais](global-reports.md)

## Resumo da entrega {#delivery-summary-direct}

### Visão geral da entrega {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Visão geral da entrega"
>abstract="A **Visão geral da entrega** apresenta métricas principais de desempenho (KPIs) com informações detalhadas sobre as interações de visitantes com cada entrega de correspondência direta. As métricas estão descritas abaixo."

A **[!UICONTROL Visão geral da entrega]** apresenta métricas principais de desempenho (KPIs) com informações detalhadas sobre as interações de visitantes com cada entrega de correspondência direta. As métricas estão descritas abaixo.

![](assets/global_report_direct_mail_delivery_overview.png){zoomable="yes"}{align="center"}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a serem entregues]**: número total de mensagens processadas durante a preparação da entrega.

* **[!UICONTROL Entregues]**: número de mensagens enviadas com êxito em relação ao número total de mensagens enviadas.

* **[!UICONTROL Erros]**: Total de erros acumulados durante o processamento de entrega e retorno automático em relação ao número total de mensagens enviadas.

* **[!UICONTROL Cancelamentos de assinatura]**: número de destinatários que clicaram em cancelar assinatura.
+++

### Público-alvo {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="Público-alvo"
>abstract="Os dados de destinatários e as informações da mensagem são exibidos no gráfico **Público-alvo**, refletindo a análise de preparação da entrega."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="Público-alvo"
>abstract="A tabela **Público-alvo** fornece um detalhamento dos destinatários e das mensagens correspondentes, com base nos resultados do processo de preparação da entrega."

A tabela e o gráfico para **[!UICONTROL Público-alvo]** exibem dados relacionados aos seus destinatários, com as métricas detalhadas fornecidas abaixo.

![](assets/global_report_direct_mail_targeted_audience.png){zoomable="yes"}{align="center"}

+++Saiba mais sobre métricas de Público-alvo direcionado.

* **[!UICONTROL Público-alvo]**: número total de destinatários direcionados.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* **[!UICONTROL Exclusão]**: número total de endereços ignorados durante a análise ao aplicar regras: endereço em quarentena, em, em inclui na lista de bloqueios, etc.

+++

### Estatísticas de entrega {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="Estatísticas de entrega"
>abstract="O gráfico **Estatísticas de entrega** fornece informações sobre a eficácia das entregas de correspondência direta, incluindo entregas bem-sucedidas e erros encontrados."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="Estatísticas de entrega"
>abstract="A tabela **Estatísticas de entrega** detalha o sucesso da entrega de correspondência direta e os erros que ocorreram."

O gráfico e a tabela **[!UICONTROL Estatísticas de entrega]** fornecem um detalhamento do sucesso de cada entrega de correspondência direta, com métricas detalhadas descritas abaixo.

+++Saiba mais sobre Estatísticas de entrega.

* **[!UICONTROL Mensagem a ser entregue]**: Número total de mensagens a serem entregues após a preparação da entrega.

* **[!UICONTROL Success]**: Número de mensagens processadas com êxito em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Erros / Devoluções]**: Número total de erros acumulados durante as entregas e o processamento automático de reassociação em relação ao número de mensagens a serem entregues.

* **[!UICONTROL Novas quarentenas]**: Número total de endereços colocados em quarentena após uma entrega com falha (usuário desconhecido, domínio inválido) em relação ao número de mensagens a serem entregues.

+++

### Causas da exclusão {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Exclusões"
>abstract="A tabela **Causas de exclusão** exibe um detalhamento por regra das mensagens que foram rejeitadas durante o processo de preparação da entrega."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Causas da exclusão"
>abstract="O gráfico **Causas de exclusão** ilustra a distribuição de mensagens rejeitadas durante a preparação para a entrega, categorizada por cada regra."

![](assets/global_report_direct_mail_exclusions.png){zoomable="yes"}{align="center"}

O gráfico e a tabela de Exclusões ilustram os motivos que impediram os perfis de usuário, excluídos dos perfis direcionados, de receber a mensagem.

+++Saiba mais sobre Causas de métricas de exclusão.

* **[!UICONTROL Endereço em quarentena]**: Tipo de erro gerado quando o endereço é colocado em quarentena.

* **[!UICONTROL Endereço não especificado]**: Tipo de erro gerado ao enviar uma entrega para indicar que o endereço não existe.

* **[!UICONTROL Endereço de má qualidade]**: Tipo de erro gerado quando a classificação de qualidade do endereço postal é muito baixa.

* incluir na lista de bloqueios incluir na lista de bloqueios **[!UICONTROL Endereço solicitado]**: Tipo de erro gerado quando o destinatário foi solicitado quando a entrega foi realizada.

* **[!UICONTROL Duplo]**: Tipo de erro gerado quando o destinatário foi excluído porque seus valores de chaves não eram exclusivos.

* **[!UICONTROL Grupo de controle]**: o endereço do destinatário faz parte do grupo de controle.

* **[!UICONTROL Tamanho do público alvo limitado]**: o tamanho máximo de entrega foi atingido para o destinatário.

+++
