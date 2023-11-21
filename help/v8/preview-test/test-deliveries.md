---
audience: end-user
title: Enviar entregas de teste
description: Saiba como definir e enviar deliveries de teste
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Beta"
source-git-commit: 969401ab1258eb60697d16b3dc0470620abd346d
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 11%

---

# Enviar entregas de teste {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Modo de visualização"
>abstract="Visualize e teste a mensagem incluindo a população de teste ao público-alvo principal."

Depois que o conteúdo da mensagem for definido, você poderá pré-visualizá-lo e testá-lo enviando deliveries de teste para perfis de teste. Se você inseriu conteúdo personalizado, é possível verificar como esse conteúdo é exibido na mensagem, usando os dados do perfil de teste.

Para detectar possíveis erros nas configurações de conteúdo ou personalização da mensagem, envie mensagens de teste para perfis de teste antes de enviá-la para o público-alvo de destino. Uma mensagem de teste deve ser enviada sempre que uma alteração for feita, para validar o conteúdo mais recente. O envio de deliveries de teste (anteriormente conhecidos como &quot;provas&quot;) é uma etapa importante para validar sua campanha e identificar possíveis problemas. Os recipients de uma mensagem de teste podem verificar vários elementos, como links, links para opção de não participação, imagens ou mirror pages, bem como detectar erros na renderização, conteúdo, configurações de personalização e configuração do delivery.

## Simular conteúdo com destinatários de teste {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="População de teste"
>abstract="Selecione um modo de população de teste."

Antes de enviar um teste, defina um público-alvo de direcionamento para sua entrega. [Saiba mais](../audience/about-recipients.md)


Para começar a testar o conteúdo da mensagem:

1. Edite o conteúdo do seu delivery.
1. Clique em **[!UICONTROL Simular conteúdo]** botão.
1. Clique em **[!UICONTROL Teste]** botão para enviar mensagens de teste.

   ![](assets/simulate-test-button-email.png)

1. Selecione os recipients do teste.

   Dependendo do canal de mensagem, as mensagens de teste podem ser enviadas para os seguintes tipos de recipients:

   * Para SMS e emails, você pode usar [perfis de teste](#test-profiles), que são recipients adicionais específicos do banco de dados. Esses destinatários são criados na variável [!DNL Campaign] console do cliente. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   * Para SMS e emails, você também pode usar o [substituição do público alvo principal](#substitution-profiles) que envia as mensagens de teste para o endereço de teste de email ou número de telefone e usa dados de personalização de um perfil existente. Isso permite experimentar a mensagem da mesma maneira que os recipients, fornecendo uma representação precisa do conteúdo que o perfil receberá.

   * Para mensagens por push, é possível usar [assinantes](#subscribers), que são assinantes fictícios adicionados ao banco de dados. Eles são criados na [!DNL Campaign] console. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   A configuração detalhada para cada modo está disponível abaixo.

## Usar perfis de teste {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Público-alvo da prova"
>abstract="É possível fazer upload de um segundo arquivo como “público-alvo de prova” se desejar testar a entrega antes de enviar para o público-alvo principal."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Fazer upload de perfis"
>abstract="É possível fazer upload de um segundo arquivo com perfis adicionais se quiser testar a entrega com um conjunto diferente do conjunto usado como o público-alvo principal."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Arquivo de modelo"
>abstract="A formatação do arquivo precisa ser igual à do arquivo original.<br/>Formatos de arquivo compatíveis: txt, csv. Tamanho máximo do arquivo: 15 MB. Usar a primeira linha como cabeçalho da coluna."

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Incluir perfis de teste no público principal"
>abstract="Habilite esta opção para também enviar a mensagem final para os recipients do delivery de teste."

Os perfis de teste são seed addresses, que são recipients adicionais no banco de dados. Eles podem ser criados na variável [!DNL Adobe Campaign] console do cliente. As etapas para enviar mensagens de teste para seed addresses são detalhadas abaixo.

1. A partir do conteúdo do seu delivery, clique no link **[!UICONTROL Simular conteúdo]** e o botão **[!UICONTROL Teste]** botão.

1. No **[!UICONTROL Modo]** selecione **[!UICONTROL Perfis de teste]** para direcionar recipients fictícios que receberão o email de teste ou a delivery de SMS.

   ![](assets/simulate-profile-mode.png)

1. Se você já tiver selecionado perfis para [visualizar a mensagem](preview-content.md) na tela de simulação de conteúdo, esses perfis são pré-selecionados como recipients de teste. Você pode limpar sua seleção e/ou adicionar outros recipients usando o **[!UICONTROL Adicionar perfil(s) de teste]** botão.

   >[!NOTE]
   >
   >Os perfis de teste são criados no [!DNL Campaign] console do cliente na **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** pasta. Saiba como criar e gerenciar seed addresses no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.

1. Para enviar também a mensagem final aos recipients do delivery de teste, selecione o **[!UICONTROL Incluir população de teste no público alvo principal]** opção.

1. Depois que os perfis de teste forem selecionados, você poderá [enviar o delivery de teste](#send-test).

## Substituir dados do perfil {#substitution-profiles}

Use a substituição de perfil para enviar mensagens de teste para um endereço de email ou número de telefone específico, enquanto exibe dados de um perfil existente do [!DNL Adobe Campaign] banco de dados. Esse modo só poderá ser selecionado se o público-alvo da entrega tiver sido definido.

Para substituir os dados do perfil do target principal, siga as etapas abaixo:


1. A partir do conteúdo do seu delivery, clique no link **[!UICONTROL Simular conteúdo]** e o botão **[!UICONTROL Teste]** botão.

1. No **[!UICONTROL Modo]** selecione **[!UICONTROL Substituir do público alvo principal]** para enviar um teste para um endereço de email ou número de telefone específico ao exibir dados de um perfil existente.

   >[!CAUTION]
   >
   >Se você não selecionou um [público](../audience/about-recipients.md) para o seu delivery, a variável **[!UICONTROL Substituir do público alvo principal]** estará acinzentada e não será possível selecionar perfis de substituição.

1. Clique em **[!UICONTROL Adicionar endereço]** e especifique o endereço de email ou número de telefone que receberá o delivery de teste.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >Você pode inserir qualquer endereço de email ou número de telefone. Isso permite enviar deliveries de teste para qualquer recipient, mesmo que não sejam usuários do [!DNL Adobe Campaign].

1. Selecione o perfil do target definido para o delivery a ser usado como substituto. Você também pode permitir [!DNL Adobe Campaign] selecione um perfil aleatório no target. Os dados do perfil selecionado serão exibidos no delivery de teste.

1. Confirme o recipient e repita a operação para adicionar quantos endereços de email ou números de telefone forem necessários.

   ![](assets/simulate-profile-substitute.png)

1. Para enviar também a mensagem final aos recipients do delivery de teste, selecione o **[!UICONTROL Incluir população de teste no público alvo principal]** opção.

1. Depois que os perfis de substituição forem selecionados, você poderá [enviar o delivery de teste](#send-test).

## Enviar testes para assinantes de aplicativos {#subscribers}

Ao criar com notificações por push, os deliveries de teste só podem ser enviados aos assinantes do aplicativo. Para selecioná-los, siga as etapas abaixo.

1. No conteúdo do delivery de push, clique no link **[!UICONTROL Simular conteúdo]** e o botão **[!UICONTROL Teste]** botão.

   ![](assets/simulate-test-button-push.png)

1. Se você já tiver selecionado assinantes para [pré-visualizar o delivery](preview-content.md) na tela content simulation, esses perfis são pré-selecionados como assinantes de teste.

   Você pode limpar sua seleção e/ou adicionar mais assinantes usando o botão dedicado.

   ![](assets/simulate-test-subscribers.png)

1. Para enviar também a notificação por push final aos assinantes de teste, selecione o **[!UICONTROL Incluir população de teste no público alvo principal]** opção.

1. Depois que os assinantes forem selecionados, você poderá [enviar o delivery de teste](#send-test).

## Enviar o delivery de teste {#send-test}

Para enviar o delivery de teste para os recipients selecionados, siga as etapas abaixo.

1. Clique em **[!UICONTROL Enviar teste]** botão.

1. Confirme o envio.

   ![](assets/simulate-send-test.png)

1. Envie quantos testes forem necessários até concluir o conteúdo do delivery.

Depois de concluído, você pode preparar e enviar o delivery para o target principal. Saiba mais nas seções dedicadas abaixo:

* [Envie seu email](../monitor/prepare-send.md)
* [Enviar sua notificação por push](../push/send-push.md#send-push)
* [Enviar a entrega de SMS](../sms/send-sms.md#send-sms)

## Acesso a deliveries de teste enviados {#access-proofs}

Depois que os deliveries de teste forem enviados, você poderá acessar logs dedicados no **[!UICONTROL Exibir log de teste]** botão.

Esses logs permitem acessar todos os testes enviados para o delivery selecionado e visualizar estatísticas específicas relacionadas ao envio. [Saiba como monitorar os logs de entrega](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

Você também pode acessar testes enviados do [lista de entregas](../msg/gs-messages.md), como qualquer delivery.

![](assets/simulate-deliveries-list.png)
