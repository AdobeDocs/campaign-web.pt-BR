---
title: Procurar e acessar esquemas
description: Saiba como procurar e acessar esquemas na interface.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 3%

---

# Acessar e configurar schemas {#access}

Os esquemas podem ser acessados no menu **[!UICONTROL Administração]** > **[!UICONTROL Esquemas]**.

![Tela da lista de esquemas mostrando os esquemas e filtros disponíveis](assets/schemas-list.png)

Nessa tela, você pode exibir todos os esquemas existentes. Os filtros estão disponíveis para ajudar a refinar a lista, por exemplo, para exibir apenas esquemas editáveis.

Para abrir um esquema, selecione seu nome. Uma visualização detalhada do esquema é exibida.

![Tela de detalhes do esquema mostrando as propriedades e o conteúdo do esquema](assets/schema-details.png)

## Visão geral do esquema {#overview}

A guia **[!UICONTROL Visão geral]** fornece uma exibição geral do esquema:

* A seção **[!UICONTROL Propriedades]** exibe informações importantes, como o nome do esquema, o namespace e o nome da tabela associada.

* A seção **[!UICONTROL Definição de esquema]** mostra detalhes sobre a definição de esquema, incluindo a chave primária usada para reconciliação de dados e seus links com outras tabelas.

  Clique no botão **[!UICONTROL Visualização do esquema]** para exibir os diferentes campos e links que compõem o esquema. Isso permite verificar a estrutura completa de um esquema. Se o esquema tiver sido estendido com campos personalizados, você poderá visualizar todas as suas extensões.

* A seção **[!UICONTROL Content]** exibe o conteúdo XML do esquema, permitindo que você alterne entre a fonte e a sintaxe gerada.

## Dados do esquema {#data}

A guia **[!UICONTROL Dados]** fornece informações sobre os dados do esquema.

![Guia de dados de esquema mostrando a estrutura de dados e os atributos](assets/schemas-data.png)

## Personalizar exibição de tela {#screen-def}

A definição de tela permite configurar como os campos de esquema são exibidos e editados na interface. Você pode configurar colunas padrão para exibições de lista, personalizar quais campos personalizados serão exibidos em telas de detalhes, adicionar listas de coleção para mostrar dados relacionados e organizar campos em seções com separadores e critérios de visibilidade.

Para acessar a definição da tela:

1. Navegue até o menu **[!UICONTROL Esquemas]** e localize os esquemas editáveis usando os filtros.

   ![Tela da lista de esquemas mostrando os esquemas e filtros disponíveis](assets/schemas-list2.png)

1. Selecione o nome do esquema na lista para abri-lo e clique no botão **[!UICONTROL Edição da tela]** na exibição de detalhes do esquema para acessar a definição da tela.

   ![Tela da lista de esquemas mostrando os esquemas e filtros disponíveis](assets/schemas-list3.png)

   As diferentes listas permitem reordenar elementos usando os ícones de seta para cima e para baixo ou arrastando e soltando-os. Para remover itens, clique no ícone de lixeira em uma linha específica ou selecione **[!UICONTROL Excluir tudo]** do ícone de reticências.

   ![Seção geral de definição de tela](assets/schemas-general.png)

Na definição da tela, é possível:

* [Configurar colunas de lista padrão](schemas-list-columns.md) - Configure quais colunas são exibidas por padrão nos modos de exibição de lista.
* [Editar campos personalizados](schemas-custom-fields.md) - Configure quais campos personalizados serão exibidos em telas de detalhes e organize-os em seções.
* [Adicionar listas de coleções](schemas-collection-lists.md) - Adicione listas de coleções para mostrar dados relacionados em telas de perfil.
