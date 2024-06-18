---
audience: end-user
title: Alertas de entrega
description: Saiba como trabalhar com alertas de delivery.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 2%

---

# Painéis de alertas de entrega {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Painéis de alertas de entrega"
>abstract="O Alertas de delivery é um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre suas execuções de delivery. Os painéis de alerta de delivery permitem especificar quem receberá alertas de email, escolher e configurar os critérios de alerta a serem usados para enviar esses alertas e acessar o histórico de todas as notificações enviadas."

Os painéis de alerta de delivery permitem especificar quem receberá alertas de email, escolher e configurar os critérios de alerta a serem usados para enviar esses alertas e acessar o histórico de todas as notificações enviadas. Elas podem ser acessados pelo **Alertas de entrega** no painel de navegação esquerdo, sob a guia **Painéis** guia.

![](assets/alerting-dashboard-list.png)

## Criar um painel de entrega {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Criar um painel de alerta de entrega"
>abstract="A criação de um painel de alerta de delivery permite especificar quem receberá alertas por email, escolher e configurar os critérios de alerta a serem usados para enviar esses alertas e acessar o histórico de todas as notificações enviadas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Parâmetros gerais de alertas de entrega"
>abstract="Especifique as propriedades gerais do painel de alerta de delivery. A variável **Selecionar grupo de alertas** permite especificar a variável **grupo de operadores** para receber os alertas enviados por esse painel."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Critérios de alertas de entrega"
>abstract="Nesta seção, adicione os critérios que deseja usar para enviar alertas a partir deste painel. Escolha entre critérios predefinidos ou crie seus próprios critérios para se alinhar às necessidades específicas."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Parâmetros de critérios"
>abstract="Os critérios têm valores de parâmetros padrão que definem como eles devem ser aplicados. É possível alterar esses valores para atender às suas necessidades nesta seção."

Para criar um painel de delivery, siga estas etapas:

1. Navegue até a **Alertas de entrega** no painel de navegação esquerdo e clique em **Criar painel de entrega**.

   ![](assets/alerting-dashboard.png)

1. Nomeie seu painel no campo **Rótulo** campo. A variável **Nome interno** O campo é preenchido automaticamente e é somente leitura.

1. No **Selecionar grupo de alertas** especifique o **grupo de operadores** para receber os alertas enviados por esse painel. Todos os membros do grupo de operadores selecionado receberão os alertas.

   Saiba mais sobre permissões e grupos de operadores no [Documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. No **Critérios de alerta de entrega** adicione os critérios que deseja utilizar para enviar alertas. Escolha entre critérios predefinidos ou crie seus próprios critérios para se alinhar às necessidades específicas. [Saiba como trabalhar com critérios](../msg/delivery-alerting-criteria.md)

1. Os critérios têm valores de parâmetros padrão que definem como eles devem ser aplicados. É possível alterar esses valores para atender às suas necessidades a partir da **Parâmetros de critérios** seção.

   ![](assets/alerting-criteria-parameters.png)

   Por exemplo, por padrão, a variável **Tamanho mínimo do público-alvo da entrega** o parâmetro criteria é definido como 50, o que significa que um delivery será incluído no alerta enviado por esse painel somente se for direcionado a pelo menos 50 perfis. Você pode alterar esse parâmetro se quiser incluir deliveries com menos de 50 perfis.

   Expanda a seção abaixo para obter mais informações sobre cada parâmetro de critério:

   +++Parâmetros de critérios disponíveis

   * **Tamanho mínimo do público-alvo da entrega**: por exemplo, se você inserir 100 neste campo, uma notificação será enviada somente para deliveries com um público alvo igual ou maior que 100 recipients. Esse parâmetro se aplica a todos os critérios.
   * **Período de monitoramento antes e depois da data de contato (em horas)**: Número de horas antes e depois da hora atual. Somente os deliveries com uma data de contato nesse intervalo de tempo são considerados. Esse parâmetro se aplica a todos os critérios. Por padrão, o valor desse campo é definido como 24 horas.
   * **Taxa máxima de erros de rejeição temporária**: uma notificação é enviada para todos os deliveries com uma taxa de erro de rejeição temporária maior que o valor especificado. Por padrão, o valor desse campo é definido como 0,05 (5%).
   * **Taxa máxima de erros de rejeição permanente**: uma notificação é enviada para todos os deliveries com uma taxa de erro de rejeição permanente maior que o valor especificado. Por padrão, o valor desse campo é definido como 0,05 (5%).
   * **Limite de tempo mínimo para entrega no status &quot;Início pendente&quot; (em minutos)**: uma notificação é enviada para todos os deliveries com status Start pending por mais tempo do que a duração especificada nesse campo, Start pending status significando que as mensagens ainda não foram consideradas pelo sistema.
   * **Tempo mínimo necessário para o cálculo da taxa de transferência (em minutos)**: somente os deliveries iniciados (com status In progress) por mais do que a duração especificada são considerados para os Deliveries com critério de baixa taxa de transferência.
   * **Porcentagem máxima de mensagens processadas para o cálculo da taxa de transferência**: somente deliveries com uma porcentagem de mensagens processadas inferior à porcentagem especificada são considerados para os Deliveries com critério de baixa taxa de transferência.
   * **Taxa de transferência mínima esperada (em mensagens enviadas por hora)**: somente deliveries com uma taxa de transferência inferior ao valor especificado são considerados para os Deliveries com critério de taxa de transferência baixa.
   * **Taxa mínima processada necessária para o critério &quot;Entregas em andamento&quot;**: somente os deliveries com uma porcentagem de mensagens processadas maior que a porcentagem especificada são considerados.

+++

1. Por padrão, os painéis de alerta são desativados, o que significa que os alertas de email vinculados a esse painel não são enviados. Para ativar o painel imediatamente, alterne a variável **Ativado** opção no **Geral** ao lado do campo de seleção do grupo de alertas.

   Você também pode salvar o painel e habilitá-lo posteriormente.

   ![](assets/alerting-dashboard-enable.png)

1. Para salvar o painel de alerta, clique no link **Salvar** botão.

O painel de alertas é aberto com dados em branco. Quando estiver pronto para ativá-lo e enviar notificações, clique no link **Configurações** e alterne o botão **Ativado** opção se ainda não tiver feito isso.

Agora, sempre que um delivery atender aos critérios definidos nesse painel, uma notificação de alerta será enviada para o grupo de operadores especificado.

## Gerenciar painéis de alerta

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Alertas de entrega enviados"
>abstract="Esta seção permite visualizar informações relacionadas aos alertas enviados mais recentes."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Histórico de alertas de entrega"
>abstract="A variável **Histórico** contém todos os alertas enviados deste painel. Clique em um item para acessar os alertas correspondentes enviados naquele momento específico."

Todos os painéis de alertas criados podem ser acessados no **Alertas de entrega** no menu, no **Painéis** guia.

![](assets/alerting-dashboard-list.png)

É possível duplicar ou excluir um painel de controle usando o **Mais ações** localizado ao lado do seu nome.

Para acessar uma exibição detalhada de um painel, clique no nome na lista. Nesta tela, você pode visualizar o alerta enviado mais recente. Todos os alertas enviados são listados no painel esquerdo. Clique em um item para acessar os alertas correspondentes enviados naquele momento específico.

![](assets/alerting-dashboard-details.png)

Para editar o painel, clique no link **Configurações** no canto superior direito e faça as alterações desejadas.
