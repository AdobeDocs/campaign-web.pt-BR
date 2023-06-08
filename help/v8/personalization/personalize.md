---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: b8b1cb62c11b66eaade5937fa798d58a9c376127
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 36%

---


# Personalize seu conteúdo{#add-personalization}

A personalização pode ser adicionada a qualquer delivery usando o editor de expressão.

Uma tag de personalização sempre usa a seguinte sintaxe: `<%=table.field%>`Por exemplo, para inserir o nome do recipient, armazenado na tabela de recipients, a tag de personalização usa a sintaxe &lt;%= recipient.lastName %>.

Quando um delivery é preparado, essas tags são interpretadas automaticamente pelo Adobe Campaign e substituídas pelo valor do campo para um determinado recipient. A substituição física pode ser exibida ao simular o conteúdo.

Para adicionar tags de personalização a um delivery, clique no ícone Open personalization dialog que é acessível a partir de campos de edição de tipo de texto, como a linha de assunto ou o corpo do SMS.

![](assets/perso-access.png)

O editor de expressão é exibido. Os campos de personalização são organizados em três menus, localizados à esquerda da tela. Esses menus dão acesso a todos os campos disponíveis no banco de dados do Adobe Campaign.

| Menu | Descrição |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | A variável **[!UICONTROL Recipient]** lista todos os campos definidos na tabela de recipients, como nome, idade ou endereço dos recipients. |
| ![](assets/do-not-localize/perso-message-menu.png) | A variável **[!UICONTROL Mensagem]** lista todos os campos relacionados aos logs do delivery, ou seja, todas as mensagens enviadas aos recipients ou dispositivos em todos os canais, como a data do último evento com um determinado recipient |
| ![](assets/do-not-localize/perso-delivery-menu.png) | A variável **[!UICONTROL Entrega]** O menu lista todos os campos relacionados aos parâmetros necessários para executar deliveries, como canal de delivery, rótulo, etc. |

>[!NOTE]
>
>Por padrão, a lista mostra todos os campos na tabela selecionada (Recipients, / Message / Delivery). Se quiser incluir campos de tabelas vinculadas à tabela selecionada, ative a opção **[!UICONTROL Exibir atributos avançados]** opção localizada abaixo da lista.

Para adicionar um campo de personalização, coloque o cursor no local desejado no conteúdo e clique no botão + para inseri-lo.

![](assets/perso-insert-field.png)

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


## Personalize suas ofertas {#personalize-offers}

Também é possível acessar o editor de personalização ao adicionar conteúdo do tipo texto às representações das ofertas. Saiba mais [nesta seção](../content/offers.md).

