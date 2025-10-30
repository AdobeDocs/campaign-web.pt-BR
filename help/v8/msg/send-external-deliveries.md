---
audience: end-user
title: Introdução a entregas externas
description: Saiba como criar e enviar deliveries externos com o Adobe Campaign Web
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 8%

---

# Enviar entregas externas {#gs-direct-mail}

O Adobe Campaign permite gerenciar deliveries criados fora do Campaign para delivery em massa de emails personalizados, mensagens SMS ou notificações por push (iOS e Android) por meio de um sistema externo.

<!--The supported channels are Email, Mobile (SMS), and Push (iOS and Android).-->

Ao criar um delivery externo, o Adobe Campaign gera automaticamente um arquivo de extração contendo todos os perfis direcionados e dados selecionados. Esse arquivo é enviado para o servidor de sua escolha, que lida com o processo de envio.

## Criar uma conta externa dedicada {#routing-external-account}

Você precisa configurar uma conta externa específica para usar em seus deliveries externos. Deve ser do tipo **[!UICONTROL Roteamento]**.

>[!NOTE]
>
>Saiba como criar uma conta externa do tipo roteamento em [esta seção](../administration/external-account.md#routing).

Por exemplo, selecione o canal **[!UICONTROL Mobile (SMS)]** para a conta externa. **[!UICONTROL Externo]** é selecionado por padrão como o **[!UICONTROL Modo de entrega]**.

![Configuração do modo de entrega da conta externa](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## Criar e enviar o delivery externo {#create-external-delivery}

Depois que a conta externa específica for configurada, crie o delivery externo. Siga as etapas abaixo.

1. Criar um delivery. [Saiba como](create-deliveries.md)

   Há três opções:

   * **Em um fluxo de trabalho**: adicione uma atividade de canal externo (email, SMS ou push) ao seu fluxo de trabalho. Para obter instruções detalhadas sobre como configurar fluxos de trabalho, consulte [esta página](../workflows/gs-workflow-creation.md).
   * **Em uma campanha**: depois de criar uma campanha, você pode criar uma entrega externa de email, SMS ou canal de push. Para obter mais informações sobre como configurar sua campanha, consulte [esta página](../campaigns/gs-campaigns.md).
   * **Entrega independente**: envolva os clientes direta e instantaneamente com uma entrega externa individual. [Saiba como criar uma entrega](../msg/gs-deliveries.md)

1. Nas [configurações](../advanced-settings/delivery-settings.md) do modelo de entrega ou entrega, selecione a conta externa criada para o canal de sua escolha (neste exemplo, o canal SMS) e salve.

   ![Configuração de roteamento de entrega externa](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se você estiver criando uma entrega, verifique se selecionou um [modelo de entrega](delivery-template.md) usando uma conta externa do tipo **[!UICONTROL Roteamento]**. Caso contrário, você não poderá selecionar a conta dedicada criada [acima](#routing-external-account).

1. Na seção de entrega de **[!UICONTROL Conteúdo]**, clique em **[!UICONTROL Editar conteúdo]**.

   ![Editar conteúdo na entrega externa](assets/external-delivery-edit-content.png){zoomable="yes"}

1. Diferentemente de um delivery padrão, você não projeta o conteúdo da mensagem propriamente dita. Em vez disso, defina as propriedades e as colunas do arquivo que será enviado para o sistema externo.

   ![Configuração de propriedades de arquivo para entrega externa](assets/external-delivery-file-properties.png){zoomable="yes"}

   Siga as mesmas etapas de criação do conteúdo do arquivo de extração gerado por [entregas de correspondência direta](../direct-mail/content-direct-mail.md):

   * Defina as propriedades do arquivo de extração. [Saiba mais](../direct-mail/content-direct-mail.md#properties)
   * Selecione as colunas que contêm as informações a serem exportadas para o arquivo. [Saiba mais](../direct-mail/content-direct-mail.md#content)

1. Visualize o arquivo e envie provas<!--not in UI right now - to check-->. [Saiba como](../direct-mail/send-direct-mail.md#preview-dm)

   ![Simular entrega externa](assets/external-delivery-simulate.png){zoomable="yes"}

1. Envie o delivery para gerar o arquivo de extração. [Saiba como](../direct-mail/send-direct-mail.md#send-dm)

Depois que a entrega é enviada, o arquivo de extração é gerado automaticamente e exportado para o local especificado na [conta externa](../administration/external-account.md#create-ext-account) selecionada nas configurações do modelo de entrega.

Acompanhe os KPIs na página de entrega e os dados do menu **[!UICONTROL Logs]**.