---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: dbb86e2e835ce114cd47380cd256c5873a9eae43
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 64%

---


# Blocos de conteúdo incorporados {#ootb-content-blocks}

O Adobe Campaign oferece uma lista de blocos de conteúdo pré-configurados. Esses blocos de conteúdo são dinâmicos, personalizados e têm uma renderização específica que pode ser inserida em seus deliveries. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para uma mirror page.

Para adicionar um bloco de conteúdo em um delivery, siga estas etapas:

1. Abra um delivery e edite seu conteúdo.

1. Localize o campo onde deseja adicionar um bloco de conteúdo e clique no **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone para abrir o editor de expressão.

   ![](assets/content-block-access.png){width="800" align="center"}

1. No editor de expressão, navegue até o campo **[!UICONTROL Blocos de conteúdo]** menu esquerdo.

1. Para adicionar um bloco de conteúdo, coloque o cursor no local desejado no conteúdo e clique no botão &quot;+&quot; para inseri-lo.

   ![](assets/content-blocks.png){width="800" align="center"}

Os blocos de conteúdo incorporados são:

* **[!UICONTROL Aprovação da personalização Purl]**
* **[!UICONTROL Banner de recusa padrão]**
* **[!UICONTROL Habilitado pelo Adobe Campaign]**: insere o logotipo &quot;Habilitado pelo Adobe Campaign&quot;.
* **[!UICONTROL Pré-inserção do facebook]**
* **[!UICONTROL Formatting function for proper nouns]**: gera a função JavaScript **[!UICONTROL toSmartCase]**, que coloca a primeira letra de cada palavra em maiúscula.
* **[!UICONTROL Saudações]**: insere saudações com o nome completo do recipient, seguido de vírgula. Exemplo: “Olá, fulano,”.
* **[!UICONTROL Inserir logotipo]**: insere um logotipo definido nas configurações de instância.
* **[!UICONTROL Link para mirror page]**: insere um link para a [mirror page](../content/mirror-page.md). O formato padrão é: &quot;Caso não consiga visualizar esta mensagem corretamente, clique aqui.&quot;
* **[!UICONTROL URL de mirror page]**: insere o URL da mirror page, permitindo que os criadores da entrega verifiquem o link.
* **[!UICONTROL Estilo de notificação]**
* **[!UICONTROL Oferecer URL de aceitação no modo unitário]**: insere um URL que permite definir uma oferta como **[!UICONTROL Aceita]**. (Este bloco estará disponível se o módulo Interação estiver habilitado)
* **[!UICONTROL Registration confirmation]**: insere um link que permite confirmar a assinatura.
* **[!UICONTROL Registration link]**: insere um link de assinatura. Esse link é definido nas configurações da instância. O conteúdo padrão é: &quot;Para se registrar, clique aqui&quot;.
* **[!UICONTROL Registration link (with referrer)]**: insere um link de assinatura, permitindo identificar o visitante e a entrega. Esse link é definido nas configurações da instância.
* **[!UICONTROL URL da página de registro]**: insere um URL para assinatura
* Links de compartilhamento de rede social
* **[!UICONTROL Estilo de emails de conteúdo]** e **[!UICONTROL Estilo de notificação]**: geram um código que formata um email com estilos HTML predefinidos.
* **[!UICONTROL Link para cancelar assinatura]**: insere um link que permite cancelar a inscrição de todas as entregas (lista de bloqueios). O conteúdo padrão associado é: &quot;Você está recebendo esta mensagem porque esteve em contato com ***nome da organização*** ou um afiliado. Para não receber mais mensagens de ***nome da organização*** clique aqui.&quot;

>[!NOTE]
>
>Você pode definir novos blocos no console do Adobe Campaign V8 que permitirão otimizar a personalização dos deliveries. [Saiba mais na documentação do console](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/personalizing-deliveries/personalization-blocks.html?lang=pt-BR)
