---
audience: end-user
title: Pré-visualizar e enviar um delivery de correspondência direta
description: Saiba como visualizar e enviar um delivery de correspondência direta com o Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 3%

---


# Pré-visualizar e enviar um delivery de correspondência direta {#send-direct-mail}

Depois de configurar o arquivo de extração para o delivery de correspondência direta, você pode utilizar perfis de teste para visualizá-lo. Se você incluiu conteúdo personalizado, poderá examinar como esse conteúdo é exibido nas colunas usando os dados do perfil de teste. Isso permite garantir que o conteúdo do arquivo seja renderizado corretamente e que os elementos personalizados sejam incorporados adequadamente.

Quando o arquivo de extração estiver pronto, você poderá enviar o delivery de correspondência direta para gerar o arquivo e compartilhá-lo com seu provedor de correspondência direta. [Saiba como enviar o delivery de correspondência direta](#dm-send)

## Visualizar o arquivo de extração {#preview-dm}

As principais etapas para visualizar seu arquivo de extração são as seguintes. Mais detalhes sobre como visualizar deliveries estão disponíveis em [nesta seção](../preview-test/preview-content.md).

1. Na página de conteúdo do delivery, use **[!UICONTROL Simular conteúdo]** para visualizar seu conteúdo personalizado.

   ![](assets/dm-simulate.png){zoomable=&quot;yes&quot;}

1. Clique em **[!UICONTROL Adicionar perfil(s) de teste]** para selecionar um ou vários perfis para visualizar seus dados no conteúdo do arquivo de extração.

1. No painel direito, você encontrará uma pré-visualização do arquivo de extração, em que os elementos personalizados são substituídos dinamicamente pelos dados do perfil selecionado.

   ![](assets/dm-preview-right.png){zoomable=&quot;yes&quot;}

## Enviar provas {#test-dm}

Usar **Adobe Campaign**, você pode enviar provas antes de enviá-las para o público-alvo principal. Essa etapa é importante para validar o delivery e identificar quaisquer problemas. Os recipients de teste podem revisar elementos, como configurações de personalização, garantindo o desempenho ideal e detectando erros. Esse processo ajuda a refinar e otimizar o arquivo de extração antes de atingir o público-alvo principal.

Para deliveries de correspondência direta, o envio de provas gera uma amostra do arquivo de extração usando dados dos perfis de teste selecionados. Para acessá-lo, siga estas etapas:

1. Na tela de simulação de conteúdo, clique no link **[!UICONTROL Enviar prova]** e siga as mesmas etapas de qualquer tipo de delivery para enviar uma prova. [Saiba como enviar provas](../preview-test/test-deliveries.md)

1. Depois que a prova for enviada, você poderá acessá-la no **[!UICONTROL Exibir provas]** ou na lista de deliveries. [Saiba como acessar provas enviadas](../preview-test/test-deliveries.md#access-test-deliveries)

1. No painel de delivery de prova, clique no link **[!UICONTROL Visualizar arquivo]** botão para acessar uma pré-visualização do arquivo de extração.

   ![](assets/dm-proof.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Somente as primeiras 100 linhas são exibidas no arquivo de visualização.

## Enviar o delivery de correspondência direta {#send-dm}

Quando a correspondência direta estiver pronta para ser enviada aos clientes, você poderá enviar o delivery para iniciar a extração de dados no arquivo de extração especificado. Para fazer isso, siga estes passos:

1. Depois de criar o conteúdo do arquivo de extração, clique em **[!UICONTROL Revisar e enviar]** do seu **[!UICONTROL Entrega]** página.

   ![](assets/dm-review-send.png){zoomable=&quot;yes&quot;}

1. Clique em **[!UICONTROL Preparar]** acompanhamento dos progressos e das estatísticas fornecidos.

   Se ocorrerem erros, consulte a **[!UICONTROL Logs]** para obter informações detalhadas sobre a falha.

   ![](assets/dm-prepare.png){zoomable=&quot;yes&quot;}

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para continuar com o processo final de envio.

1. Confirme a ação de envio clicando no ícone **[!UICONTROL Enviar]**.

   Se o delivery de mala direta tiver sido agendado, clique no link **[!UICONTROL Enviar conforme agendado]** botão. Saiba mais sobre a programação de delivery em [nesta seção](../msg/gs-messages.md#schedule-the-delivery-sending).

Depois que o delivery é enviado, o arquivo de extração é gerado e exportado automaticamente para o local especificado na **[!UICONTROL Roteamento]** conta externa selecionada no modelo de entrega [configurações avançadas](../advanced-settings/delivery-settings.md).

Você pode rastrear seus KPIs (indicadores principais de desempenho) por meio da página de entrega e dados do **[!UICONTROL Logs]** menu.

Você também pode começar a medir o impacto da sua mensagem com relatórios integrados. [Saiba mais](../reporting/direct-mail.md)