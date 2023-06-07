---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
source-git-commit: 573f0bbf396f795029c5e34b436521cb1c7b80a5
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 100%

---


# Blocos de conteúdo incorporados {#ootb-content-blocks}

Os blocos de conteúdo incorporados são:

* **[!UICONTROL Habilitado pelo Adobe Campaign]**: insere o logotipo &quot;Habilitado pelo Adobe Campaign&quot;.
* **[!UICONTROL Formatting function for proper nouns]**: gera a função JavaScript **[!UICONTROL toSmartCase]**, que coloca a primeira letra de cada palavra em maiúscula.
* **[!UICONTROL Saudações]**: insere saudações com o nome completo do recipient, seguido de vírgula. Exemplo: “Olá, fulano,”.
* **[!UICONTROL Inserir logotipo]**: insere um logotipo, que é definido nas configurações de instância.
* **[!UICONTROL Link para mirror page]**: insere um link para a [mirror page](../content/mirror-page.md). O formato padrão é: &quot;Caso não consiga visualizar esta mensagem corretamente, clique aqui.&quot;
* **[!UICONTROL URL de mirror page]**: insere o URL da mirror page, permitindo que os criadores da entrega verifiquem o link.
* **[!UICONTROL Oferecer URL de aceitação no modo unitário]**: insere um URL que permite definir uma oferta como **[!UICONTROL Aceita]**. (Este bloco estará disponível se o módulo Interação estiver habilitado)
* **[!UICONTROL Registration confirmation]**: insere um link que permite confirmar a assinatura.
* **[!UICONTROL Registration link]**: insere um link de assinatura. Esse link é definido nas configurações da instância. O conteúdo padrão é: &quot;Para se registrar, clique aqui&quot;.
* **[!UICONTROL Registration link (with referrer)]**: insere um link de assinatura, permitindo identificar o visitante e a entrega. Esse link é definido nas configurações da instância.
* **[!UICONTROL URL da página de registro]**: insere um URL para assinatura
* **[!UICONTROL Estilo de emails de conteúdo]** e **[!UICONTROL Estilo de notificação]**: geram um código que formata um email com estilos HTML predefinidos.
* **[!UICONTROL Link para cancelar assinatura]**: insere um link que permite cancelar a inscrição de todas as entregas (lista de bloqueios). O conteúdo padrão associado é: &quot;Você está recebendo esta mensagem porque esteve em contato com ***nome da organização*** ou um afiliado. Para não receber mais mensagens de ***nome da organização*** clique aqui.&quot;
