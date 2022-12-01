---
audience: end-user
title: Criar seu primeiro email
description: Documentação da Web do Campaign v8
source-git-commit: cdddef89cda4fa39cee38e9d0171a6ea395537c7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 1%

---

# Enviar seu primeiro email {#first-email}

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

Este caso de uso apresenta como criar seu primeiro email

Neste exemplo, vamos agendar o envio de um email em uma data específica para clientes de fidelidade prata e ouro. Esse email será projetado usando um template HTML predefinido de um arquivo ZIP e incluirá a personalização usando os atributos do perfil.

![](assets/delivery-list.png)

## Criar o email {#create-email}

1. Crie um novo delivery a partir do **[!UICONTROL Deliveries]** menu.
1. Selecione o **[!UICONTROL Email]** e o modelo a ser usado e clique em **[!UICONTROL Criar]**.

   >[!NOTE]
   >
   >informações sobre templates. verificar informações no documento V7

   ![](assets/channel-template.png)

1. Forneça um rótulo para o delivery e configure opções adicionais dependendo de suas necessidades:

   * Nome interno:
   * Pasta:
   * Código de entrega:
   * Descrição:
   * Natureza:

   verifique quais configurações estão definidas no modelo e as mencione (descrição? pasta?, natureza?)

   ![](assets/email-properties.png)

   >[!NOTE]
   >
   >informações sobre o botão de configurações do delivery + link para doc

## Criar o conteúdo do email {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Crie seu primeiro conteúdo de email usando o Designer de email."
>abstract="Criar seu primeiro conteúdo de email"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="Criar o conteúdo do email"
>abstract="TBC"

1. Clique no botão **[!UICONTROL Editar conteúdo]** para começar a criar o conteúdo do email.

   Essa tela permite que você configure o conteúdo do email e o projete usando o Designer de email.

   ![](assets/edit-content.png)

   >[!NOTE]
   >
   >O nome de formulário e as informações de email de De são predefinidos no modelo de email selecionado.
   >
   >Por padrão, o rastreamento de email é ativado para aberturas e cliques. Para desativar essas opções, desmarque-as na seção Recursos opcionais .

1. Especifique o assunto do seu email usando o Editor de expressão. [Saiba como personalizar seu conteúdo](../personalization/personalize.md)

   Neste exemplo, queremos personalizar a linha de assunto usando o nome dos perfis.

   ![](assets/subject-line.png)

1. Adicione um arquivo anexado ao seu email, se necessário. Saiba como editar conteúdo de email

1. Clique no botão **[!UICONTROL Editar corpo do email]** para criar e criar o conteúdo do email.

   Escolha o método a ser usado para criar o conteúdo de email. Neste exemplo, queremos importar um conteúdo HTML existente.

   ![](assets/import-html.png)

1. Selecione o HTML ou arquivo ZIP a ser importado e clique em **[!UICONTROL Próximo]**.

   Se a pasta contiver ativos, escolha a instância e a pasta em que eles devem ser armazenados e clique em **[!UICONTROL Importar]**. (+ link para documento sobre ativos?)

   ![](assets/import-folder.png)

1. Depois que o conteúdo é importado, ele é exibido no Designer de email, permitindo que você o edite, se necessário, e adicione personalização.

   Neste exemplo, queremos adicionar personalização ao título do email. Para fazer isso, selecione o bloco de componentes e clique em **[!UICONTROL Adicionar personalização]**.

   ![](assets/add-perso.png)

1. Quando o conteúdo estiver pronto, salve-o e clique na seta para voltar à tela de criação de email.

   ![](assets/save-content.png)

## Definir a audiência {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Definir a audiência"
>abstract="TBC"

1. Clique no botão **[!UICONTROL Seleção do público-alvo]** em seguida, escolha um público-alvo ou crie um novo.

   Neste exemplo, queremos usar um público-alvo existente direcionado a clientes que pertencem aos níveis de pontos de fidelidade de prata e ouro.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Os públicos-alvo disponíveis na lista são originários da instância do Campaign V8 ou do Adobe Experience Platform, se a integração de Destino/Fontes tiver sido implementada em sua instância. Saiba como selecionar o público do email

1. Depois que o público-alvo for selecionado, você poderá editar as regras, se necessário. Você também pode definir um grupo de controle para analisar o comportamento dos destinatários de email em comparação ao comportamento dos perfis que não foram direcionados. Saiba como trabalhar com grupos de controle

## Programar o envio {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Programar o envio"
>abstract="TBC"

Para agendar o envio do email, clique em Habilitar e especifique a data e a hora desejadas.

= confirmar antes de enviar opção : o que acontece na data agendada: para confirmar o envio da mensagem?

![](assets/schedule.png)

## Visualizar e testar o email {#preview-test}

Quando o email estiver pronto, você poderá pré-visualizá-lo e testá-lo antes de iniciar seu envio.

1. Clique em **[!UICONTROL Revisar para enviar]**. É exibida uma visualização do email, juntamente com todas as propriedades, público-alvo e programação configurados. Você pode editar qualquer um desses elementos usando o botão modificar .

   ![](assets/review-email.png)

1. Clique no botão **[!UICONTROL Simular conteúdo]** para visualizar o email e enviar provas.

1. Na área do lado esquerdo, selecione os perfis a serem usados para visualizar o email. Você pode usar perfis direcionados ou perfis de teste dedicados.

1. Uma visualização do email é exibida na área direita com base no perfil selecionado. Se você tiver adicionado vários perfis, é possível alternar entre eles para visualizar o email correspondente.

   ![](assets/preview.png)

   >[!NOTE]
   >
   >Além disso, a variável **[!UICONTROL Renderizar email]** permite visualizar o email usando vários dispositivos ou provedores de email. Saiba como visualizar a renderização de email

1. Para enviar provas do seu email, clique no link **[!UICONTROL Teste]** em seguida, selecione os perfis que receberão a prova. Neste exemplo, queremos enviar as provas para um perfil de teste específico.

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >Você também pode testar suas mensagens representando alguns dos perfis segmentados e enviando a mensagem de prova para o endereço de email de sua escolha. Saiba como usar Substituir do modo de destino

1. Clique em **[!UICONTROL Enviar email de teste]** em seguida, confirme o envio.

   Depois que as provas forem enviadas, você poderá verificar seu status clicando no botão **[!UICONTROL Exibir log de email de teste]** botão.

## Enviar e monitorar o email {#prepare-send}

Depois de revisar e testar seu email, você pode iniciar a preparação e enviá-lo.

1. Clique em **[!UICONTROL Preparar]** para iniciar a preparação da mensagem.

   Você pode acompanhar o progresso da preparação em tempo real, juntamente com estatísticas. Quando a preparação estiver concluída, você poderá acessar logs detalhados para mais análise. Saiba como monitorar deliveries

   ![](assets/preparation.png)

1. Depois que o email estiver pronto para ser enviado, clique em **[!UICONTROL Enviar]** em seguida, confirme o envio.

   Você pode rastrear o envio em tempo real, juntamente com as estatísticas. Além disso, a variável **[!UICONTROL Logs]** permite acessar informações detalhadas sobre o envio do email. Saiba como monitorar deliveries

   ![](assets/logs.png)

1. Depois que o email tiver sido enviado, você poderá acessar relatórios dedicados para fins de análise adicional.

   ![](assets/reports.png)
