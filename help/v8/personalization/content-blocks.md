---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo no Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 45cdd310-7c0c-4b57-bb7f-0576d8eca19d
source-git-commit: 70028ebe3e87498a5ef5778838491d8f964e8e87
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 58%

---

# Adicionar blocos de conteúdo integrados {#ootb-content-blocks}

O Adobe Campaign oferece uma lista de blocos de conteúdo pré-configurados. Esses blocos de conteúdo são dinâmicos, personalizados e têm uma renderização específica que pode ser inserida em seus deliveries. Por exemplo, você pode adicionar um logotipo, uma mensagem de saudação ou um link para uma mirror page.

Para adicionar um bloco de conteúdo em um delivery, siga estas etapas:

1. Abra um delivery e edite seu conteúdo.

1. Localize o campo onde deseja adicionar um bloco de conteúdo e clique no ícone **[!UICONTROL Abrir caixa de diálogo de personalização]** para abrir o editor de expressão.

   ![](assets/content-block-access.png){zoomable="yes"}{width="800" align="center"}

1. No editor de expressão, navegue até o menu esquerdo **[!UICONTROL Blocos de conteúdo]**.

1. Para adicionar um bloco de conteúdo, coloque o cursor no local desejado no conteúdo e clique no botão &quot;+&quot; para inseri-lo.

   ![](assets/content-blocks.png){zoomable="yes"}{width="800" align="center"}

Os blocos de conteúdo incorporados são:

* **[!UICONTROL Banner padrão de recusa]**
* **[!UICONTROL Habilitado pelo Adobe Campaign]**: insere o logotipo &quot;Habilitado pelo Adobe Campaign&quot;.
* **[!UICONTROL Função de formatação para substantivos adequados]**: gera a função JavaScript **[!UICONTROL toSmartCase]**, que coloca a primeira letra de cada palavra em maiúscula.
* **[!UICONTROL Saudações]**: insere saudações com o nome completo do destinatário, seguido de vírgula. Exemplo: “Olá, fulano,”.
* **[!UICONTROL Inserir Logotipo]**: insere um logotipo definido nas configurações de instância.
* **[!UICONTROL Link para mirror page]**: insere um link para a [mirror page](../email/mirror-page.md). O formato padrão é: &quot;Caso não consiga visualizar esta mensagem corretamente, clique aqui.&quot;
* **[!UICONTROL URL de mirror page]**: insere o URL da mirror page, permitindo que os criadores da entrega verifiquem o link.
* **[!UICONTROL Estilo de notificação]**
* **[!UICONTROL Oferecer URL de aceitação no modo unitário]**: insere um URL que permite definir uma oferta como **[!UICONTROL Aceita]**. (Este bloco estará disponível se o módulo Interação estiver habilitado)
* **[!UICONTROL Registration confirmation]**: insere um link que permite confirmar a assinatura.
* **[!UICONTROL Registration link]**: insere um link de assinatura. Esse link é definido nas configurações da instância. O conteúdo padrão é: &quot;Para se registrar, clique aqui&quot;.
* **[!UICONTROL Registration link (with referrer)]**: insere um link de assinatura, permitindo identificar o visitante e a entrega. Esse link é definido nas configurações da instância.
* **[!UICONTROL URL da página de registro]**: insere um URL para assinatura
* Links de compartilhamento de redes sociais
* **[!UICONTROL Estilo de emails de conteúdo]** e **[!UICONTROL Estilo de notificação]**: geram um código que formata um email com estilos HTML predefinidos.
* **[!UICONTROL Link para cancelar assinatura]**: insere um link que permite cancelar a inscrição de todas as entregas (lista de bloqueios). O conteúdo padrão associado é: &quot;Você está recebendo esta mensagem porque esteve em contato com ***nome da organização*** ou um afiliado. Para não receber mais mensagens de ***nome da organização*** clique aqui.&quot;

>[!NOTE]
>
>Você pode definir novos blocos no console do Adobe Campaign v8 que permitem otimizar a personalização de deliveries. Saiba mais na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/personalize/personalization-blocks.html#create-custom-personalization-blocks){target="_blank"}.
