---
product: campaign
title: Acessar entregas
description: Saiba como acessar e gerenciar seus deliveries no Campaign Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
source-git-commit: ecff4e56bd346aadf381a1bf2077204804938f62
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 69%

---

# Acessar entregas {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Entregas"
>abstract="Uma entrega é uma comunicação enviada para um público-alvo em um canal específico: email, SMS ou notificação por push. Nesta tela, você pode editar, duplicar e excluir as entregas existentes. Também é possível exibir relatórios de entregas concluídas. Clique no botão **Criar entrega** para adicionar uma nova entrega."

## Acessar entregas {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Público-alvo adicional"
>abstract="Essas regras só podem ser alteradas no console do cliente."

Os deliveries podem ser acessados no menu **[!UICONTROL Deliveries]**, no painel de navegação esquerdo. Todos os deliveries criados no console do cliente ou na interface do usuário da Web são exibidos nesta lista. Nessa tela, é possível monitorar todos os deliveries existentes, duplicá-los ou excluí-los ou criar novos.

![](assets/deliveries-list.png)

Para abrir um delivery, clique no nome na lista. O delivery é aberto, permitindo executar várias ações, como editar parâmetros, verificar a execução ou monitorar o desempenho usando relatórios dedicados.

![](assets/delivery-details.png)

>[!NOTE]
>
>Se você abrir uma entrega criada no console do cliente, a seção **[!UICONTROL Destino adicional]** poderá ser exibida para o público-alvo. Isso significa que vários targets foram configurados para este delivery. Esses parâmetros só podem ser modificados no console.
>
>![](assets/target-warning-audience.png){zoomable="yes"}

## Duplicação de uma entrega {#delivery-duplicate}

É possível criar uma cópia de uma entrega existente, ou na lista de entregas ou no painel de entregas.

Para duplicar uma entrega da lista de entregas, siga estas etapas:

1. Clique no botão de três pontos à direita, ao lado do nome da entrega a ser duplicada.
1. Selecione  **[!UICONTROL Duplicar]**.
1. Confirme a duplicação: o novo painel de entrega será aberto na tela central.

Para duplicar uma entrega do painel, siga estas etapas:

1. Abra a entrega e clique no botão **[!UICONTROL ...Mais]** na seção superior da tela.
1. Selecione **[!UICONTROL Duplicar]**.
1. Confirme a duplicação: a nova entrega substituirá a entrega atual na tela central.

## Excluir uma entrega {#delivery-delete}

As entregas são excluídas na lista de entregas - seja da entrada da entrega principal no painel esquerdo ou da lista de entregas de uma campanha.

Para excluir uma entrega da lista de entregas, siga estas etapas:

1. Clique no botão de três pontos à direita, ao lado do nome da entrega a ser duplicada.
1. Selecione **[!UICONTROL Excluir]**.
1. Confirmar exclusão.

![Excluir uma entrega da lista de entregas](assets/delete-delivery-from-list.png)

Todas as entregas estão disponíveis nessas listas, mas as entregas criadas em um workflow não podem ser excluídas nelas. Para excluir uma entrega criada no contexto de um workflow, será necessário excluir a atividade de entrega do workflow.

Para excluir uma entrega de um workflow, siga estas etapas:

1. Selecionar a atividade de entrega.
1. Clique no ícone de **[!UICONTROL Excluir]** no painel direito.
1. Confirmar exclusão. Se a entrega tiver nós derivados, você poderá optar por excluí-los também ou mantê-los.

![Excluir uma entrega em um workflow](assets/delete-delivery-from-wf.png)
