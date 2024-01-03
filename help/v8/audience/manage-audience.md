---
audience: end-user
title: Monitorar e gerenciar públicos-alvo
description: Saiba como monitorar e gerenciar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 16%

---

# Monitorar e gerenciar públicos-alvo {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Erro de público-alvo"
>abstract="Os dados de público-alvo não estão disponíveis. Aguarde o fim da execução do fluxo de trabalho."

O público-alvo é o principal foco da sua entrega: os destinatários que receberão as mensagens O tipo de público-alvo depende do target mapping definido no modelo de entrega. Saiba mais sobre modelos de entrega em [esta página](../msg/delivery-template.md).

Para definir a população de um público-alvo, é possível:

* [Criar novos públicos](create-audience.md) do **[!UICONTROL Públicos-alvo]** menu,
* [Selecionar um público existente](add-audience.md) criado como uma lista no console do cliente ou proveniente da Adobe Experience Platform,
* [Criar um novo público](segment-builder.md) com o construtor de regras, definindo e combinando critérios de filtragem,
* [Usar um público-alvo de um arquivo externo](file-audience.md). Essa opção só está disponível para deliveries de email independentes e não pode ser usada em deliveries de campanha.

Ao direcionar um público-alvo, você também pode definir **grupos de controle** para evitar o envio de mensagens para uma parte do público-alvo e medir o impacto das campanhas. [Saiba como definir um grupo de controle](control-group.md)

>[!NOTE]
>
>Ao enviar mensagens no contexto de um workflow de campanha, o público-alvo é definido em um **Criar público-alvo** atividade de workflow. Nesse contexto, não é possível carregar um público-alvo de um arquivo para uma entrega de email, e o público-alvo é definido somente nessa atividade dedicada. Saiba como definir o público-alvo do seu delivery em um fluxo de trabalho de campanha no [nesta seção](../workflows/activities/build-audience.md)

A lista de públicos-alvo disponíveis para uso no Campaign Web pode ser acessada no **[!UICONTROL Públicos-alvo]** menu.

![](assets/audiences-list.png)

Os públicos-alvo podem se originar de várias fontes. A variável **[!UICONTROL Origem]** indica onde um determinado público-alvo foi criado:

* **[!UICONTROL Adobe Campaign]**: esses públicos-alvo são criados no console do Adobe Campaign V8. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=pt-BR){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Esses públicos-alvo são criados no Adobe Experience Platform e integrados ao Campaign Web usando a integração Adobe Fontes e Destinos. Saiba como configurar essa integração no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

>[!NOTE]
>
>Para usar os públicos da Adobe Experience Platform no Campaign, você precisa configurar a integração com Fontes e Destinos do Adobe. Consulte [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL WebUI do Adobe Campaign]**: esses públicos são criados usando workflows de público-alvo da Web do Campaign. [Saiba como criar públicos](create-audience.md)

Para obter mais informações sobre um público, abra-o na lista. As propriedades do público são exibidas junto com o número de perfis incluídos no público. É possível atualizar a contagem de públicos-alvo a qualquer momento usando o **[!UICONTROL Calcular]** botão.

A variável **[!UICONTROL Dados]** permite visualizar os perfis que fazem parte do público-alvo. Você pode personalizar essa visualização adicionando mais colunas ou utilizando filtros avançados para refinar os dados exibidos.

![](assets/audiences-details.png)

Para duplicar ou excluir um público-alvo, clique no **[!UICONTROL Mais ações]** botão disponível na lista públicos-alvo ao lado do nome do público-alvo ou dentro de uma tela de detalhes do público-alvo.
