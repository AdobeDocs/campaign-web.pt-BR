---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do usuário da Web do Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: b85bf75da466502e4579a061c02a2c4ce4361cd5
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 11%

---

# Personalizar seu conteúdo{#add-personalization}

![](../assets/do-not-localize/badge.png)

Você pode personalizar o conteúdo da mensagem ao:

* Inserção dinâmica **campos de personalização**

   Os campos de personalização são usados para personalização de primeiro nível das mensagens. Você pode selecionar qualquer campo disponível no banco de dados no editor de personalização. Para um delivery, é possível selecionar qualquer campo relacionado ao recipient, à mensagem ou ao delivery. Esses atributos de personalização podem ser inseridos na linha de assunto ou no corpo de suas mensagens.

   ![](assets/perso-subject-line.png)

   A sintaxe a seguir insere a cidade do recipient no conteúdo: &lt;%= recipient.location.city %>.

* Inserção de predefinido **blocos de conteúdo**

   O Campaign vem com um conjunto de blocos de personalização que contêm uma renderização específica que você pode inserir nos deliveries. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para a mirror page da mensagem. Os blocos de conteúdo estão disponíveis em uma entrada dedicada no editor de personalização.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## Personalizar a linha de assunto do email {#personalize-subject-line}

Para adicionar personalização na **[!UICONTROL Linha de assunto]** siga as etapas abaixo:

1. Clique no botão **Abrir caixa de diálogo de personalização** ícone à direita do **Linha de assunto** campo.
1. Insira o conteúdo da linha de assunto e selecione os atributos de personalização a serem adicionados.
1. Clique em **Confirmar** para validar. Os atributos de personalização são adicionados à linha de assunto.

![](assets/perso-subject.png)

## Personalizar seu conteúdo de email {#personalize-emails}

Para personalizar o conteúdo do email, abra a mensagem no Designer de email e:

1. Clique dentro de um bloco de texto.
1. Na barra de ferramentas contextual, selecione **Adicionar personalização**.

   ![](assets/perso-add-to-content.png)

1. Insira o nome do recipient no editor de personalização e confirme.

   ![](assets/perso-add-name.png)

   O atributo de personalização é adicionado ao conteúdo do email.

   Você pode simular o conteúdo para verificar a renderização. [Saiba mais](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

Para adicionar um bloco de conteúdo ao seu email, aplique as mesmas etapas e selecione um bloco de conteúdo do último ícone:

![](assets/perso-insert-block.png)

Depois de inserido, o bloco de conteúdo é adicionado ao conteúdo do email, conforme mostrado abaixo. Ele é adaptado automaticamente ao perfil do recipient quando a personalização é gerada, na etapa de preparação do delivery.

![](assets/perso-content-block-in-email.png)


Os blocos de conteúdo incorporados são:

* **[!UICONTROL Ativado pela Adobe Campaign]**: insere o logotipo &quot;Ativado pela Adobe Campaign&quot;.
* **[!UICONTROL Formatting function for proper nouns]**: gera a função JavaScript **[!UICONTROL toSmartCase]**, que coloca a primeira letra de cada palavra em maiúscula.
* **[!UICONTROL Saudações]**: insere saudações com o nome completo do recipient, seguido de uma vírgula. Exemplo: “Olá, John Doe”.
* **[!UICONTROL Inserir logotipo]**: insere um logotipo que é definido nas configurações de instância.
* **[!UICONTROL Link para mirror page]**: insere um link para o [mirror page](../content/mirror-page.md). O formato padrão é: &quot;Se não conseguir exibir esta mensagem corretamente, clique aqui&quot;.
* **[!UICONTROL Mirror page URL]**: insere o URL da mirror page, permitindo que os designers de delivery verifiquem o link.
* **[!UICONTROL Oferecer o URL de aceitação no modo unitário]**: insere um URL que permite definir uma oferta para **[!UICONTROL Aceite]**. (Este bloco estará disponível se o módulo Interaction estiver habilitado)
* **[!UICONTROL Registration confirmation]**: insere um link que permite confirmar a subscrição.
* **[!UICONTROL Registration link]**: insere um link de subscrição. Esse link é definido nas configurações da instância. O conteúdo padrão é: &quot;Para registrar, clique aqui.&quot;
* **[!UICONTROL Registration link (with referrer)]**: insere um link de subscrição, permitindo identificar o visitante e o delivery. Esse link é definido nas configurações da instância.
* **[!UICONTROL URL da página de registro]**: insere um URL de subscrição
* **[!UICONTROL Estilo de emails de conteúdo]** e **[!UICONTROL Estilo de notificação]**: gere um código que formate um email com estilos de HTML predefinidos.
* **[!UICONTROL Link de cancelamento de assinatura]**: insere um link que permite cancelar a inscrição de todos os deliveries ( lista de bloqueios). O conteúdo associado padrão é: &quot;Você está recebendo esta mensagem porque esteve em contato com ***nome da organização*** ou um afiliado. Para não receber mais mensagens de ***nome da organização*** clique aqui.&quot;



## Personalizar links em seus emails {#personalize-links}

Para personalizar um **link**:

1. Selecione um bloco de texto ou uma imagem.
1. Na barra de ferramentas contextual, selecione **Inserir link**.

   ![](assets/perso-link.png)

1. Insira o rótulo do link e use o **Inserir link** para personalizar o link.

   ![](assets/perso-link-insert-icon.png)

1. Use o editor de personalização para definir e personalizar o link e confirme.

   ![](assets/perso-link-edit.png)


## Personalize suas ofertas {#personalize-offers}

Também é possível acessar o editor de personalização ao adicionar conteúdo do tipo texto às representações das ofertas. Saiba mais [nesta seção](../content/offers.md).
