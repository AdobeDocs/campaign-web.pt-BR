---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo na interface do Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positive"
source-git-commit: 1e5bc39adfeae4f956fc208ef9763eb020552364
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 6%

---


# Personalize seu conteúdo {#add-personalization}

Você pode personalizar qualquer delivery usando o editor de expressão, que é acessível em campos com o **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone, como a linha de assunto, links de email e componentes de conteúdo de texto/botão. [Saiba como acessar o editor de expressão](gs-personalization.md/#access)

## Sintaxe de personalização {#syntax}

As tags de personalização seguem uma sintaxe específica: `<%=table.field%>`. Por exemplo, para inserir o sobrenome do recipient na tabela de recipients, use o `<%= recipient.lastName %>` sintaxe.

Durante o processo de preparação do delivery, o Adobe Campaign interpreta automaticamente essas tags e as substitui pelos valores de campo correspondentes para cada recipient. Você pode visualizar a substituição real simulando seu conteúdo.

## Adicionar tags de personalização {#add}

Para adicionar tags de personalização em um delivery, siga estas etapas:

1. Abra o editor de expressão usando o **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone acessível a partir de campos de edição de tipo de texto, como a linha de assunto ou o corpo do SMS. [Saiba como acessar o editor de expressão](gs-personalization.md/#access)

   ![](assets/perso-access.png)

1. O editor de expressão se abre. Os campos de personalização disponíveis no banco de dados do Adobe Campaign são organizados em vários menus no lado esquerdo da tela:

![](assets/perso-insert-field.png)

| Menu | Descrição |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | A variável **[!UICONTROL Aplicativo de assinantes]** lista os campos relacionados aos assinantes de um aplicativo, como o terminal usado ou o sistema operacional. *Esse menu está disponível somente para notificações por push* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | A variável **[!UICONTROL Recipient]** lista os campos definidos na tabela de recipients, como nomes, idades ou endereços dos recipients. |
| ![](assets/do-not-localize/perso-message-menu.png) | A variável **[!UICONTROL Mensagem]** lista os campos relacionados aos logs do delivery, incluindo todas as mensagens enviadas aos recipients ou dispositivos em todos os canais, como a data do último evento com um determinado recipient |
| ![](assets/do-not-localize/perso-delivery-menu.png) | A variável **[!UICONTROL Entrega]** O menu lista os campos relacionados aos parâmetros necessários para executar deliveries, como canal de delivery ou rótulo. |

>[!NOTE]
>
>Por padrão, cada menu lista todos os campos na tabela selecionada (Recipients, / Message / Delivery). Se quiser incluir campos de tabelas vinculadas à tabela selecionada, ative a opção **[!UICONTROL Exibir atributos avançados]** opção localizada abaixo da lista.

1. Para adicionar um campo de personalização, posicione o cursor no local desejado no conteúdo e clique no `+` botão para inseri-lo.

1. Quando o conteúdo estiver pronto, você poderá salvá-lo e testar a renderização da personalização simulando o conteúdo. O exemplo abaixo mostra a personalização de uma mensagem SMS com os nomes dos recipients.

   *Adicionar a tag de personalização ao conteúdo da mensagem*

   ![](assets/perso-preview1.png)

   *Simular a renderização da personalização para um determinado perfil de teste*

   ![](assets/perso-preview2.png)
