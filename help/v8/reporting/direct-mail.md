---
audience: end-user
title: Relatórios de correspondência direta
description: Saiba como acessar e usar relatórios de correspondência direta
exl-id: 268fe1e3-bd5c-40f1-8973-7671cd8c9960
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 20%

---

# Relatório de entrega de correspondência direta {#direct-mail-report}

O **Relatório de entrega por correspondência direta** fornece informações e dados abrangentes específicos sobre sua entrega por correspondência direta. Ele inclui informações detalhadas sobre o desempenho, a eficácia e os resultados de deliveries individuais, oferecendo uma visão geral completa.

## Resumo da entrega {#delivery-summary-direct-mail}

### Visão geral da entrega {#delivery-overview-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_overview_direct_mail"
>title="Visão geral da entrega"
>abstract="A **Visão geral da entrega** apresenta métricas principais de desempenho (KPIs) com informações detalhadas sobre as interações de visitantes com cada entrega de correspondência direta. As métricas estão descritas abaixo."

A **[!UICONTROL Visão geral da entrega]** fornece insights detalhados sobre as interações do visitante com cada entrega de correspondência direta, mostrando métricas essenciais de desempenho (KPIs). As métricas estão descritas abaixo.

![Gráfico de métricas de visão geral da entrega mostrando os principais indicadores de desempenho para entrega de correspondência direta.](assets/direct-overview.png){zoomable="yes"}{align="center"}

+++Saiba mais sobre Métricas de visão geral de delivery.

* **[!UICONTROL Mensagens a serem entregues]**: número total de mensagens processadas durante a preparação da entrega.
* **[!UICONTROL Direcionado]**: número de perfis de usuário qualificados como perfis de destino para mensagens de correspondência direta.
* **[!UICONTROL A excluir]**: número de perfis de usuário excluídos dos perfis direcionados que não receberão mensagens de correspondência direta.
+++

### População inicial de público-alvo {#direct-mail-delivery-targeted-population}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target_direct_mail"
>title="População inicial de público-alvo"
>abstract="O gráfico **População inicial de público-alvo** exibe dados relativos a destinatários e mensagens, com base nos resultados da preparação da entrega."

O gráfico **[!UICONTROL População inicial do destino]** exibe os dados relacionados aos destinatários. As métricas são calculadas durante a preparação do delivery e incluem o público inicial, o número de mensagens a serem enviadas e o número de recipients excluídos.

![Gráfico de população de destino inicial mostrando o tamanho do público-alvo, mensagens a serem enviadas e exclusões.](assets/direct-mail-delivery-targeted-population.png){zoomable="yes"}

Passe o mouse sobre uma parte do gráfico para exibir o número exato.

![Exibição detalhada do gráfico de população de destino inicial com funcionalidade de focalização.](assets/direct-mail-delivery-targeted-population_2.png){zoomable="yes"}

+++Saiba mais sobre Métricas de relatório de delivery de correspondência direta.

* **[!UICONTROL Público-alvo inicial]**: número total de destinatários direcionados.
* **[!UICONTROL Para entregar]**: Número total de mensagens a serem entregues após a preparação da entrega.
* **[!UICONTROL Exclusão]**: número total de destinatários excluídos da população do público-alvo.
+++

### Estatísticas de entrega {#direct-mail-delivery-stats}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary_direct_mail"
>title="Estatísticas de entrega"
>abstract="O gráfico **Estatísticas de entrega** detalha o sucesso da entrega de correspondência direta e os erros que ocorreram."

O gráfico **[!UICONTROL Estatísticas de entrega]** fornece uma visão geral do desempenho de entrega, oferecendo métricas detalhadas para medir o sucesso e a eficácia.

![Gráfico de estatísticas de entrega mostrando taxas de sucesso, erros e quarentenas.](assets/direct-mail-delivery-stats.png){zoomable="yes"}

+++Saiba mais sobre as métricas de relatório da campanha de correspondência direta.

* **[!UICONTROL Mensagem enviada]**: Número total de mensagens a serem entregues após a preparação da entrega.
* **[!UICONTROL Êxito]**: número de mensagens processadas com êxito em comparação ao número de mensagens a serem entregues.
* **[!UICONTROL Erros]**: Número total de erros acumulados durante as entregas e o processamento automático de reassociação em comparação ao número de mensagens a serem entregues.
* **[!UICONTROL Novas quarentenas]**: Número total de endereços colocados em quarentena após a entrega com falha (por exemplo, usuário desconhecido, domínio inválido) em comparação ao número de mensagens a serem entregues.
+++

### Causas da exclusão {#direct-mail-delivery-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_causes_exclusion_direct_mail"
>title="Causas de exclusão de entrega"
>abstract="O gráfico **Causas de exclusão** ilustra a distribuição de mensagens rejeitadas durante a preparação para a entrega, categorizada por cada regra."

O gráfico **[!UICONTROL Causas da exclusão]** fornece uma análise dos motivos da rejeição da mensagem durante a preparação da entrega. Esse detalhamento é organizado por várias regras, oferecendo uma visualização detalhada dos fatores que contribuem para a exclusão de mensagens. As regras de exclusão são detalhadas na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=pt-BR#email-error-types){_blank}.

![Gráfico de causas de exclusão mostrando a distribuição de mensagens rejeitadas por regra.](assets/direct-mail-delivery-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

+++Saiba mais sobre Causas de métricas de exclusão.

* **[!UICONTROL Endereço em quarentena]**: Tipo de erro gerado quando um endereço é colocado em quarentena.
* **[!UICONTROL Endereço não especificado]**: Tipo de erro gerado quando um endereço não existe.
* **[!UICONTROL Endereço de má qualidade]**: Tipo de erro gerado quando a classificação de qualidade do endereço postal é muito baixa.
* incluir na lista de bloqueios incluir na lista de bloqueios **[!UICONTROL Endereço solicitado]**: Tipo de erro gerado quando o destinatário foi solicitado durante a entrega.
* **[!UICONTROL Duplo]**: Tipo de erro gerado quando o destinatário foi excluído devido a valores de chave não exclusivos.
* **[!UICONTROL Grupo de controle]**: o endereço do destinatário faz parte do grupo de controle.
* **[!UICONTROL Tamanho do público alvo limitado]**: o tamanho máximo de entrega foi atingido para o destinatário.
+++

### Exclusões {#direct-mail-exclusions}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusions_direct_mail"
>title="Exclusões"
>abstract="A tabela **[!UICONTROL Exclusões]** exibe um detalhamento por regra das mensagens que foram rejeitadas durante o processo de preparação da entrega."

A tabela **[!UICONTROL Exclusões]** fornece um detalhamento detalhado, categorizado por regras específicas, das mensagens rejeitadas durante a preparação da entrega. Essa divisão oferece uma compreensão clara dos motivos por trás das exclusões de mensagem.

![Tabela de exclusões mostrando o detalhamento das mensagens rejeitadas por regra.](assets/direct-mail-exclusions.png){zoomable="yes"}{align="center" zoomable="yes"}

As métricas disponíveis são as mesmas das [Causas de exclusão](#direct-mail-delivery-exclusions) descritas acima.