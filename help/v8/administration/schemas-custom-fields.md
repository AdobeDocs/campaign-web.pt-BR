---
title: Editar campos personalizados
description: Saiba como configurar campos personalizados e sua visibilidade na interface.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 5%

---

# Editar campos personalizados {#fields}

Os campos personalizados são atributos adicionais adicionados a esquemas prontos para uso por meio do console do Adobe Campaign. Eles permitem que você personalize esquemas, incluindo novos atributos para atender às necessidades da sua organização.

Campos personalizados podem ser exibidos em várias telas, como detalhes de perfil na interface. Você pode controlar quais campos estão visíveis e como eles aparecem na interface.

Para obter mais informações sobre a tela de definição de tela e como acessá-la, consulte a seção [Acessar a definição de tela](schemas-browse-access.md#screen-def).

Para adicionar campos personalizados à lista:

1. Navegue até o menu **[!UICONTROL Esquemas]** e localize os esquemas editáveis usando os filtros.

1. Selecione o nome do esquema na lista para abri-lo e clique no botão **[!UICONTROL Edição da tela]** na exibição de detalhes do esquema para acessar a definição da tela.

1. Clique no ícone de reticências acima da tabela **[!UICONTROL Lista de campos personalizados]** e escolha **[!UICONTROL Selecionar atributos]** para selecionar um ou vários campos personalizados para exibir na interface.
   ![Tela de campos personalizados mostrando atributos editáveis](assets/schemas-custom5.png)
1. Selecione os campos personalizados que deseja adicionar e confirme.

   ![Tela de campos personalizados mostrando atributos editáveis](assets/schemas-custom2.png)

   >[!NOTE]
   >
   > Você também pode selecionar **[!UICONTROL Preencher automaticamente a lista de campos personalizados]** para adicionar todos os campos personalizados definidos para o esquema à interface.

Depois que campos personalizados forem adicionados, você poderá visualizá-los, reorganizá-los, torná-los obrigatórios, editar suas configurações ou organizá-los em subseções.

## Definir configurações de campo {#field-settings}

Para definir configurações específicas para cada campo personalizado, clique no ícone de reticências em uma linha de campo na lista e selecione **[!UICONTROL Editar]**.

![Caixa de diálogo de configurações do atributo](assets/schemas-attribute-settings.png)

Configurações disponíveis:

* **[!UICONTROL Atributo]**: o nome do campo personalizado (somente leitura).
* **[!UICONTROL Rótulo (personalizado)]**: o rótulo a ser exibido na interface. Se nenhum rótulo for fornecido, o rótulo definido no esquema será exibido.
* **[!UICONTROL Visível se]**: defina uma condição usando uma expressão xtk que controle quando o campo é exibido. Por exemplo, oculte este campo se outro campo estiver vazio.
* **[!UICONTROL Obrigatório]**: tornar o campo obrigatório na interface.
* **[!UICONTROL Somente leitura]**: tornar o campo somente leitura na interface. Os usuários não poderão editar o valor do campo.
* **[!UICONTROL Configurações de filtro]** (para campos do tipo link): use o modelador de consulta para especificar regras para a exibição de um campo personalizado do tipo link. Por exemplo, restringir valores de lista com base em outra entrada de campo.

  +++Exibir exemplo

  Você também pode fazer referência ao valor inserido em outros campos em suas condições usando a sintaxe `$(<field-name>)`. Isso permite fazer referência ao valor atual de um campo, conforme inserido no formulário, mesmo que ele ainda não tenha sido salvo no banco de dados.

  No exemplo abaixo, a condição verifica se o valor do campo @ref corresponde ao valor inserido no campo @refCom. Por outro lado, usar `@refCom` em vez de `$(@refCom)` referenciaria o valor do campo @ref como ele existe no banco de dados.

  ![Captura de tela mostrando um exemplo de configurações de filtro para campos personalizados](assets/custom-fields-ref.png)

  +++

* **[!UICONTROL Abranger duas colunas]**: por padrão, os campos personalizados são exibidos na interface em duas colunas. Ative essa opção para exibir o campo personalizado na largura total da tela, em vez de em duas colunas.

## Visualizar campos personalizados {#preview}

Clique em **[!UICONTROL Visualizar]** para exibir os campos personalizados em uma tela de exemplo. Isso permite que você veja como os campos serão exibidos na interface, incluindo quais campos são marcados como obrigatórios.

![Visualizar campos personalizados](assets/schemas-custom4.png)

## Organizar campos em subseções {#separator}

É possível adicionar separadores para agrupar campos personalizados na interface para melhorar a leitura. Para fazer isso, siga estes passos:

1. Clique no ícone de reticências acima da tabela **[!UICONTROL Lista de campos personalizados]** e escolha **[!UICONTROL Adicionar separador]**.

1. Uma nova linha representando o separador é adicionada à lista. Clique no ícone de reticências na linha separadora e escolha **[!UICONTROL Editar]**.

1. Insira um **[!UICONTROL Rótulo]** para o separador e (opcional) defina uma condição **[!UICONTROL Visible if]** para controlar quando o separador é exibido.

   ![Caixa de diálogo de propriedades do separador](assets/schemas-custom3.png)

1. Use as setas para cima e para baixo para mover o separador para o local desejado. Os campos listados abaixo do separador serão agrupados abaixo dele.

   Neste exemplo, os campos &quot;Coleções interessadas&quot; e &quot;Marca&quot; são agrupados em uma subseção &quot;Coleção&quot;.

   | Configuração de campos personalizados | Renderização na interface |
   |  ---  |  ---  |
   | ![Captura de tela mostrando a configuração de um separador](assets/custom-fields-separator.png){zoomable="yes"} | ![Captura de tela mostrando a renderização de uma subseção na interface](assets/custom-fields-section.png){zoomable="yes"} |
