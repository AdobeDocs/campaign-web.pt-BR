---
product: campaign
title: Acessar entregas
description: Saiba como acessar e gerenciar seus deliveries no Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
TQID: 'https://experienceleague.adobe.com/P9OIAwfErA7-JDq-nlxKBelTAR0vn8QVVcghdIxyth4'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: 50d1fd2e-0fc9-5627-bbc9-02dbc9d15e08
    internal-label: Email
  - id: 237333ba-90fa-554c-bc8d-2047e6173477
    internal-label: Cross Channel Orchestration
  - id: a4671286-a59f-47e3-b97b-90627a1977d5
    internal-label: Communication channels
subfeature_v2:
  - id: a4657621-810c-498b-8a27-7ced9c176dda
    internal-label: Push notifications
  - id: b1bd1421-1927-4c59-9bc6-ce292360e43b
    internal-label: SMS Messaging
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 4fa6c49fb2456ef2edeb3f609b77c0cc5d33b95e
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 36%
---
# Acessar entregas {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Entregas"
>abstract="Uma entrega é uma comunicação que é enviada para um público-alvo em um canal específico: email, SMS ou push. Nesta tela, você pode editar, duplicar e excluir as entregas existentes. Também é possível exibir relatórios de entregas concluídas. Clique no botão **Criar entrega** para adicionar uma nova entrega."

## Acessar entregas {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Público-alvo adicional"
>abstract="Essas regras só podem ser alteradas no console do cliente."

Os deliveries podem ser acessados no menu **[!UICONTROL Deliveries]**, no painel de navegação esquerdo. Todos os deliveries criados no console do cliente ou na interface do usuário da Web aparecem nesta lista. Nessa tela, é possível monitorar todos os deliveries existentes, duplicá-los ou excluí-los ou criar novos.

![Lista de entregas exibida na interface](assets/deliveries-list.png)

Para abrir um delivery, clique no nome na lista. A entrega é aberta, permitindo executar várias ações, como editar parâmetros, verificar a execução ou monitorar o desempenho usando relatórios dedicados.

![Tela de detalhes da entrega mostrando parâmetros e relatórios](assets/delivery-details.png)

Se você abrir um delivery criado no console do cliente, duas novas seções poderão ser exibidas para o público-alvo. Esses parâmetros só podem ser modificados no console.

* **[!UICONTROL Destino adicional]**: indica que vários destinos foram configurados para esta entrega.

* **[!UICONTROL Destino de prova adicional]**: indica que uma condição dinâmica foi definida para destinos de prova nesta entrega.

![Mensagem de aviso sobre a configuração de destino adicional](assets/target-warning-audience.png){zoomable="yes"}

## Duplicação de uma entrega {#delivery-duplicate}

É possível criar uma cópia de uma entrega existente, ou na lista de entregas ou no painel de entregas.

Para duplicar uma entrega da lista de entregas, siga estas etapas:

1. Clique no botão de três pontos à direita, ao lado do nome da entrega a ser duplicada.
1. Selecione **[!UICONTROL Duplicar]**.
1. Confirme a duplicação. O novo painel do delivery é aberto na tela central.

Para duplicar uma entrega do painel, siga estas etapas:

1. Abra a entrega e clique no botão **[!UICONTROL ...Mais]** na seção superior da tela.
1. Selecione **[!UICONTROL Duplicar]**.
1. Confirme a duplicação. O novo delivery substitui o delivery atual na tela central.

## Excluir uma entrega {#delivery-delete}

Os deliveries são excluídos da lista de delivery, seja da entrada de delivery principal no painel esquerdo ou da lista de delivery de uma campanha.

Para excluir uma entrega da lista de entregas, siga estas etapas:

1. Clique no botão de três pontos à direita, ao lado do nome do delivery a ser excluído.
1. Selecione **[!UICONTROL Delete]**.
1. Confirmar exclusão.

![Excluindo uma entrega da interface da lista de entrega](assets/delete-delivery-from-list.png)

Todas as entregas estão disponíveis nessas listas, mas as entregas criadas em um fluxo de trabalho não podem ser excluídas nelas. Para excluir um delivery criado no contexto de um workflow, exclua a atividade de delivery do workflow.

Para excluir uma entrega de um fluxo de trabalho, siga estas etapas:

1. Selecione a atividade de delivery.
1. Clique no ícone **[!UICONTROL Excluir]** no painel direito.
1. Confirmar exclusão. Se o delivery tiver nós filhos, escolha excluí-los também ou mantê-los.

![Excluindo uma atividade de entrega em um fluxo de trabalho](assets/delete-delivery-from-wf.png)