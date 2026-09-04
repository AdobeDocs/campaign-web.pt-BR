---
title: Controlar ações em dados
description: Saiba como restringir ações de criação, edição e exclusão em registros de esquema personalizados.
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 12%

---

# Controlar ações em dados {#action-data}

>[!CONTEXTUALHELP]
>id="acw_schema_action_data"
>title="Dados de ações"
>abstract="Configure as ações disponíveis para as telas de detalhes e de lista do esquema. Habilite **[!UICONTROL Somente leitura]** para definir a tela de detalhes como somente leitura e remover ações da lista. Habilite **[!UICONTROL Não permitir exclusão]** para remover a ação de exclusão das telas de detalhes e listas."

A seção **[!UICONTROL Dados de ação]** permite restringir as ações disponíveis nos registros de um esquema personalizado, independentemente das [regras de segurança](../get-started/work-with-folders.md) configuradas em pastas individuais. Essa restrição se aplica no nível do schema, em todas as pastas, para cada usuário, incluindo administradores.

>[!NOTE]
>
>Esta seção só está disponível para esquemas personalizados.

Para obter mais informações sobre a tela de definição de tela e como acessá-la, consulte a seção [Acessar a definição de tela](schemas-browse-access.md#screen-def).

Para configurar dados de ação, siga as etapas abaixo:

1. Navegue até o menu **[!UICONTROL Esquemas]** e localize os esquemas editáveis usando os filtros.

1. Selecione o nome do esquema na lista para abri-lo e clique no botão **[!UICONTROL Edição da tela]** na exibição de detalhes do esquema para acessar a definição da tela.

1. Role para baixo até a seção **[!UICONTROL Dados de ação]**, na parte inferior da definição da tela.

   ![Seção de dados de ação na definição de tela](assets/schemas-action-data1.png)

1. Selecione uma ou mais das opções disponíveis:

   * **[!UICONTROL Somente leitura]**: a tela de detalhes se torna somente leitura para todos os usuários. Nenhuma ação de criação, duplicação, atualização ou exclusão está disponível na lista, e as ações de exclusão e duplicação estão ocultas na tela de detalhes. Selecionar essa opção é semelhante à configuração de uma visualização: os usuários ainda podem abrir registros e reutilizá-los, por exemplo, ao direcionar um delivery, mas não podem modificá-los.

   * **[!UICONTROL Não permitir exclusão]**: a ação de exclusão é removida da tela de detalhes e da lista, em todas as pastas. Outras ações, como criar, duplicar e atualizar, permanecem disponíveis.

   * **[!UICONTROL Não permitir duplicação]**: a ação duplicada é removida da tela de detalhes e da lista, em todas as pastas. Outras ações, como criar, excluir e atualizar, permanecem disponíveis.

     >[!NOTE]
     >
     >A habilitação de **[!UICONTROL Somente leitura]** também abrange automaticamente a exclusão e a duplicação. Portanto, as opções **[!UICONTROL Não permitir exclusão]** e **[!UICONTROL Não permitir duplicação]** são desabilitadas enquanto **[!UICONTROL Somente leitura]** é selecionado.

1. Clique em **[!UICONTROL Save]**.

1. Navegue até a lista de registros deste esquema para verificar o resultado.

   Neste exemplo, **[!UICONTROL Somente leitura]** está habilitado: a lista não exibe mais as ações duplicadas e de exclusão.

   ![Renderização somente leitura na tela da lista](assets/schemas-action-data2.png)

1. Abra um registro para verificar a tela de detalhes. Seus campos são exibidos sem permitir nenhuma edição.

   ![Renderização somente leitura na tela de detalhes](assets/schemas-action-data3.png)
