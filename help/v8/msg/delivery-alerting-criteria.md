---
audience: end-user
title: Alerta de entrega
description: Saiba como trabalhar com alertas de delivery.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 26%

---

# Critérios de alertas de entrega {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Painel de critérios de alertas de entrega"
>abstract="A interface do usuário do Campaign Web fornece critérios de alerta predefinidos (entregas com baixa taxa de transferência, entregas cuja preparação falhou...) que podem ser adicionados ao painel. Você também pode criar seus próprios critérios para atender às suas necessidades."

A interface da Web do Campaign fornece critérios de alerta predefinidos (entregas com baixa taxa de transferência, entregas cuja preparação falhou...) que podem ser adicionados ao painel. Você também pode criar seus próprios critérios para atender às suas necessidades.

Os critérios de alerta podem ser acessados no menu **Alertas de Entrega**, no painel de navegação esquerdo, na guia **Critérios**.

![](assets/alerting-criteria-list.png)

## Critérios de alerta predefinidos {#ootb-criteria}

Os critérios de alerta predefinidos estão disponíveis na interface da Web do Campaign. Estes critérios abrangem uma série de cenários, a seguir enumerados:

* **Falha nas entregas**: qualquer entrega agendada dentro de um intervalo definido, com um status incorreto.
* **Falha na entrega com preparação**: qualquer entrega modificada dentro de um intervalo definido, para a qual a etapa de preparação (cálculo de destino e geração de conteúdo) falhou.
* **Entrega com taxa de erro incorreta para rejeições temporárias**: qualquer entrega agendada dentro de um intervalo definido, com status pelo menos Em andamento, com uma taxa de erro de rejeição temporária maior que uma porcentagem definida.
* **Entrega com taxa de erro incorreta para rejeições permanentes**: qualquer entrega agendada dentro de um intervalo definido, com um status pelo menos Em andamento, com uma taxa de erro de rejeição permanente maior que uma porcentagem definida.
* **Entregas com início longo pendente**: qualquer entrega agendada dentro de um intervalo definido, com um status de Início pendente por mais tempo do que uma duração definida, status de Início pendente significando que as mensagens ainda não foram consideradas pelo sistema.
* **Entregas com baixa taxa de transferência**: qualquer entrega iniciada por mais de uma duração definida, com menos de uma porcentagem definida de mensagens processadas, com uma taxa de transferência inferior a um valor definido.
* **Entregas em andamento**: qualquer entrega agendada dentro de um intervalo definido, com o status Em andamento.

>[!NOTE]
>
>Os valores padrão são aplicados a todos os parâmetros para os critérios acima. Esses valores podem ser personalizados na seção **Parâmetros de critério** dos painéis de alerta de entrega onde estão sendo usados. [Saiba como trabalhar com painéis](../msg/delivery-alerting-dashboards.md)

## Criar um critério de alerta {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Criar critérios de alertas de entrega"
>abstract="Além dos critérios de alerta predefinidos fornecidos pelo Adobe Campaign, você pode criar seus próprios critérios para atender às suas necessidades."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicadores para adicionar em alertas"
>abstract="Selecione os indicadores a serem exibidos como colunas na seção “Detalhes” dos alertas de email."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Tipo de alerta"
>abstract="Especifique o **Tipo de alerta** para o critério, ou seja, o rótulo e a cor a serem exibidos ao lado do critério de entrega na seção “Resumo” dos alertas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Frequência do critério"
>abstract="Controle a frequência de alertas por dia para cada entrega que atende ao critério."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Criar um critério de alerta"
>abstract="Para criar filtros de entrega, crie um novo filtro predefinido no console do Campaign v8 pelo nó **Administração** > **Configuração** > **Filtros Predefinidos**."

Para criar um novo critério, siga estas etapas:

1. Navegue até o menu **Delivery Àlerting** no painel de navegação esquerdo e selecione a guia **Critérios**.
1. Clique no botão **Criar critérios de alerta de entrega**.
1. Forneça um rótulo para o critério. O nome interno é preenchido automaticamente e é somente leitura.
1. O **Filtro de entrega aplicado por este critério** permite refinar o escopo do critério, aplicando um filtro predefinido a ele.

   No exemplo abaixo, o filtro **Deliveries em andamento (critInProgressDeliveries)** foi selecionado, o que significa que o critério só considera deliveries com o status &quot;Em andamento&quot;.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Se nenhum dos filtros predefinidos atender às suas necessidades, entre em contato com o administrador para criar seu próprio filtro.  Informações detalhadas sobre como criar filtros predefinidos no console do Campaign estão disponíveis na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Esta operação deve ser executada somente por usuários avançados.

1. Na seção **Indicators to add in alerts**, escolha os indicadores a serem exibidos como colunas na seção &quot;Details&quot; dos alertas de email.

1. Especifique o **Tipo de alerta** para o critério, ou seja, o rótulo e a cor a serem exibidos ao lado do critério de entrega na seção “Resumo” dos alertas.

1. A seção **Frequência de Critérios** permite controlar a frequência de alertas por dia para cada entrega que atenda ao critério:

   * **Este critério de entrega será repetido em cada notificação**: exiba uma entrega que atenda ao critério em cada alerta por email do dia.
   * **Este critério de entrega é enviado somente na primeira ocorrência do dia**: exibir uma entrega que atenda ao critério somente no primeiro relatório do dia, não repetido em alertas de email subsequentes.
