---
audience: end-user
title: Rastrear suas mensagens
description: Saiba como adicionar links e rastrear mensagens enviadas
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: 8398c0cacb2e6e2198e295787bb5e4e25af74e6e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 3%

---

# Adicionar links e rastrear mensagens {#tracking}

![](../assets/do-not-localize/badge.png)

Use o Designer de email para adicionar links ao seu conteúdo e rastrear as mensagens enviadas para monitorar o comportamento dos recipients.

## Inserir links {#insert-links}

Ao criar uma mensagem, você pode adicionar links ao seu conteúdo.

>[!NOTE]
>
>Quando o rastreamento é ativado, todos os links incluídos no conteúdo da mensagem são rastreados.

Para inserir links no seu conteúdo de email, siga as etapas abaixo:

1. Selecione um elemento e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![](assets/message-tracking-insert-link.png)

1. Adicione um **[!UICONTROL Rótulo]** e **[!UICONTROL Link]**.

1. Salve as alterações.

1. Depois que o link for criado, você ainda poderá modificá-lo da variável **[!UICONTROL Configurações do componente]** painel à direita.

   * Você pode editar o link e alterar seu **[!UICONTROL Target]**.
   * Você pode optar por sublinhar o link ou não, marcando a opção correspondente.

   ![](assets/message-tracking-link-settings.png)

>[!NOTE]
>
>As mensagens de email de tipo de marketing devem incluir um link para opção de não participação, que não é necessário para mensagens transacionais. A categoria da mensagem (**[!UICONTROL Marketing]** ou **[!UICONTROL Transacional]**) é definida no nível da superfície do canal (ou seja, predefinição de mensagem) e ao criar a mensagem.

## Link para uma mirror page {#mirror-page}

A mirror page é uma página HTML acessível online através de um navegador da Web. Seu conteúdo é idêntico ao conteúdo do email.

Para adicionar um link a uma mirror page no seu email:

1. Selecione um elemento e clique em **[!UICONTROL Inserir link]** na barra de ferramentas contextual.

   ![](assets/message-tracking-mirror-page.png)

1. Selecione o **[!UICONTROL Inserir link]** para acessar o menu de personalização.

   ![](assets/message-tracking-mirror-page_2.png)

1. No **[!UICONTROL Bloco de conteúdo]** selecione **[!UICONTROL Mirror page URL]** e clique em **[!UICONTROL Adicionar]**.

   ![](assets/message-tracking-mirror-page_3.png)

A mirror page é criada automaticamente.

>[!IMPORTANT]
>
>Os links de mirror pages são gerados automaticamente e não podem ser editados. Eles contêm todos os dados personalizados criptografados necessários para renderizar o email original. Como resultado, o uso de atributos personalizados com valores grandes pode gerar URLs de mirror pages longas, o que pode impedir que o link funcione em navegadores da Web com tamanho máximo de URLs.

Depois que o email for enviado, quando os recipients clicarem no link da mirror page, o conteúdo do email será exibido no navegador padrão.

>[!NOTE]
>
>No email de teste enviado aos perfis de teste, o link para a mirror page não está ativo. Ela só é ativada nas mensagens finais.

O período de retenção de uma mirror page é de 60 dias. Após esse atraso, a mirror page não estará mais disponível.

## Gerenciar rastreamento {#manage-tracking}

O [Email Designer](create-email-content.md) permite gerenciar os URLs rastreados, como editar o tipo de rastreamento para cada link.

1. Clique no botão **[!UICONTROL Links]** ícone do painel esquerdo para exibir a lista de todos os URLs do seu conteúdo que serão rastreados.

   Essa lista permite que você tenha uma visualização centralizada e localize cada URL no conteúdo do email.

1. Para editar um link, clique no ícone de lápis correspondente.

   ![](assets/message-tracking-edit-links.png)

1. Você pode modificar o **[!UICONTROL Tipo de rastreamento]** se necessário:

   ![](assets/message-tracking-edit-a-link.png)

   Para cada URL rastreado, é possível definir o modo de rastreamento para um destes valores:

   * **[!UICONTROL Rastreado]**: Ativa o rastreamento nesse URL.
   * **[!UICONTROL Recusar]**: Considera esse URL como recusa ou cancelamento de subscrição.
   * **[!UICONTROL Mirror page]**: Considera esse URL como sendo de mirror page.
   * **[!UICONTROL Nunca]**: Nunca ativa o rastreamento desse URL. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Adicione um **[!UICONTROL Categoria]** ao link para agrupar links rastreados e clicar em **[!UICONTROL Salvar]**.

   ![](assets/message-tracking-edit-a-link_2.png)

1. Após enviar o delivery, acesse o relatório do delivery. Em **[!UICONTROL Rastreamento]** , o **[!UICONTROL Fluxos de clique e URLs]** exibe quais URLs do seu delivery são os mais visitados. [Saiba mais](../reporting/reports.md)
