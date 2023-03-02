---
audience: end-user
title: Envie seu primeiro email
description: Saiba como enviar seu primeiro email com a interface do Campaign Web
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 4332facf1b7853cb36c9de752ff48bb68e97d6e0
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 1%

---

# Envie seu primeiro email {#first-email}

![](../assets/do-not-localize/badge.png)

Saiba como criar seu primeiro email direcionado. Nesse caso de uso, você agenda o envio de um email para os membros de fidelidade Silver e Gold em uma data específica.

Com base em um modelo de design predefinido, o email também apresenta conteúdo personalizado com base nos atributos do perfil do cliente.

![](assets/delivery-list.png)

## Criar o email {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Selecionar um modelo de email"
>abstract="Um template de email é uma configuração de delivery específica que contém configurações predefinidas, como regras de tipologia, parâmetros de personalização ou roteamento. Os templates são definidos no console do cliente do Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Propriedades de email"
>abstract="As propriedades são os parâmetros comuns do delivery que ajudam a nomear e classificar o delivery. Se o seu delivery for baseado em um schema estendido definido no console do Adobe Campaign v8, alguns **Opções personalizadas** campos estão disponíveis."

1. Para criar um novo delivery, vá para a **[!UICONTROL Entregas]** e selecione **[!UICONTROL E-mail]** como canal.

1. Selecione o template que deseja usar e clique em **[!UICONTROL Criar entrega]**.

   >[!NOTE]
   >
   >Os modelos são configurações de entrega pré-definidas salvas para uso futuro. Eles podem ser criados por usuários administradores no console do Adobe Campaign. [Saiba como trabalhar com modelos de entrega](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. Forneça um rótulo para o email e configure opções adicionais com base nas suas necessidades:

   * **[!UICONTROL Nome interno]**: atribuir um identificador exclusivo ao delivery,
   * **[!UICONTROL Pasta]**: armazene o delivery em uma pasta específica,
   * **[!UICONTROL Código de entrega]**: use esse campo para organizar seus deliveries com base em sua própria convenção de nomenclatura,
   * **[!UICONTROL Descrição]**: especifique uma descrição para o delivery,
   * **[!UICONTROL Natureza]**: especifique a natureza do email para fins de classificação.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Se você tiver estendido seu esquema com campos personalizados específicos, poderá acessá-los na **[!UICONTROL Opções personalizadas]** seção.

   ![](assets/email-properties.png)

   Além disso, as configurações avançadas, como regras de tipologia e mapeamentos de público-alvo, podem ser acessadas clicando no botão localizado ao lado do nome do delivery. Essas configurações são pré-definidas no modelo selecionado, mas podem ser editadas conforme necessário para esse email específico.

## Criar o conteúdo do email {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Saiba como criar conteúdo de email"
>abstract="Saiba como usar o Designer de email."

Nesse caso de uso, você usa um modelo predefinido para criar nosso email.

Instruções detalhadas sobre como configurar o conteúdo de email estão disponíveis em [nesta seção](../content/edit-content.md).

1. Para começar a criar o conteúdo de email, clique no link **[!UICONTROL Editar conteúdo]** botão.

   Isso leva você a uma interface dedicada, onde é possível configurar o conteúdo de email e projetá-lo usando o Designer de email.

   ![](assets/edit-content.png)

1. Insira a linha de assunto do seu email e personalize-a usando o Editor de expressão. [Saiba como personalizar seu conteúdo](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Para projetar o corpo do email, clique no link **[!UICONTROL Editar corpo do email]** botão.

   Escolha o método a ser usado para criar o conteúdo de email. Neste exemplo, use um modelo de design predefinido.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Após selecionar o template, ele será exibido no Designer de email, onde você poderá fazer as edições necessárias e adicionar personalização.

   Por exemplo, para adicionar personalização ao título do email, selecione o bloco de componentes e clique em **[!UICONTROL Adicionar personalização]**.

   ![](assets/add-perso.png)

1. Quando estiver satisfeito com o conteúdo, salve e feche o design. Clique em **[!UICONTROL Salvar]** para retornar à tela de criação do email.

   ![](assets/save-content.png)

## Definir a audiência {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definir a audiência"
>abstract="Selecione o melhor público para sua mensagem de marketing. Você pode escolher um público-alvo existente já definido em uma instância do Campaign v8 ou no Adobe Experience Platform, ou criar um novo público-alvo com o construtor de regras."

Nesse caso de uso, você envia o email para um público-alvo existente. Instruções adicionais sobre como trabalhar com públicos-alvo estão disponíveis em [nesta seção](../audience/about-audiences.md).

1. Para selecionar o público do email, clique no link **[!UICONTROL Selecionar público]** e escolha um público-alvo na lista.

   Neste exemplo, queremos usar um público-alvo existente direcionado a clientes pertencentes aos níveis de pontos de fidelidade prata e ouro.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Os públicos-alvo disponíveis na lista são originários da instância do Campaign v8 ou da Adobe Experience Platform se a integração Destino/Fontes tiver sido configurada na instância.
   >
   >A integração Destino / Fontes permite enviar segmentos de Experience Platform para o Adobe Campaign e enviar a entrega do Campaign e os logs de rastreamento para o Adobe Experience Platform. [Saiba como trabalhar com o Campaign e o Adobe Experience Platform](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. Depois que o público-alvo for selecionado, você poderá refinar ainda mais o público-alvo aplicando regras adicionais.

   Você também pode definir um grupo de controle para analisar o comportamento dos recipients de email em comparação àqueles que não foram direcionados. [Saiba como trabalhar com grupos de controle](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Agendar o envio {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Agendar o envio"
>abstract="Defina a data e a hora exata do envio. Ao escolher a hora mais apropriada para sua mensagem de marketing, você pode maximizar as taxas de abertura."

Para agendar o envio do email, clique em **[!UICONTROL Ativar]** e defina a data e a hora desejadas para o envio.

Por padrão, a variável **[!UICONTROL Confirmar antes de enviar]** estiver ativada, exigindo que você confirme o envio antes que o email seja enviado na data e hora agendadas. Se desejar enviar o email automaticamente na data e hora agendadas, você pode desativar essa opção.

![](assets/schedule.png)

## Pré-visualizar e testar o email {#preview-test}

Antes de enviar o email, você pode visualizá-lo e testá-lo para garantir que ele atenda às suas expectativas.

Nesse caso de uso, você pré-visualiza o email e envia versões de teste para endereços de email específicos enquanto representa alguns dos perfis direcionados.

Informações adicionais sobre como pré-visualizar e testar emails estão disponíveis em [nesta seção](../preview-test/preview-test.md).

1. Para revisar e enviar o email, clique em **[!UICONTROL Revisar e enviar]**. Isso exibirá uma pré-visualização do email, juntamente com todas as propriedades, o público-alvo e o agendamento configurados. Você pode editar qualquer um desses elementos clicando no botão modify.

1. Para visualizar o email e enviar versões de teste, clique no link **[!UICONTROL Simular conteúdo]** botão.

   ![](assets/review-email.png)

1. No lado esquerdo, selecione os perfis que deseja usar para visualizar o email.

   O painel direito exibe uma pré-visualização do email com base no perfil selecionado. Se você tiver adicionado vários perfis, é possível alternar entre eles para visualizar o email correspondente.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Para enviar versões de teste do seu email, clique no link **[!UICONTROL Teste]** e escolha o modo que deseja usar.

   Neste exemplo, use o **[!UICONTROL Substituir do público alvo principal]** que envia versões de teste para endereços de email específicos enquanto representa alguns dos perfis direcionados pelo email.

   ![](assets/proof-mode.png)

1. Clique em **[!UICONTROL Adicionar endereço]** e especifique os endereços de email que receberão as versões de teste.

   Para cada endereço de email, selecione o perfil que será representado. Você também pode permitir que o Adobe Campaign selecione um perfil aleatório no público-alvo.

   ![](assets/proof-test-profile.png)

1. Clique em **[!UICONTROL Enviar email de teste]** e confirme o envio.

   As versões de teste são enviadas para os endereços de email especificados usando o perfil selecionado com o **[Prova x]** prefixo.

   ![](assets/proof-sent.png)

   Você pode verificar o status do envio e acessar os emails de teste enviados a qualquer momento clicando no link **[!UICONTROL Exibir log de email de teste]** botão na tela simular conteúdo.

## Enviar e monitorar o email {#prepare-send}

Depois de revisar e testar o email, você pode iniciar a preparação e enviá-lo.

1. Para iniciar a preparação do email, clique em **[!UICONTROL Preparar]**. [Saiba como preparar um email](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Quando o email estiver pronto para ser enviado, clique no link **[!UICONTROL Enviar]** botão (ou **[!UICONTROL Enviar conforme agendado]** se você tiver programado o envio) e confirme o envio.

1. Durante o processo de envio, você pode acompanhar o progresso e exibir estatísticas em tempo real diretamente nesta tela.

   ![](assets/sent-mail.png)

   Também é possível acessar informações detalhadas sobre o envio clicando no link **[!UICONTROL Logs]** botão. [Saiba como monitorar logs do delivery](../monitor/delivery-logs.md)

1. Depois que o email for enviado, você poderá acessar relatórios dedicados para análise adicional clicando no link **[!UICONTROL Relatórios]** botão.

![](assets/reports.png)
