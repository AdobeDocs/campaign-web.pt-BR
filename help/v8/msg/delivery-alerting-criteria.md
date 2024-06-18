---
audience: end-user
title: Alertas de entrega
description: Saiba como trabalhar com alertas de delivery.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 7%

---

# Critérios de alertas de entrega {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Painel de critérios de alertas de entrega"
>abstract="A interface da Web do Campaign fornece critérios de alerta predefinidos (entregas com baixa taxa de transferência, entregas cuja preparação falhou...) que podem ser adicionados ao painel. Você também pode criar seus próprios critérios para atender às suas necessidades."

A interface da Web do Campaign fornece critérios de alerta predefinidos (entregas com baixa taxa de transferência, entregas cuja preparação falhou...) que podem ser adicionados ao painel. Você também pode criar seus próprios critérios para atender às suas necessidades.

Os critérios de alerta podem ser acessados no **Alertas de entrega** no painel de navegação esquerdo, sob a guia **Critérios** guia.

![](assets/alerting-criteria-list.png)

## Critérios de alerta predefinidos {#ootb-criteria}

Os critérios de alerta predefinidos estão disponíveis na interface da Web do Campaign. Estes critérios abrangem uma série de cenários, a seguir enumerados:

* **Falha nos deliveries**: qualquer delivery agendado dentro de uma faixa definida, com um status incorreto.
* **Falha nos deliveries com preparação**: qualquer delivery modificado dentro de um intervalo definido, para o qual a etapa de preparação (cálculo de target e geração de conteúdo) falhou.
* **Entrega com taxa de erro incorreta para rejeições temporárias**: qualquer delivery agendado dentro de um intervalo definido, com um status pelo menos Em andamento, com uma taxa de erro de rejeição temporária maior que uma porcentagem definida.
* **Entrega com taxa de erro ruim para rejeições permanentes**: qualquer delivery agendado dentro de um intervalo definido, com um status pelo menos Em andamento, com uma taxa de erro de rejeição permanente maior que uma porcentagem definida.
* **Entregas com início longo pendente**: Qualquer delivery agendado em um intervalo definido, com um status Start pending por mais de uma duração definida, Start pending status significa que as mensagens ainda não foram consideradas pelo sistema.
* **Entregas com baixa taxa de transferência**: qualquer delivery iniciado por mais do que uma duração definida, com menos do que uma porcentagem definida de mensagens processadas, com uma taxa de transferência inferior a um valor definido.
* **Entregas em andamento**: qualquer delivery agendado dentro de um intervalo definido, com o status In progress.

>[!NOTE]
>
>Os valores padrão são aplicados a todos os parâmetros para os critérios acima. Esses valores podem ser personalizados na variável **Parâmetros de critérios** seção dos painéis de alerta de delivery onde estão sendo usados. [Saiba como trabalhar com painéis](../msg/delivery-alerting-dashboards.md)

## Criar um critério de alerta {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Criar critérios de alertas de entrega"
>abstract="Além dos critérios de alerta predefinidos fornecidos pelo Adobe Campaign, você pode criar seus próprios critérios para atender às suas necessidades."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicadores para adicionar em alertas"
>abstract="Selecione os indicadores a serem exibidos como colunas na seção &quot;Detalhes&quot; dos alertas de email."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Tipo de alerta"
>abstract="Especifique a **Tipo de alerta** para o critério, o que significa o rótulo e a cor a serem exibidos ao lado do critério de delivery na seção &quot;Resumo&quot; dos alertas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frequência do critério"
>abstract="Controle a frequência de alertas por dia para cada delivery que atende ao critério."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Criar um critério de alerta"
>abstract="Para criar filtros de entrega, crie um novo filtro predefinido no console do Campaign v8 pelo nó **Administração** > **Configuração** > **Filtros Predefinidos**."

Para criar um novo critério, siga estas etapas:

1. Navegue até a **Alerta de entrega** no painel de navegação esquerdo e selecione a guia **Critérios** guia.
1. Clique em **Criar critérios de alerta de entrega** botão.
1. Forneça um rótulo para o critério. O nome interno é preenchido automaticamente e é somente leitura.
1. A variável **Filtro de entrega aplicado por este critério** permite refinar o escopo do critério aplicando um filtro predefinido a ele.

   No exemplo abaixo, a variável **Entregas em andamento (critInProgressDeliveries)** O filtro foi selecionado, o que significa que o critério considera apenas os deliveries com o status &quot;Em andamento&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Se nenhum dos filtros predefinidos atender às suas necessidades, entre em contato com o administrador para criar seu próprio filtro.  Informações detalhadas sobre como criar filtros predefinidos no console do Campaign estão disponíveis na [Documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Esta operação deve ser executada somente por usuários avançados.

1. No **Indicadores para adicionar nos alertas** escolha os indicadores a serem exibidos como colunas na seção &quot;Detalhes&quot; dos alertas de email.

1. Especifique a **Tipo de alerta** para o critério, o que significa o rótulo e a cor a serem exibidos ao lado do critério de delivery na seção &quot;Resumo&quot; dos alertas.

1. A variável **Frequência dos critérios** permite controlar a frequência de alertas por dia para cada delivery que atenda ao critério:

   * **Este critério de entrega será repetido em cada notificação**: exiba um delivery que atenda ao critério em cada alerta de email do dia.
   * **Este critério de entrega é enviado somente na primeira ocorrência do dia**: exibe um delivery que atende ao critério somente no primeiro relatório do dia, não repetido em alertas de email subsequentes.
