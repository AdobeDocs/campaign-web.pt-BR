---
title: Adicionar filtros personalizados
description: Saiba como adicionar filtros personalizados como campos de acesso rápido no painel Filtros de uma exibição de lista.
exl-id: 2c3d4e5f-6a7b-4c8d-9e0f-1a2b3c4d5e6f
source-git-commit: c2e627d322937b80cb0bc09e86680757d4867dcd
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Adicionar filtros personalizados {#custom-filters}

A seção **[!UICONTROL Configuração da lista de inventário]** > **[!UICONTROL Filtros personalizados]** permite escolher quais atributos serão exibidos como campos de acesso rápido no [painel de filtros](../query/filter.md) da exibição de lista de um esquema, acima do **[!UICONTROL Construtor de regras de filtros avançados]**.

Para obter mais informações sobre a tela de definição de tela e como acessá-la, consulte a seção [Acessar a definição de tela](schemas-browse-access.md#screen-def).

## Adicionar filtros personalizados {#add}

1. Navegue até o menu **[!UICONTROL Esquemas]** e localize os esquemas editáveis usando os filtros.

1. Selecione o nome do esquema na lista para abri-lo e clique no botão **[!UICONTROL Edição da tela]** na exibição de detalhes do esquema para acessar a definição da tela.

1. Vá para a seção **[!UICONTROL Configuração da lista de inventário]** e clique no ícone de reticências acima da tabela **[!UICONTROL Filtros personalizados]** e escolha **[!UICONTROL Selecionar atributos]**.

   ![Seleção de filtros personalizados](assets/schemas-custom-filters1.png)

1. Selecione um ou vários atributos e confirme.

   É possível selecionar:

   * Um atributo direto do schema, por exemplo, um código ou uma categoria.
   * Um atributo de link, por exemplo, uma marca vinculada a um produto. Nesse caso, o filtro usa um seletor de pesquisa restrito ao schema vinculado.
   * Um subatributo de um link, por exemplo, o nome completo de uma pasta vinculada ou o email de um recipient vinculado.

   ![Seletor de atributos mostrando atributos diretos e subatributos de links](assets/schemas-custom-filters2.png)

1. Clique em **[!UICONTROL Save]**. Você pode reordenar filtros personalizados usando as setas para cima e para baixo ou arrastando-os e remover um filtro usando o ícone de lixeira na linha.

1. Navegue até a lista de registros para este esquema e abra o painel de filtros. Os atributos selecionados são exibidos como **[!UICONTROL Filtros personalizados]**, acima do construtor de regras de **[!UICONTROL Filtros avançados]**.

   ![Filtros personalizados exibidos no painel de filtros](assets/schemas-custom-filters3.png)

   >[!NOTE]
   >
   >Um filtro personalizado com base em um atributo de data ou data e hora é exibido como um seletor de intervalo de datas.

1. Insira ou selecione um valor em um dos filtros personalizados para refinar a lista.

<!--
## Configure a custom filter's settings {#settings}

To configure specific settings for a custom filter, click the ellipsis icon on its row and select **[!UICONTROL Edit]**.

![Custom filter settings dialog](assets/schemas-custom-filters5.png)

Available settings are:

* **[!UICONTROL Label (custom)]**: The label to display for this filter. If no label is provided, the attribute's label defined in the schema is used.
* **[!UICONTROL Filter settings]** (for link-type custom filters only): Use the query modeler to specify a condition that restricts the values available in the picker. For example, restrict a delivery filter to deliveries using the email channel.
-->