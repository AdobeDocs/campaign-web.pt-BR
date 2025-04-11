---
audience: end-user
title: Pré-visualizar e enviar um delivery de correspondência direta
description: Saiba como visualizar e enviar um delivery de correspondência direta com o Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 1%

---

# Pré-visualizar e enviar um delivery de correspondência direta {#send-direct-mail}

Depois de configurar o arquivo de extração para o delivery de correspondência direta, use perfis de teste para pré-visualizá-lo. Se houver conteúdo personalizado incluído, examine como esse conteúdo aparece nas colunas usando os dados do perfil de teste. Isso garante que o conteúdo do arquivo seja renderizado corretamente e que os elementos personalizados sejam incorporados adequadamente.

Quando o arquivo de extração estiver pronto, envie o delivery de correspondência direta para gerar o arquivo e compartilhe-o com seu provedor de correspondência direta. [Saiba como enviar sua entrega de correspondência direta](#dm-send)

## Visualizar o arquivo de extração {#preview-dm}

As principais etapas para visualizar seu arquivo de extração são as seguintes. Mais detalhes sobre como visualizar entregas estão disponíveis em [esta seção](../preview-test/preview-content.md).

1. Na sua página de conteúdo de entrega, use **[!UICONTROL Simular conteúdo]** para pré-visualizar seu conteúdo personalizado.

   ![Captura de tela mostrando a opção de simulação de conteúdo na página de conteúdo da entrega](assets/dm-simulate.png){zoomable="yes"}

1. Clique em **[!UICONTROL Adicionar perfil(s) de teste]** para selecionar um ou vários perfis e visualizar seus dados no conteúdo do arquivo de extração.

1. No painel direito, visualize o arquivo de extração, em que os elementos personalizados são substituídos dinamicamente por dados do perfil selecionado.

   ![Captura de tela mostrando a visualização do arquivo de extração no painel direito](assets/dm-preview-right.png){zoomable="yes"}

## Enviar provas {#test-dm}

Usando o **Adobe Campaign**, envie provas antes de entregá-las ao seu público principal. Esta etapa valida o delivery e identifica quaisquer problemas. Os recipients de teste revisam elementos, como configurações de personalização, garantindo o desempenho ideal e detectando erros. Esse processo refina e otimiza o arquivo de extração antes de atingir o público-alvo principal.

Para deliveries de correspondência direta, o envio de provas gera uma amostra do arquivo de extração usando dados dos perfis de teste selecionados. Para acessá-lo, siga estas etapas:

1. Na tela de simulação de conteúdo, clique no botão **[!UICONTROL Enviar prova]** e siga as mesmas etapas de qualquer tipo de entrega para enviar uma prova. [Saiba como enviar provas](../preview-test/test-deliveries.md)

1. Depois que a prova for enviada, acesse-a pelo botão **[!UICONTROL Exibir provas]** ou pela lista de entregas. [Saiba como acessar provas enviadas](../preview-test/test-deliveries.md#access-test-deliveries)

1. No painel de entrega de prova, clique no botão **[!UICONTROL Visualizar arquivo]** para acessar uma visualização do arquivo de extração.

   ![Captura de tela mostrando a opção de arquivo de visualização no painel de entrega de prova](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >Somente as primeiras 100 linhas são exibidas no arquivo de visualização.

## Enviar o delivery de correspondência direta {#send-dm}

Quando a correspondência direta estiver pronta para ser enviada aos clientes, envie o delivery para iniciar a extração de dados no arquivo de extração especificado. Para fazer isso, siga estes passos:

1. Após criar o conteúdo do arquivo de extração, clique em **[!UICONTROL Revisar e enviar]** da sua página **[!UICONTROL Entrega]**.

   ![Captura de tela mostrando a opção de revisão e envio na página de entrega](assets/dm-review-send.png){zoomable="yes"}

1. Clique em **[!UICONTROL Preparar]** e monitore o progresso e as estatísticas fornecidas.

   Se ocorrerem erros, consulte o menu **[!UICONTROL Logs]** para obter informações detalhadas sobre a falha.

   ![Captura de tela mostrando a opção de preparação e o menu de logs](assets/dm-prepare.png){zoomable="yes"}

1. Envie as mensagens clicando em **[!UICONTROL Enviar]** para prosseguir com o processo de envio final.

1. Confirme a ação de envio clicando em **[!UICONTROL Enviar]**.

   Se a entrega da correspondência direta estiver agendada, clique no botão **[!UICONTROL Enviar como agendado]**. Saiba mais sobre o agendamento de entrega em [esta seção](../msg/gs-messages.md#schedule-the-delivery-sending).

Depois que a entrega é enviada, o arquivo de extração é gerado automaticamente e exportado para o local especificado na conta externa **[!UICONTROL Roteamento]** selecionada nas [configurações avançadas](../advanced-settings/delivery-settings.md) do modelo de entrega.

Acompanhe seus KPIs (indicadores principais de desempenho) na página de entrega e os dados do menu **[!UICONTROL Logs]**.

Comece a medir o impacto da sua mensagem com relatórios integrados. [Saiba mais](../reporting/direct-mail.md)