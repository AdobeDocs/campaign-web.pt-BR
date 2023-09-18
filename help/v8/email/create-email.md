---
audience: end-user
title: Enviar seu primeiro email
description: Saiba como enviar seu primeiro email com a interface do Campaign Web
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
badge: label="Beta"
source-git-commit: 4fdeaacaa2998bf66b53fd93857bd14d65b98b33
workflow-type: tm+mt
source-wordcount: '1354'
ht-degree: 67%

---


# Enviar seu primeiro email {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_card2"
>title="IA generativa para conteúdo de email"
>abstract="Nossa tecnologia de IA generativa utiliza algoritmos avançados para gerar um conteúdo personalizado altamente envolvente. Promova maiores taxas de abertura, taxas de click-through e conversões com a geração de conteúdo inteligente da IA generativa. Mantenha-se à frente da concorrência e eleve seu marketing por email com a IA generativa para conteúdo de email."

Saiba como criar seu primeiro email direcionado. Nesse caso de uso, você agendará uma data específica para o envio de um email para membros do programa de fidelidade de nível prata e ouro.

Com base em uma configuração [modelo de design](../content/email-sample-templates.md), o email também apresenta conteúdo personalizado com base nos atributos do perfil do cliente.

## Criar o delivery de email {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Selecionar um modelo de email"
>abstract="Um modelo de email é uma configuração específica de entrega que contém configurações predefinidas, como regras de tipologia, personalização ou parâmetros de roteamento. Os modelos são definidos no console do cliente do Campaign."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Definir suas propriedades de email"
>abstract="As propriedades são os parâmetros de entrega comuns que ajudam a nomear e classificar a entrega. As configurações adicionais são opcionais. Se a entrega for baseada em um schema estendido definido no console do Adobe Campaign v8, alguns campos de **Opções personalizadas** estarão disponíveis."

Você pode criar um delivery de email independente ou criar um email no contexto de um workflow da campanha. As etapas abaixo detalham o procedimento para um delivery de email independente (único). Se estiver trabalhando no contexto de um workflow da campanha, as etapas de criação serão detalhadas em [nesta seção](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Para criar um novo delivery de email independente, siga as etapas abaixo.

1. Navegue até o **[!UICONTROL Entregas]** no painel à esquerda e clique no botão  **[!UICONTROL Criar entrega]** botão.

   ![](assets/delivery-list.png)

1. Selecionar **[!UICONTROL E-mail]** como canal e escolha um template do delivery de email na lista.

   >[!NOTE]
   >
   >Os templates são configurações de entrega predefinidas salvas para uso futuro. [Saiba mais](../msg/delivery-template.md)

   ![](assets/channel-template.png)

1. Clique no botão **[!UICONTROL Criar entrega]** para confirmar.
1. Insira um rótulo para a entrega e configure as opções adicionais com base em suas necessidades:

   * **[!UICONTROL Nome interno]**: atribui um identificador exclusivo à entrega.
   * **[!UICONTROL Pasta]**: armazena a entrega em uma pasta específica.
   * **[!UICONTROL Código de entrega]**: use esse campo para organizar suas entregas com base em sua própria convenção de nomeação.
   * **[!UICONTROL Descrição]**: especifica uma descrição da entrega.
   * **[!UICONTROL Natureza]**: especifica a natureza do email para fins de classificação.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Se tiver estendido seu schema com campos personalizados específicos, será possível acessá-los na seção **[!UICONTROL Opções personalizadas]**.

   ![](assets/email-properties.png)

1. Além disso, as configurações avançadas, como regras de tipologia e target mappings, podem ser acessadas por meio do **[!UICONTROL Configurações]** localizado na parte superior direita da tela. Essas definições são pré-configuradas no modelo selecionado, mas podem ser editadas conforme necessário para esse email específico. [Saiba mais](../advanced-settings/delivery-settings.md)

## Definir o público {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Selecionar um público-alvo para a entrega"
>abstract="Selecione o melhor público para a sua mensagem de marketing. Você pode escolher um público-alvo existente (já definido em uma instância do Campaign v8 ou no Adobe Experience Platform), criar um novo público-alvo usando o construtor de regras ou fazer upload de um arquivo contendo seu público-alvo. Os grupos de controle não estão habilitados para o **Selecionar do arquivo** e vice-versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="Selecionar os públicos principais"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/control-group.html" text="Configurar um grupo de controle"

Nesse caso de uso, você enviará o email para um público existente.

Instruções adicionais sobre como trabalhar com públicos estão disponíveis [nesta seção](../audience/about-audiences.md).

1. Para selecionar o público do email, clique no botão **[!UICONTROL Selecionar público-alvo]** e escolha um público existente na lista.

   Neste exemplo, queremos usar um público existente direcionado a clientes que pertencem aos níveis prata e ouro do programa de fidelidade.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Os públicos disponíveis na lista são originários da instância do Campaign v8 ou da Adobe Experience Platform se a integração Destino/Origem tiver sido configurada na instância. Essa integração permite enviar segmentos de Experience Platform para o Adobe Campaign e enviar o delivery do Campaign e os logs de rastreamento para o Adobe Experience Platform. Saiba como trabalhar com o Campaign e o Adobe Experience Platform na [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. Depois que o público é selecionado, você pode refinar o público alvo aplicando regras adicionais.

   ![](assets/audience-selected.png)

1. Você também pode definir um grupo de controle para analisar o comportamento dos recipients de email, em comparação com aqueles que não foram direcionados. [Saiba como trabalhar com grupos de controle](../audience/control-group.md)

## Definir o conteúdo do email {#create-content}

Para começar a criar seu conteúdo de email, siga as etapas abaixo. Nesse caso de uso, você usa um email predefinido [template do delivery](../msg/delivery-template.md) para criar seu email.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../content/edit-content.md).-->

1. No painel de delivery de email, clique no link **[!UICONTROL Editar conteúdo]** botão.

   ![](assets/email-edit-content.png)

   Isso leva você a uma interface dedicada, onde é possível configurar o conteúdo de email e acessar o Designer de email. [Saiba mais](../content/edit-content.md)

   ![](assets/edit-content.png)

1. Insira a linha de assunto do email e personalize-a usando o Editor de expressão. [Saiba como personalizar o conteúdo](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Para criar o conteúdo do email, clique no botão **[!UICONTROL Editar corpo do email]**.

   Escolha o método a ser usado para criar o conteúdo de email. Neste exemplo, use um [modelo de conteúdo predefinido](../content/email-sample-templates.md).

   ![](assets/select-template.png)

1. Depois de selecionar o modelo, ele será exibido no [Email Designer](../content/create-email-content.md), em que você pode fazer as edições necessárias e adicionar personalização.

   Por exemplo, para personalizar o título do email, selecione o bloco de componentes e clique em **[!UICONTROL Adicionar personalização]**.

   ![](assets/add-perso.png)

1. Quando estiver satisfeito com o conteúdo, salve e feche o design. Clique em **[!UICONTROL Salvar]** para retornar à tela de criação do email.

   ![](assets/save-content.png)

## Agendar o envio {#schedule}

Para agendar o envio do email, siga as etapas abaixo.

Instruções adicionais sobre como agendar o envio do delivery são detalhadas em [nesta seção](../msg/gs-messages.md#gs-schedule).

1. Navegue até o **[!UICONTROL Agendar]** seção.

1. Use o **[!UICONTROL Ativar agendamento]** para ativá-la.

1. Defina a data e a hora desejadas para envio.

   ![](assets/schedule.png)

Após enviar a entrega, o envio só será realizado na data de contato definida.

## Visualizar e testar o email {#preview-test}

Antes de enviar um email, você pode visualizá-lo e testá-lo para garantir que ele atenda às suas expectativas.

Nesse caso de uso, você visualizará o email e enviará as versões de teste para endereços de email específicos como representações de alguns dos perfis direcionados.

Informações adicionais sobre como visualizar e testar emails estão disponíveis [nesta seção](../preview-test/preview-test.md).

1. Para revisar seu email, clique em **[!UICONTROL Revisar e enviar]**. Isso exibe uma visualização do email, juntamente com todas as propriedades, o público e o agendamento configurados. Você pode editar qualquer um desses elementos clicando no botão Modificar.

1. Para visualizar o email e enviar versões de teste, clique no link **[!UICONTROL Simular conteúdo]** botão.

   ![](assets/review-email.png)

1. No lado esquerdo, selecione os perfis que deseja usar para visualizar o email.

   O painel direito exibe uma visualização do email com base no perfil selecionado. Se você tiver adicionado vários perfis, é possível alternar entre eles para visualizar o email correspondente.

   ![](assets/preview.png)

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Para enviar versões de teste do seu email, clique no botão **[!UICONTROL Teste]** e escolha o modo que deseja usar.

   Neste exemplo, use o modo **[!UICONTROL Substituir do público alvo principal]**, que envia versões de teste para endereços de email específicos como representações de alguns dos perfis direcionados pelo email.

   ![](assets/proof-mode.png)

1. Clique em **[!UICONTROL Adicionar endereço]** e especifique os endereços de email que receberão as versões de teste.

   Para cada endereço de email, selecione o perfil a ser representado. Você também pode permitir que o Adobe Campaign selecione um perfil aleatório do público alvo.

   ![](assets/proof-test-profile.png)

1. Clique em **[!UICONTROL Enviar email de teste]** e confirme o envio.

   As versões de teste são enviadas para os endereços de email especificados usando o perfil selecionado com o prefixo **[Prova x]**.

   ![](assets/proof-sent.png)

   Você pode verificar o status do envio e acessar os emails de teste enviados a qualquer momento clicando no botão **[!UICONTROL Exibir log de email de teste]** na tela Simular conteúdo.

## Enviar e monitorar o email {#prepare-send}

Após revisar e testar seu email, você pode iniciar sua preparação e envio.

1. Para iniciar a preparação do email, clique em **[!UICONTROL Preparar]**. [Saiba como preparar um email](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Depois que o email estiver pronto para ser enviado, clique no botão **[!UICONTROL Enviar]** (ou em **[!UICONTROL Enviar conforme agendado]** caso tenha agendado seu envio) e confirme o envio.

1. Durante o processo de envio, você pode acompanhar seu progresso e exibir estatísticas em tempo real diretamente nessa tela.

   ![](assets/sending-email.png)

   <!--
    ![](assets/sent-email.png)-->

   Você também pode acessar informações detalhadas sobre o envio clicando no botão **[!UICONTROL Logs]**. [Saiba como monitorar os logs de entrega](../monitor/delivery-logs.md)

1. Depois que o email tiver sido enviado, você poderá acessar os relatórios dedicados para análise adicional clicando no botão **[!UICONTROL Relatórios]**.

![](assets/reports.png)
