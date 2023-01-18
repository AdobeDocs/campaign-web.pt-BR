---
audience: end-user
title: Enviar ofertas
description: Enviar ofertas
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 5%

---

# Enviar ofertas {#offers-content}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Configurações de ofertas"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Configurações avançadas de ofertas"
>abstract="TBC"

O Adobe Campaign v8 Web permite enviar com suas ofertas de email que foram criadas no console usando o **[!UICONTROL Interação]** módulo. Para obter mais informações sobre Interação e como gerenciar um catálogo de ofertas no console, consulte o [Documentação do Campaign v8](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

As etapas para enviar ofertas com um email são as seguintes:

1. [Configurar as ofertas a serem propostas](#configure),
1. [Insira as ofertas no email](#insert).

## Configurar as ofertas a serem propostas {#configure}

1. Para selecionar as ofertas a serem propostas no seu email, clique no link **[!UICONTROL Ofertas]** na tela de edição de conteúdo de email.

   ![](assets/setup-offers.png)

1. Configure quais ofertas devem ser propostas para os recipients. Primeiro selecione o **[!UICONTROL Espaço de ofertas]** que corresponde ao seu ambiente de oferta.

   ![](assets/create-content-offers.png)

1. Para refinar a escolha de ofertas do mecanismo, selecione um **[!UICONTROL Categoria de oferta]** em que as ofertas são classificadas.

   Se nenhuma categoria for especificada, todas as ofertas contidas no ambiente serão consideradas pelo Mecanismo de oferta, a menos que uma **[!UICONTROL Tema da oferta]** está selecionada.

   >[!NOTE]
   >
   >Temas são palavras-chave definidas upstream nas categorias. Eles atuam como um filtro e permitem refinar o número de ofertas a serem apresentadas ao selecioná-las em um conjunto de categorias.

1. Use o **[!UICONTROL Propostas]** para especificar o número de ofertas que deseja inserir no email.

1. Selecione a opção **[!UICONTROL Exclude non-eligible recipients]** se necessário.

   Essa opção permite ativar ou desativar a exclusão de recipients para os quais não há ofertas elegíveis suficientes.

   * Se a opção estiver ativada, os recipients que não têm apresentações suficientes serão excluídos do delivery.
   * Se a opção estiver desativada, esses recipients não serão excluídos, mas não poderão ter o número solicitado de apresentações.

1. Se necessário, selecione o **[!UICONTROL Ocultar tudo se nenhuma oferta estiver selecionada]** opção.

   Essa opção permite escolher como a mensagem será processada caso uma das proposições não exista.

   * Se a opção estiver habilitada, a representação da proposta ausente não será exibida e nenhum conteúdo será exibido na mensagem para essa proposta.
   * Se a opção estiver desativada, a mensagem propriamente dita será cancelada durante o envio e os recipients não poderão mais receber mensagens.

Depois de configurar as ofertas para propor no seu email, você pode inseri-las no email usando o Editor de expressão. [Saiba como inserir ofertas no email](#insert)

## Inserir ofertas no email {#insert}

As ofertas podem ser adicionadas ao email usando o Editor de expressão. Podem ser inseridos:

* Na linha de assunto do email,
* No corpo do email, permitindo a personalização em qualquer componente de conteúdo. [Saiba como adicionar componentes de conteúdo](content-components.md)

>[!NOTE]
>
>Antes de inserir uma oferta, verifique se você [configurado quais ofertas propor com o email](#configure).

Para inserir uma oferta usando o Editor de expressão, siga estas etapas:

1. Abra o Editor de expressão e selecione o **[!UICONTROL Propostas]** menu.

   As apresentações disponíveis são exibidas na lista. O número de apresentações é definido ao configurar as ofertas a serem propostas.

   ![](assets/offer-insertion.png)

1. Adicione as apresentações ao assunto ou corpo do email usando os campos de personalização, as funções de renderização ou os atributos de oferta disponíveis para cada apresentação.

   ![](assets/offer-inserted.png)
