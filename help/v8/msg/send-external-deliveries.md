---
audience: end-user
title: Introdução a entregas externas
description: Saiba como criar e enviar deliveries externos com o Adobe Campaign Web
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 7%

---

# Enviar deliveries externos {#gs-direct-mail}

O Adobe Campaign permite manipular deliveries criados fora do Campaign para fazer deliveries em massa de emails personalizados, mensagens SMS ou notificações por push (iOs e Android) por meio de um sistema externo.

<!--The supported channels are Email, Mobile (SMS), and Push (iOs and Android).-->

Ao criar um delivery externo, o Adobe Campaign gera automaticamente um arquivo de extração contendo todos os perfis direcionados e dados selecionados. Esse arquivo é enviado ao servidor de sua escolha, que lidará com o processo de envio para você.

## Criar uma conta externa dedicada {#routing-external-account}

Primeiro, é necessário configurar uma conta externa específica que será usada nos deliveries externos. Deve ser do tipo **[!UICONTROL Roteamento]**.

>[!NOTE]
>
>Saiba como criar uma conta externa do tipo roteamento em [esta seção](../administration/external-account.md#routing).

Por exemplo, selecione o canal **[!UICONTROL Mobile (SMS)]** para a conta externa. **[!UICONTROL Externo]** é selecionado por padrão como o **[!UICONTROL Modo de entrega]**.

![](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## Criar e enviar o delivery externo {#create-external-delivery}

Depois que a conta externa específica for configurada, crie o delivery externo. Siga as etapas abaixo.

1. Criar um delivery. [Saiba como](create-deliveries.md)

   Há três opções:

   * **Em um fluxo de trabalho**: adicione uma atividade de canal externo (email, SMS ou push) ao seu fluxo de trabalho. Para obter instruções detalhadas sobre como configurar o fluxo de trabalho, consulte [esta página](../workflows/gs-workflow-creation.md).
   * **Em uma campanha**: depois de criar uma campanha, você pode criar uma entrega externa de email, SMS ou canal de push. Para obter mais informações sobre como configurar sua campanha, consulte [esta página](../campaigns/gs-campaigns.md).
   * **Entrega independente**: envolva os clientes direta e instantaneamente com uma entrega externa individual. [Saiba como criar uma entrega](../msg/gs-deliveries.md)

1. Nas [configurações](../advanced-settings/delivery-settings.md) do modelo de entrega ou de entrega, selecione a conta externa que você criou para o canal de sua escolha (neste exemplo, o canal SMS) e salve.

   ![](assets/external-delivery-routing.png){zoomable="yes"}

   >[!NOTE]
   >
   >Se você estiver criando uma entrega, verifique se selecionou um [modelo de entrega](delivery-template.md) usando uma conta externa do tipo **[!UICONTROL Roteamento]**; caso contrário, não será possível selecionar a conta dedicada criada [acima](#routing-external-account).

1. Na seção de entrega de **[!UICONTROL Conteúdo]**, clique em **[!UICONTROL Editar conteúdo]**.

   ![](assets/external-delivery-edit-content.png){zoomable="yes"}

1. Ao contrário de um delivery padrão, você não está projetando o conteúdo da mensagem em si. Em vez disso, você precisa definir as propriedades e colunas do arquivo que será enviado para o sistema externo.

   ![](assets/external-delivery-file-properties.png){zoomable="yes"}

   Siga as mesmas etapas de criação do conteúdo do arquivo de extração gerado por [entregas de correspondência direta](../direct-mail/content-direct-mail.md):

   * Defina as propriedades do arquivo de extração. [Saiba mais](../direct-mail/content-direct-mail.md#properties)
   * Selecione as colunas que contêm as informações a serem exportadas para esse arquivo. [Saiba mais](../direct-mail/content-direct-mail.md#content)

1. Você pode visualizar o arquivo e enviar provas<!--not in UI right now - to check-->. [Saiba como](../direct-mail/send-direct-mail.md#preview-dm)

   ![](assets/external-delivery-simulate.png){zoomable="yes"}

1. Envie o delivery para gerar o arquivo de extração. [Saiba como](../direct-mail/send-direct-mail.md#send-dm)

Depois que a entrega é enviada, o arquivo de extração é gerado automaticamente e exportado para o local especificado na [conta externa](../administration/external-account.md#create-ext-account) selecionada nas configurações do modelo de entrega.

É possível rastrear os KPIs na página de entrega e os dados no menu **[!UICONTROL Logs]**.