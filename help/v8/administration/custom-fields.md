---
title: Campos personalizados
description: Saiba como configurar campos personalizados e sua visibilidade na interface.
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: f08603afde2493457bc81a0d808b647b70a52f7c
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 20%

---

# Configurar campos personalizados {#custom-fields}

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="Edição de tela"
>abstract="Todos os campos personalizados da interface do esquema selecionado são exibidos. É possível alterar a ordem em que eles são exibidos na interface, usando as setas para cima e para baixo e agrupar campos em subseções adicionando separadores. Para excluir um campo personalizado ou editar configurações como condições de visibilidade, clique no botão de reticências."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_general"
>title="Geral"
>abstract="Defina as configurações gerais do campo personalizado. Se nenhum rótulo for fornecido, o rótulo definido no esquema será exibido. Use o campo **Visível se** para definir uma condição usando uma expressão xtk que controla quando o campo é exibido. Você também pode marcar o campo como obrigatório ou somente leitura na interface."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_link"
>title="Propriedades do link"
>abstract="Use o modelador de consultas para especificar regras para a exibição de um campo personalizado do tipo link. Por exemplo, restringir valores de lista com base em outra entrada de campo."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings_layout"
>title="Layout"
>abstract="Por padrão, os campos personalizados são exibidos na interface em duas colunas. Ative essa opção para exibir o campo personalizado na largura total da tela, em vez de em duas colunas."

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_separatorproperties"
>title="Propriedades do separador"
>abstract="Especifique o nome que será exibido na interface da subseção."

<!-- NOT USED IN THE UI?-->

>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields_settings"
>title="Configurações de atributo"
>abstract="Configurações de atributo"

Os campos personalizados são atributos adicionais adicionados a esquemas prontos para uso por meio do console do Adobe Campaign. Eles permitem que você personalize esquemas, incluindo novos atributos para atender às necessidades da sua organização. Saiba como estender um esquema na [documentação do Adobe Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html?lang=pt-BR){target="_blank"}.

Campos personalizados podem ser exibidos em várias telas, como detalhes do perfil na interface da Web do Campaign. Os administradores podem controlar quais campos ficam visíveis e como eles são exibidos. Essas alterações se aplicam a todos os usuários do Campaign.

>[!NOTE]
>
>Você precisa ter direitos de administrador para gerenciar campos personalizados.

Campos personalizados estão disponíveis para os seguintes esquemas:

* Campanhas (nms)
* Planos (nms)
* Programas (nms)
* Destinatários (nms)
* Seed addresses (nms)
* Entregas (nms)

## Adicionar campos personalizados à interface {#add}

Para exibir campos personalizados na interface, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Esquemas]** no painel de navegação esquerdo e localize o esquema desejado.

   Use o filtro **[!UICONTROL Editável]** no painel de filtros para identificar rapidamente esquemas com campos personalizados.

   ![Captura de tela mostrando o menu Esquemas e o filtro Editável no painel de navegação](assets/custom-fields-open.png)

1. Selecione o nome do schema na lista para abri-lo. Uma visualização detalhada do esquema é exibida. [Saiba mais sobre detalhes do esquema](../administration/schemas.md). Clique no botão **[!UICONTROL Edição de tela]** para acessar campos personalizados. Neste exemplo, campos são adicionados para o esquema **[!UICONTROL Recipients]**.

   ![Captura de tela mostrando o botão Definição de tela na exibição de esquema](assets/custom-fields-edit.png)

   A lista de campos personalizados exibidos na interface do esquema é exibida.

1. Clique no botão **[!UICONTROL Visualizar]** para exibir os campos personalizados em uma tela de exemplo.

   ![](assets/custom-fields-edit2.png)

   Aqui, o campo &quot;Valor&quot; foi marcado como obrigatório.

   ![](assets/custom-fields-edit3.png)

1. Para adicionar um campo personalizado à interface, clique no botão de reticências e escolha uma das seguintes opções:

   * **[!UICONTROL Selecionar campos personalizados]**: selecione um ou vários campos personalizados para exibir na interface.
   * **[!UICONTROL Preencha automaticamente a lista de campos personalizados]**: adicione à interface todos os campos personalizados definidos para o esquema.

   ![Captura de tela mostrando as opções para adicionar campos personalizados](assets/custom-fields-add.png)

1. Depois que os campos personalizados forem adicionados, você poderá:

   * **Reordenar campos**: use as setas para cima e para baixo ou mova os campos usando a função arrastar e soltar.
   * **Tornar campos obrigatórios**: marque a caixa de seleção **Obrigatório**.
   * **Editar configurações de campo**: clique no botão de reticências e escolha **[!UICONTROL Editar]**. [Saiba mais](#settings)
   * **Excluir campos**: clique no botão de reticências e escolha **[!UICONTROL Excluir]**.
   * **Organize os campos em subseções na interface**: clique no botão de reticências ao lado das setas para cima e para baixo e escolha **[!UICONTROL Adicionar separador]**. [Saiba mais](#separator)

## Definir configurações de campos personalizados {#settings}

Para definir configurações específicas para cada campo personalizado, clique no botão de reticências ao lado do campo desejado e selecione **[!UICONTROL Editar]**.

![Captura de tela mostrando o menu de configurações para campos personalizados](assets/custom-fields-settings.png)

Configurações disponíveis:

* **[!UICONTROL Atributo]**: o nome do campo personalizado.
* **[!UICONTROL Rótulo (personalizado)]**: o rótulo a ser exibido na interface. Se nenhum rótulo for fornecido, o rótulo definido no esquema será exibido.
* **[!UICONTROL Visível se]**: defina uma condição usando uma expressão xtk que controle quando o campo é exibido. Por exemplo, oculte este campo se outro campo estiver vazio.
* **[!UICONTROL Obrigatório]**: tornar o campo obrigatório na interface.
* **[!UICONTROL Somente leitura]**: tornar o campo somente leitura na interface. Os usuários não poderão editar o valor do campo.
* **[!UICONTROL Configurações de filtro]** (para campos do tipo link): use o modelador de consulta para especificar regras para a exibição de um campo personalizado do tipo link. Por exemplo, restringir valores de lista com base em outra entrada de campo.

  Você também pode fazer referência ao valor inserido em outros campos em suas condições usando a sintaxe `$(<field-name>)`. Isso permite fazer referência ao valor atual de um campo, conforme inserido no formulário, mesmo que ele ainda não tenha sido salvo no banco de dados.

  No exemplo abaixo, a condição verifica se o valor do campo @ref corresponde ao valor inserido no campo @refCom. Por outro lado, usar `@refCom` em vez de `$(@refCom)` referenciaria o valor do campo @ref como ele existe no banco de dados.

  +++Exibir exemplo

  ![Captura de tela mostrando um exemplo de configurações de filtro para campos personalizados](assets/custom-fields-ref.png)

  +++

* **[!UICONTROL Abranger duas colunas]**: por padrão, os campos personalizados são exibidos na interface em duas colunas. Ative essa opção para exibir o campo personalizado na largura total da tela, em vez de em duas colunas.

## Organizar campos personalizados em subseções {#separator}

A interface do usuário da Web do Campaign permite adicionar separadores para agrupar campos personalizados na interface para facilitar a leitura. Para fazer isso, siga estes passos:

1. Clique no botão de reticências ao lado das setas para cima e para baixo e selecione **[!UICONTROL Adicionar separador]**.

1. Uma nova linha representando o separador é adicionada à lista. Clique no botão de reticências e escolha **[!UICONTROL Editar]** para nomear a subseção.

1. Use as setas para cima e para baixo para mover o separador para o local desejado. Os campos listados abaixo do separador serão agrupados abaixo dele.

   Neste exemplo, os campos &quot;Coleções interessadas&quot; e &quot;Marca&quot; são agrupados em uma subseção &quot;Coleção&quot;.

   | Configuração de campos personalizados | Renderização na interface |
   |  ---  |  ---  |
   | ![Captura de tela mostrando a configuração de um separador](assets/custom-fields-separator.png){zoomable="yes"} | ![Captura de tela mostrando a renderização de uma subseção na interface](assets/custom-fields-section.png){zoomable="yes"} |