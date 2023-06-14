---
audience: end-user
title: Enviar ofertas
description: Enviar ofertas
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
badge: label="Alpha"
source-git-commit: 4fbab5ddf2f1c69fbe27d214aa3e349075054c10
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 95%

---


# Enviar ofertas {#offers-content}

O Adobe Campaign v8 Web permite enviar com suas ofertas de email que foram criadas no console usando o módulo **[!UICONTROL Interação]**. Para obter mais informações sobre o módulo Interação e como gerenciar um catálogo de ofertas no console, consulte a [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html?lang=pt-BR){target="_blank"}.

As etapas para enviar ofertas com um email são as seguintes:

1. [Configurar as ofertas a serem propostas](#configure),
1. [Inserir as ofertas no email](#insert).

## Configurar as ofertas a serem propostas {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Configurações de ofertas"
>abstract="Configurar quais ofertas devem ser propostas para os recipients."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Configurações avançadas de ofertas"
>abstract="Configurar as opções avançadas em ofertas."

1. Para selecionar as ofertas a serem propostas no seu email, clique no botão **[!UICONTROL Ofertas]** na tela de edição de conteúdo de email.

   ![](assets/setup-offers.png)

1. Configurar quais ofertas devem ser propostas para os recipients. Primeiro, selecione o **[!UICONTROL Espaço de ofertas]** que corresponda ao seu ambiente de oferta.

   ![](assets/create-content-offers.png)

1. Para refinar a escolha de ofertas do mecanismo, selecione uma **[!UICONTROL Categoria de oferta]** específica em que as ofertas são classificadas. Ao selecionar uma pasta, todas as subpastas são incluídas automaticamente e não podem ser removidas. Observe que a interface do usuário não reflete esse comportamento.

   Se nenhuma categoria for especificada, todas as ofertas contidas no ambiente serão consideradas pelo Mecanismo de oferta, a menos que um **[!UICONTROL Tema de oferta]** seja selecionado.

   >[!NOTE]
   >
   >Os temas são palavras-chave definidas de forma ascendente nas categorias. Elas funcionam como um filtro e permitem refinar o número de ofertas que serão apresentadas ao selecioná-las em um conjunto de categorias.

1. Use o campo **[!UICONTROL Proposições]** para especificar o número de ofertas que deseja inserir no email.

1. Selecione a opção **[!UICONTROL Excluir recipients não qualificados]** se necessário.

   Essa opção permite ativar ou desativar a exclusão de recipients para os quais não há ofertas elegíveis suficientes.

   * Se a opção estiver ativada, os recipients que não tiverem proposições suficientes serão excluídos da entrega.
   * Se a opção estiver desativada, esses recipients não serão excluídos, mas não poderão ter o número solicitado de proposições.

1. Se necessário, selecione a opção **[!UICONTROL Ocultar tudo se nenhuma oferta estiver selecionada]**.

   Essa opção permite escolher como a mensagem será processada caso uma das proposições não exista.

   * Quando a opção estiver habilitada, a representação da proposição ausente não é exibida e nenhum conteúdo aparece na mensagem para essa proposição.
   * Se a opção estiver desabilitada, a mensagem propriamente dita será cancelada durante o envio e os receipients não receberão nenhuma mensagem.

Após configurar as ofertas para propor no seu email, você pode inseri-las no email usando o Editor de expressão. [Saiba como inserir ofertas no email](#insert)

## Inserir ofertas no email {#insert}

As ofertas podem ser adicionadas ao email usando o Editor de expressão. Também podem ser inseridos:

* Na linha de assunto do email,
* no corpo do email, permitindo a personalização em qualquer componente de conteúdo. [Saiba como adicionar componentes de conteúdo](content-components.md)

>[!NOTE]
>
>Antes de inserir uma oferta, verifique se você [configurou quais ofertas apresentará com o email](#configure).

Para inserir uma oferta usando o Editor de expressão, siga estas etapas:

1. Abra o Editor de expressão e selecione o menu **[!UICONTROL Proposições]**.

   As apresentações disponíveis são exibidas na lista. O número de apresentações é definido ao configurar as ofertas a serem propostas.

   ![](assets/offer-insertion.png)

1. Adicione as apresentações ao assunto ou corpo do email usando os campos de personalização, as funções de renderização ou os atributos de oferta disponíveis para cada apresentação.

   ![](assets/offer-inserted.png)
