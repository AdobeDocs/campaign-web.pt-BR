---
audience: end-user
title: Trabalhar com serviços de assinatura
description: Saiba como acessar, criar e gerenciar serviços de assinatura na Web do Adobe Campaign
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: e82c19df7faecbb75521bca54e32b1ba84ea1f81
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 29%

---

# Criar e gerenciar serviços de assinatura {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Criar e gerenciar serviços"
>abstract="Use o Adobe Campaign para criar e monitorar serviços, como informativos, além de verificar as assinaturas ou o seu cancelamento. As assinaturas aplicam-se somente a entregas por email e SMS."

Use o Adobe Campaign Web para gerenciar e criar seus serviços, como boletins informativos, e para verificar as assinaturas ou cancelamentos de assinaturas desses serviços.

Vários serviços podem ser definidos em paralelo, por exemplo: boletins informativos para categorias de produtos, temas ou áreas específicas de um site, assinaturas para vários tipos de mensagens de alerta e notificações em tempo real.

>[!NOTE]
>
>As assinaturas aplicam-se somente a entregas por email e SMS.

## Acessar serviços de assinatura {#access-services}

Para acessar os serviços de assinatura disponíveis para sua plataforma, siga as etapas abaixo.

1. Navegue até o menu **[!UICONTROL Serviços de assinatura]** no painel de navegação esquerdo, em **[!UICONTROL Gerenciamento de clientes]**.

   ![Captura de tela mostrando o menu Subscription services no painel de navegação esquerdo em Gerenciamento de clientes](assets/service-list.png){zoomable="yes"}

1. A lista de todos os serviços de assinatura existentes é exibida. Você pode pesquisar os serviços e filtrar por canal, pasta ou adicionar regras usando o [modelador de consultas](../query/query-modeler-overview.md).

   ![Captura de tela mostrando a lista de serviços de assinatura com filtros para canal, pasta e regras](assets/service-filters.png){zoomable="yes"}

1. Para editar um serviço existente, clique em seu respectivo nome.

1. Exclua ou duplique qualquer serviço usando o ícone de três pontos ao lado do nome do serviço.<!--so all subscribers are unsubscribed - need to mention?-->

## Criar seu primeiro serviço de assinatura {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="Definir as propriedades do serviço"
>abstract="Insira o rótulo do serviço de assinatura e defina opções adicionais, como um período de validade para o seu serviço."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Selecione uma mensagem de confirmação"
>abstract="Quando um usuário(a) assina ou cancela a assinatura de um serviço, é possível enviar uma mensagem de confirmação. Selecione os modelos a serem usados nessas mensagens."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Página de destino padrão"
>abstract="Selecione as páginas de destino padrão associadas a este serviço."

Para criar um serviço de assinatura, siga as etapas abaixo.

1. Selecione o botão **[!UICONTROL Criar serviço de assinatura]**.

   ![Captura de tela mostrando o botão Criar serviço de assinatura](assets/service-create-button.png){zoomable="yes"}

1. Selecione um canal: **[!UICONTROL Email]** ou **[!UICONTROL SMS]**.

1. Nas propriedades do serviço, insira um rótulo e defina **[!UICONTROL Opções adicionais]**, conforme necessário.

   ![Captura de tela mostrando a seção de propriedades do serviço com rótulo e opções adicionais](assets/service-create-properties.png){zoomable="yes"}

1. Por padrão, os serviços são armazenados na pasta **[!UICONTROL Serviços e Assinaturas]**. Você pode alterá-la navegando até o local desejado. [Saiba como trabalhar com pastas](../get-started/permissions.md#folders)

1. Por padrão, as subscrições são ilimitadas.

   Desabilite a opção **[!UICONTROL Período de validade ilimitado]** para definir uma duração de validade para o serviço. Quando o período de validade terminar:
   * Nenhum perfil pode assinar mais este serviço.
   * Todos os assinantes deste serviço têm a subscrição cancelada automaticamente.

   ![Captura de tela mostrando as configurações de período de validade de um serviço de assinatura](assets/service-create-validity-period.png){zoomable="yes"}

1. Quando um usuário(a) assina ou cancela a assinatura de um serviço, é possível enviar uma mensagem de confirmação. Selecione os modelos a serem usados para essa mensagem de acordo com seu caso de uso. Esses modelos devem ser configurados com o target mapping de **[!UICONTROL Assinaturas]**. [Saiba mais](#create-confirmation-message)

   ![Captura de tela mostrando a seleção do modelo de mensagem de confirmação](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. Clique em **[!UICONTROL Salvar e examinar]**. O novo serviço foi adicionado à lista **[!UICONTROL Serviços de assinatura]**.

1. Selecione as landing pages de assinatura e cancelamento de assinatura padrão associadas a esse serviço.

   ![Captura de tela mostrando as configurações padrão da página de aterrissagem de um serviço de assinatura](assets/service-create-default-lp.png){zoomable="yes"}

   Depois de concluído, ao [inserir um link](../email/message-tracking.md) em um email, selecione **[!UICONTROL Link de assinatura]** ou **[!UICONTROL Link de cancelamento de assinatura]**. Ao clicar nesse link, os usuários serão direcionados para a landing page de assinatura ou unsubscription referenciada no serviço. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

   ![Captura de tela mostrando as configurações de link de assinatura e cancelamento de assinatura](assets/service-create-default-lp-link.png){zoomable="yes"}

1. Salve e revise as alterações.

Agora você pode:

* Adicionar assinantes manualmente a este serviço e cancelar a assinatura de perfis. [Saiba mais](../audience/manage-subscribers.md)

* Convide seus clientes a assinar esse serviço por meio de uma landing page. [Saiba mais](../landing-pages/lp-use-cases.md#lp-subscription)

* Enviar mensagens aos assinantes deste serviço. [Saiba como](../msg/send-to-subscribers.md)

## Criar uma mensagem de confirmação {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="Selecione o modelo de entrega de assinaturas"
>abstract="Para enviar mensagens de confirmação a usuários que assinam seu serviço, é necessário selecionar um modelo de entrega específico com base no target mapping **[!UICONTROL Assinaturas]**, sem um público-alvo definido."

>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Selecione o modelo de entrega de cancelamento de assinatura"
>abstract="Para enviar mensagens de confirmação a usuários que cancelaram a assinatura do seu serviço, você deve selecionar um modelo de entrega específico com base no target mapping **[!UICONTROL Assinaturas]**, sem público-alvo definido."

Para enviar mensagens de confirmação aos usuários que assinam ou cancelam a assinatura do seu serviço, crie um modelo de entrega com o target mapping das **[!UICONTROL Assinaturas]**, sem um destino definido. Siga as etapas abaixo:

1. Crie um template do delivery para a confirmação da subscrição. [Saiba como criar um modelo](../msg/delivery-template.md)

1. Não selecione um público para esta entrega. Em vez disso, acesse as **[!UICONTROL Configurações]** da entrega, vá para a guia [Público](../advanced-settings/delivery-settings.md#audience) e selecione o target mapping das **[!UICONTROL Assinaturas]** na lista.

   ![Captura de tela mostrando a seleção de mapeamento de destino para um modelo de entrega](assets/service-confirmation-template-mapping.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se você não selecionar o target mapping das **[!UICONTROL Assinaturas]**, seus assinantes não receberão a mensagem de confirmação. Saiba mais sobre target mappings em [esta seção](../audience/targeting-dimensions.md).

1. Edite o conteúdo do template do delivery, salve e feche-o.

   ![Captura de tela mostrando o editor de conteúdo para um modelo de entrega](assets/service-confirmation-template.png){zoomable="yes"}

   >[!NOTE]
   >
   >Saiba mais sobre os canais de entrega e como definir o conteúdo de entrega nas seções [Canal de email](../email/create-email.md) e [Canal de SMS](../sms/create-sms.md).

1. Repita as etapas acima para criar um template do delivery para a confirmação do cancelamento de subscrição.

Agora você pode selecionar essas mensagens ao [criar um serviço de assinatura](#create-service). Os usuários que assinarem ou cancelarem a assinatura desse serviço receberão as mensagens de confirmação selecionadas.

## Monitorar seus serviços de assinatura {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Contagem de assinantes"
>abstract="Clique em **Calcular** para obter o número total de assinantes deste serviço."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="Número total de assinantes"
>abstract="O Indicador principal de desempenho (KPI) fornece uma visão abrangente da base de assinantes, mostrando a contagem total de pessoas que assinaram esse serviço."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Número de assinaturas no período"
>abstract="Use a lista suspensa para alterar o intervalo de tempo e exibir o número de assinaturas e cancelamentos de assinaturas durante o período selecionado."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Evolução geral das assinaturas"
>abstract="Este gráfico mostra o detalhamento por período, incluindo assinaturas, cancelamentos de assinaturas, a evolução em números e a porcentagem de fidelidade."

Para medir a eficácia de seus serviços de assinatura para canais de SMS e email, acesse os logs e relatórios de um determinado serviço.

1. Selecione um serviço existente na lista **[!UICONTROL Subscription services]**. Clique em **[!UICONTROL Calcular]** para obter o número total de assinantes.

   ![Captura de tela mostrando o cálculo do número total de assinantes](assets/service-logs-subscribers-count.png){zoomable="yes"}

1. No painel de serviço, selecione **[!UICONTROL Logs]** para exibir a lista de assinantes deste serviço.

   É possível verificar o número total de assinantes, o nome e o endereço de cada recipient e quando eles fizeram a assinatura ou cancelaram a assinatura. Também é possível filtrá-los.

   ![Captura de tela mostrando a seção de logs com detalhes do assinante](assets/service-logs.png){zoomable="yes"}

1. No painel de serviço, selecione **[!UICONTROL Relatórios]**. Verifique os seguintes indicadores:

   * O **[!UICONTROL Número total de assinantes]** é exibido.

   * Exiba o número de subscrições e unsubscriptions durante um período selecionado. Use a lista suspensa para alterar o intervalo de tempo.

     ![Captura de tela mostrando a seção de relatórios com os dados de assinatura e cancelamento de assinatura](assets/service-reports.png){zoomable="yes"}

   * O gráfico **[!UICONTROL Evolução geral das assinaturas]** mostra o detalhamento por período, incluindo assinaturas, cancelamentos de assinaturas, a evolução em números e a porcentagem de fidelidade.<!--what is Registered?-->

1. Use o botão **[!UICONTROL Recarregar]** para recuperar os valores mais recentes da execução e do agendamento do fluxo de trabalho de rastreamento.