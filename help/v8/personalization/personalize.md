---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo no Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---


# Personalize seu conteúdo {#add-personalization}

O Personalization de conteúdo de delivery é um recurso essencial que permite personalizar mensagens para recipients individuais, tornando a comunicação mais relevante e envolvente.

No Adobe Campaign, usando os [dados de perfil](#data-personalization), como o nome do perfil, o local ou as interações anteriores e as [variáveis específicas da sua entrega](#variables-personalization), você pode personalizar elementos dinamicamente, como texto, imagens e ofertas, na sua comunicação.

A personalização do delivery não apenas melhora a experiência do usuário, mas também melhora as taxas de engajamento, resultando em mais conversão e satisfação do cliente.

## Uso de dados de perfil para personalização {#data-personalization}

Você pode personalizar qualquer entrega com dados de perfil usando o editor de expressão, que é acessível em campos com o ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**, como a linha de assunto, links de email e componentes de conteúdo de texto/botão. [Saiba como acessar o editor de expressão](gs-personalization.md/#access)

### Sintaxe do Personalization {#syntax}

As marcas Personalization seguem uma sintaxe específica: `<%= table.field %>`. Por exemplo, para inserir o sobrenome do destinatário da tabela de destinatários, use a sintaxe `<%= recipient.lastName %>`.

Durante o processo de preparação do delivery, o Adobe Campaign interpreta automaticamente essas tags e as substitui pelos valores de campo correspondentes para cada recipient. Você pode visualizar a substituição real simulando seu conteúdo.

Ao fazer upload de contatos de um arquivo externo para um delivery de email independente, todos os campos no arquivo de entrada estão disponíveis para personalização. A sintaxe é a seguinte: `<%= dataSource.field %>`.

### Adicionar tags de personalização {#add}

Para adicionar tags de personalização em um delivery, siga estas etapas:

1. Abra o editor de expressão usando o ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**, que pode ser acessado a partir de campos de edição de tipo de texto, como a linha de assunto ou o corpo do SMS. [Saiba como acessar o editor de expressão](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. O editor de expressão se abre. Os campos de personalização disponíveis no banco de dados do Adobe Campaign são organizados em vários menus no lado esquerdo da tela:

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menu | Descrição |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | O menu **[!UICONTROL Aplicativo de assinantes]** lista campos relacionados aos assinantes de um aplicativo, como o terminal usado ou o sistema operacional. *Este menu está disponível somente para notificações por push* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | O menu **[!UICONTROL Destinatário]** lista campos definidos na tabela de destinatários, como nomes, idades ou endereços de destinatários. Ao [carregar contatos de um arquivo externo](../audience/file-audience.md) para uma entrega de email autônoma, este menu lista todos os campos disponíveis no arquivo de entrada. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | O menu **[!UICONTROL Mensagem]** lista campos relacionados aos logs de entrega, incluindo todas as mensagens enviadas aos destinatários ou dispositivos em todos os canais, como a data do último evento com um determinado destinatário |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | O menu **[!UICONTROL Delivery]** lista campos relacionados aos parâmetros necessários para executar deliveries, como canal ou rótulo de entrega. |

   >[!NOTE]
   >
   >Por padrão, cada menu lista todos os campos na tabela selecionada (Recipients, / Message / Delivery). Se quiser incluir campos de tabelas vinculadas à tabela selecionada, habilite a opção **[!UICONTROL Exibir atributos avançados]**, localizada abaixo da lista.

1. Para adicionar um campo de personalização, posicione o cursor no local desejado no conteúdo e clique no botão `+` para inseri-lo.

1. Quando o conteúdo estiver pronto, você poderá salvá-lo e testar a renderização da personalização simulando o conteúdo. O exemplo abaixo mostra a personalização de uma mensagem SMS com os nomes dos recipients.

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Uso de variáveis para personalização {#variables-personalization}

Você também pode usar variáveis para personalizar o delivery.
Saiba mais sobre [adição de variáveis a uma entrega](../advanced-settings/delivery-settings.md#variables-delivery).

Por exemplo, temos a variável `deliveryType` definida como abaixo.

![](assets/variables-deliveryType.png){zoomable="yes"}

Esta variável pode ser usada no conteúdo da entrega usando o ícone **[!UICONTROL Adicionar Personalization]** e a expressão `<%= variables.deliveryType %>` para o nosso exemplo.

![](assets/variables-perso.png){zoomable="yes"}

Você pode verificar o uso da variável com o botão **[!UICONTROL Simular conteúdo]**.

![](assets/variables-simulate.png){zoomable="yes"}
