---
title: Personalizar seu conteúdo no Campaign
description: Saiba como personalizar seu conteúdo no Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 4%

---

# Personalize seu conteúdo {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="Adicionar data atual"
>abstract="Esse menu fornece funções relacionadas à formatação de data que você pode usar para personalizar seu conteúdo."

O Personalization de conteúdo de delivery é um recurso essencial que permite personalizar mensagens para recipients individuais, tornando a comunicação mais relevante e envolvente.

No Adobe Campaign, ao usar os [dados do perfil](#data-personalization), como o nome do perfil, o local ou as interações anteriores e as [variáveis específicas da sua entrega](#variables-personalization), você personaliza dinamicamente elementos como texto, imagens e ofertas na sua comunicação.

A personalização da entrega melhora a experiência do usuário e as taxas de engajamento, resultando em mais conversões e satisfação do cliente.

## Uso de dados de perfil para personalização {#data-personalization}

Personalize qualquer entrega com dados de perfil usando o editor de expressão, que pode ser acessado em campos com o ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**, como a linha de assunto, links de email e componentes de conteúdo de texto/botão. [Saiba como acessar o editor de expressão](gs-personalization.md/#access).

### Sintaxe do Personalization {#syntax}

As marcas Personalization seguem uma sintaxe específica: `<%= table.field %>`. Por exemplo, para inserir o sobrenome do destinatário da tabela de destinatários, use a sintaxe `<%= recipient.lastName %>`.

Durante o processo de preparação do delivery, o Adobe Campaign interpreta essas tags e as substitui pelos valores de campo correspondentes para cada recipient. Você visualiza a substituição real simulando seu conteúdo.

Ao fazer upload de contatos de um arquivo externo para um delivery de email independente, todos os campos no arquivo de entrada estão disponíveis para personalização. A sintaxe é a seguinte: `<%= dataSource.field %>`.

### Adicionar tags de personalização {#add}

Para adicionar tags de personalização em um delivery, siga estas etapas:

1. Abra o editor de expressão usando o ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**, que é acessível a partir de campos de edição de tipo de texto, como a linha de assunto ou o corpo do SMS. [Saiba como acessar o editor de expressão](gs-personalization.md/#access).

   ![Captura de tela mostrando como acessar a caixa de diálogo de personalização](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. O editor de expressão se abre. Os campos de personalização disponíveis no banco de dados do Adobe Campaign são organizados em vários menus no lado esquerdo da tela:

   ![Captura de tela mostrando o menu de campo de personalização](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menu | Descrição |
   |------|-------------|
   | ![Ícone de menu do aplicativo para assinantes](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | O menu **[!UICONTROL Aplicativo de assinantes]** lista campos relacionados aos assinantes de um aplicativo, como o terminal usado ou o sistema operacional. *Este menu está disponível somente para notificações por push.* |
   | ![Ícone do menu Destinatários](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | O menu **[!UICONTROL Destinatário]** lista campos definidos na tabela de destinatários, como nomes, idades ou endereços de destinatários. Ao [carregar contatos de um arquivo externo](../audience/file-audience.md) para uma entrega de email autônoma, este menu lista todos os campos disponíveis no arquivo de entrada. |
   | ![Ícone do menu Mensagem](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | O menu **[!UICONTROL Mensagem]** lista campos relacionados aos logs de entrega, incluindo todas as mensagens enviadas aos destinatários ou dispositivos em todos os canais, como a data do último evento com um determinado destinatário. |
   | ![Ícone do menu de entrega](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | O menu **[!UICONTROL Delivery]** lista campos relacionados aos parâmetros necessários para executar deliveries, como canal ou rótulo de delivery. |

   >[!NOTE]
   >
   >Por padrão, cada menu lista todos os campos na tabela selecionada (Recipients, / Message / Delivery). Se quiser incluir campos de tabelas vinculadas à tabela selecionada, habilite a opção **[!UICONTROL Exibir atributos avançados]**, localizada abaixo da lista.

1. Para adicionar um campo de personalização, posicione o cursor no local desejado no conteúdo e clique no botão `+` para inseri-lo.

1. Quando o conteúdo estiver pronto, salve-o e teste a renderização da personalização simulando o conteúdo. O exemplo abaixo mostra a personalização de uma mensagem SMS com os nomes dos recipients.

   ![Captura de tela mostrando a visualização de personalização de SMS com o nome do recipient](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![Captura de tela mostrando a visualização de personalização de SMS com o nome do recipient](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Uso de variáveis para personalização {#variables-personalization}

Você também usa variáveis para personalizar o delivery. Saiba mais sobre [adição de variáveis a uma entrega](../advanced-settings/delivery-settings.md#variables-delivery).

Por exemplo, a variável `deliveryType` é definida como mostrado abaixo.

![Captura de tela mostrando a definição da variável deliveryType](assets/variables-deliveryType.png){zoomable="yes"}

Esta variável é usada no conteúdo da entrega usando o ícone **[!UICONTROL Adicionar Personalization]** e a expressão `<%= variables.deliveryType %>` para este exemplo.

![Captura de tela mostrando o uso da variável deliveryType na personalização](assets/variables-perso.png){zoomable="yes"}

Verifique o uso da variável com o botão **[!UICONTROL Simular conteúdo]**.

![Captura de tela mostrando a simulação de conteúdo com a variável deliveryType](assets/variables-simulate.png){zoomable="yes"}