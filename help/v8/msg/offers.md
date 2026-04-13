---
audience: end-user
title: Adicionar ofertas em suas mensagens
description: Saiba como adicionar e enviar ofertas
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 23%

---

# Adicionar ofertas às suas mensagens {#offers-content}

Você pode adicionar ofertas aos seus deliveries na interface da Web do Adobe Campaign. Essas ofertas estão disponíveis no menu esquerdo **Ofertas**, que permite acessar a lista de ofertas. Todas essas ofertas são somente leitura e devem ser criadas no console do cliente do Campaign usando o módulo **[!UICONTROL Interaction]**. Para obter mais informações sobre interação e como gerenciar um catálogo de ofertas no console, consulte a [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=pt-BR){target="_blank"}.

As etapas para enviar ofertas com um delivery são as seguintes:

1. [Configurar as ofertas a serem propostas](#configure)
1. [Inserir as ofertas no delivery](#insert)

## Configurar as ofertas a serem propostas {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Defina os parâmetros das ofertas"
>abstract="Configure quais ofertas devem ser propostas aos destinatários, definindo um espaço de ofertas, opcionalmente uma categoria e um tema, e especifique o número de ofertas que deseja inserir na entrega."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Defina as configurações avançadas de ofertas"
>abstract="É possível habilitar a exclusão de destinatários para os quais não há ofertas elegíveis suficientes e escolher como a mensagem será processada caso uma das proposições não exista."

O Adobe Campaign permite responder em tempo real durante uma interação com um determinado contato, propondo uma ou várias ofertas específicas. Essas ofertas podem ser mensagens de comunicação simples, ofertas especiais de um ou vários produtos ou um serviço.

Para selecionar as ofertas a serem adicionadas ao delivery, siga as etapas abaixo.

1. Clique no botão **[!UICONTROL Configurar ofertas]** da tela de edição de conteúdo de entrega.

   ![Captura de tela mostrando o botão de configuração da oferta na tela de edição de conteúdo da entrega](assets/offer-setup.png){zoomable="yes"}

1. Configurar quais ofertas devem ser propostas para os destinatários.

   Primeiro, selecione o **[!UICONTROL Espaço de ofertas]** que corresponda ao seu ambiente de ofertas. Saiba como criar um espaço de ofertas na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}.

   ![Captura de tela mostrando a seleção do espaço de ofertas no conteúdo de criação da oferta](assets/offer-create-content.png){zoomable="yes"}

1. Para refinar a escolha de ofertas do mecanismo, selecione uma **[!UICONTROL Categoria de oferta]** específica em que as ofertas são classificadas.

   Ao selecionar uma pasta, todas as subpastas são incluídas automaticamente e não podem ser removidas. Observe que a interface [!DNL Campaign] não reflete esse comportamento.

   >[!NOTE]
   >
   >Se nenhuma categoria for especificada, todas as ofertas contidas no ambiente serão consideradas pelo Mecanismo de oferta, a menos que um **[!UICONTROL Tema de oferta]** seja selecionado.

1. (Opcional) Insira um tema para filtrar categorias. Os temas são palavras-chave definidas upstream nas categorias. Eles atuam como um filtro e refinam o número de ofertas a serem apresentadas ao selecioná-las em um conjunto de categorias.

1. Use o campo **[!UICONTROL Propositions]** para especificar o número de ofertas que deseja inserir na entrega.

1. Selecione a opção **[!UICONTROL Excluir destinatários não qualificados]** se necessário.

   Essa opção permite ativar ou desativar a exclusão de recipients para os quais não há ofertas elegíveis suficientes:

   * Se a opção estiver habilitada, os destinatários que não tiverem proposições suficientes serão excluídos da entrega.
   * Se a opção estiver desabilitada, esses recipients não serão excluídos, mas não poderão ter o número solicitado de apresentações.

1. Se necessário, selecione a opção **[!UICONTROL Ocultar tudo se nenhuma oferta estiver selecionada]**.

   Essa opção permite escolher como a mensagem será processada caso uma das proposições não exista:

   * Se a opção estiver ativada, a representação da proposta ausente não será exibida e nenhum conteúdo será exibido na mensagem para essa apresentação.
   * Se a opção estiver desabilitada, a própria mensagem será cancelada durante o envio e os recipients não poderão mais receber mensagens.

Depois de configurar as ofertas a serem propostas no delivery, você pode inseri-las no conteúdo do delivery.

## Inserir ofertas no delivery {#insert}

As ofertas podem ser adicionadas na entrega usando o [editor de expressão](../personalization/gs-personalization.md#access). Eles podem ser inseridos na linha de assunto ou no corpo do delivery.

>[!CAUTION]
>
>Antes de inserir uma oferta em uma entrega, verifique se você [configurou quais ofertas propor com essa entrega](#configure).

Para inserir uma oferta usando o editor de expressão, siga as etapas abaixo.

1. Acesse a linha de assunto ou o conteúdo de qualquer delivery.

1. Coloque o cursor onde deseja inserir a oferta e abra o editor de expressão usando o ícone de personalização.

   ![Captura de tela mostrando o ícone de personalização usado para abrir o editor de expressão](assets/offer-insert-perso-icon.png){zoomable="yes"}

1. Selecione o menu **[!UICONTROL Propositions]**. As apresentações disponíveis são exibidas na lista.

   >[!NOTE]
   >
   >O número de apresentações é definido ao [configurar ofertas](#configure) para a entrega atual.

1. Defina cada proposta usando os campos de personalização, funções de renderização ou atributos de oferta disponíveis.

   ![Captura de tela mostrando uma oferta inserida no conteúdo da entrega](assets/offer-inserted.png){zoomable="yes"}

   >[!NOTE]
   >
   >O número de apresentações disponíveis depende da maneira como a chamada do mecanismo é configurada e sua ordem depende da prioridade das ofertas. Saiba mais na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. Salve as alterações.

1. Finalize o conteúdo, teste e envie seu delivery. [Saiba mais](gs-messages.md).

Agora, quando um recipient recebe o delivery, a oferta certa é exibida para esse perfil específico.