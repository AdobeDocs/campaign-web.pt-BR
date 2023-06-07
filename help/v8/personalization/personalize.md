---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 218f433eb72a0ed928732c96ebee64294daee852
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 79%

---


# Personalize seu conteúdo{#add-personalization}

## Personalizar a linha de assunto de uma mensagem {#personalize-subject-line}

Para adicionar personalização ao campo **[!UICONTROL Linha de assunto]** da mensagem, siga as etapas abaixo:

1. Abra um delivery e clique em **[!UICONTROL Editar conteúdo]**.
1. Clique em **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone à direita do **[!UICONTROL Linha de assunto]** para emails ou o campo **[!UICONTROL Título]** campos para deliveries por push/SMS.

   ![](assets/perso-subject.png){width="600"}

1. Insira a linha de assunto ou o título e selecione os atributos de personalização a serem adicionados.

1. Clique em **[!UICONTROL Confirmar]** para validar. Os atributos de personalização são adicionados ao conteúdo.

## Personalizar seu conteúdo de email {#personalize-emails}

Para personalizar o conteúdo do email, abra a mensagem no Designer de email e:

1. Clique dentro de um bloco de texto.
1. Na barra de ferramentas contextual, selecione **[!UICONTROL Adicionar personalização]**.

   ![](assets/perso-add-to-content.png)

1. Insira o nome do recipient no editor de personalização e confirme.

   ![](assets/perso-add-name.png)

   O atributo de personalização é adicionado ao conteúdo do email.

   Você pode simular o conteúdo para verificar a renderização. [Saiba mais](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

1. Para adicionar um bloco de conteúdo ao seu email, aplique as mesmas etapas e selecione um bloco de conteúdo do último ícone:

   ![](assets/perso-insert-block.png)

1. Depois de inserido, o bloco de conteúdo é adicionado ao conteúdo do email. Ele é adaptado automaticamente ao perfil do destinatário quando a personalização é gerada na etapa de preparação da entrega.

   ![](assets/perso-content-block-in-email.png)

## Personalizar links em seus emails {#personalize-links}

Para personalizar um **link**:

1. Selecione um bloco de texto ou uma imagem.
1. Na barra de ferramentas contextual, selecione **Inserir link**.

   ![](assets/perso-link.png)

1. Insira o rótulo do link e use o botão **Inserir link** para personalizar o link.

   ![](assets/perso-link-insert-icon.png)

1. Use o editor de personalização para definir e personalizar o link e confirme.

   ![](assets/perso-link-edit.png)


## Personalize suas ofertas {#personalize-offers}

Também é possível acessar o editor de personalização ao adicionar conteúdo do tipo texto às representações das ofertas. Saiba mais [nesta seção](../content/offers.md).

