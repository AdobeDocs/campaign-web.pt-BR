---
audience: end-user
title: Monitorar e gerenciar públicos
description: Saiba como monitorar e gerenciar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
source-git-commit: 424caa898ff9d73f3520aa6d682eb1963d992069
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 3%

---


# Monitorar e gerenciar públicos {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Erro de público"
>abstract="Os dados do público-alvo não estão disponíveis. Aguarde o fim da execução do fluxo de trabalho."

A lista de públicos-alvo disponíveis para uso no Campaign Web pode ser acessada no **[!UICONTROL Públicos-alvo]** menu.

![](assets/audiences-list.png)

Os públicos-alvo podem se originar de várias fontes. A variável **[!UICONTROL Origem]** indica onde um determinado público-alvo foi criado:

* **[!UICONTROL Adobe Campaign]**: esses públicos-alvo são criados no console do Adobe Campaign V8. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=pt-BR){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Esses públicos-alvo são criados no Adobe Experience Platform e integrados ao Campaign Web usando a integração Adobe Fontes e Destinos. Saiba como configurar essa integração no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

>[!NOTE]
>
>Para usar os públicos da Adobe Experience Platform no Campaign, você precisa configurar a integração com Fontes e Destinos do Adobe. Consulte [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

* **[!UICONTROL WebUI do Adobe Campaign]**: esses públicos são criados usando workflows de público-alvo da Web do Campaign. [Saiba como criar públicos](create-audience.md)

Para obter mais informações sobre um público, abra-o na lista. As propriedades do público são exibidas junto com o número de perfis incluídos no público. É possível atualizar a contagem de públicos-alvo a qualquer momento usando o **[!UICONTROL Calcular]** botão.

A variável **[!UICONTROL Dados]** permite visualizar os perfis que fazem parte do público-alvo. Você pode personalizar essa visualização adicionando mais colunas ou utilizando filtros avançados para refinar os dados exibidos.

![](assets/audiences-details.png)

Para duplicar ou excluir um público-alvo, clique no **[!UICONTROL Mais ações]** botão disponível na lista públicos-alvo ao lado do nome do público-alvo ou dentro de uma tela de detalhes do público-alvo.