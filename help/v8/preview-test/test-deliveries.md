---
audience: end-user
title: Enviar provas
description: Saiba como definir e enviar provas
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 14%

---

# Enviar provas {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Modo de visualização"
>abstract="Visualize e teste a mensagem incluindo a população de teste ao público-alvo principal."

Depois que o conteúdo da mensagem for definido, é possível pré-visualizá-lo e testá-lo enviando provas para perfis de teste. Se você inseriu conteúdo personalizado, é possível verificar como esse conteúdo é exibido na mensagem, usando os dados do perfil de teste.

Para detectar possíveis erros nas configurações de conteúdo ou personalização da mensagem, envie provas para perfis de teste antes de enviá-la para o público-alvo. Uma prova deve ser enviada sempre que uma alteração for feita, para validar o conteúdo mais recente. O envio de provas é uma etapa importante na validação da campanha e na identificação de possíveis problemas. Os recipients de prova podem verificar vários elementos, como links, links para opção de não participação, imagens ou mirror pages, bem como detectar erros na renderização, conteúdo, configurações de personalização e configuração do delivery.

## Simular conteúdo com destinatários de teste {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="População de teste"
>abstract="Selecione um modo de população de teste."

Antes de enviar uma prova, defina um público-alvo para sua entrega. [Saiba mais](../audience/add-audience.md)

Para começar a testar o conteúdo da mensagem:

1. Edite o conteúdo do seu delivery.
1. Clique em **[!UICONTROL Simular conteúdo]** botão.
1. Clique em **[!UICONTROL Enviar prova]** botão para enviar provas.

   ![](assets/simulate-test-button-email.png){zoomable=&quot;yes&quot;}

1. Selecione os recipients da prova.

   Dependendo do canal de mensagem, as provas podem ser enviadas para os seguintes tipos de recipients:

   * Para SMS e emails, você pode usar [perfis de teste](#test-profiles), que são recipients adicionais específicos do banco de dados. Você também pode usar a variável [substituição do público alvo principal](#substitution-profiles) que envia a prova para um endereço de teste de email ou número de telefone e usa dados de personalização de um perfil existente. Isso permite experimentar a mensagem da mesma maneira que os recipients, fornecendo uma representação precisa do conteúdo que o perfil receberá.

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
>title="Incluir perfis de teste no público-alvo principal"
>abstract="Habilite essa opção para também enviar a mensagem final para os recipients da prova."

Os perfis de teste são recipients adicionais no banco de dados. Eles são criados a partir da variável **[!UICONTROL Gerenciamento de clientes]** > **[!UICONTROL Perfis]** menu. [Saiba mais](../audience/test-profiles.md#create-test-profiles)

As etapas para enviar provas para perfis de teste são detalhadas abaixo.

1. A partir do conteúdo do seu delivery, clique no link **[!UICONTROL Simular conteúdo]** e o botão **[!UICONTROL Enviar prova]** botão.

1. No **[!UICONTROL Modo]** selecione **[!UICONTROL Perfis de teste]** para direcionar recipients fictícios que receberão a prova ou o delivery de SMS.

   ![](assets/simulate-profile-mode.png){zoomable=&quot;yes&quot;}

1. Se você já tiver selecionado perfis para [visualizar a mensagem](preview-content.md) na tela de simulação de conteúdo, esses perfis são pré-selecionados como recipients de provas. Você pode limpar sua seleção e/ou adicionar outros recipients usando o **[!UICONTROL Adicionar perfil(s) de teste]** botão.

1. Ao navegar pelo perfil de teste ou pelas listas de perfis, você pode usar filtros para refinar a pesquisa. Por exemplo, é possível definir uma regra para localizar todos os perfis de teste com **[!UICONTROL Cliente Potencial]** status. Saiba como adicionar regras usando o [modelador de consultas](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Para enviar a mensagem final também aos recipients da prova, selecione o **[!UICONTROL Incluir população de teste no público alvo principal]** opção.

   ![](assets/simulate-include-test.png){zoomable=&quot;yes&quot;}

1. Depois que os perfis de teste forem selecionados, você poderá [enviar a prova](#send-test).

## Substituir dados do perfil {#substitution-profiles}

Use a substituição de perfil para enviar provas para um endereço de email ou número de telefone específico, enquanto exibe dados de um perfil existente do [!DNL Adobe Campaign] banco de dados. Esse modo só poderá ser selecionado se o público-alvo da entrega tiver sido definido.

Para substituir os dados do perfil do target principal, siga as etapas abaixo:

1. A partir do conteúdo do seu delivery, clique no link **[!UICONTROL Simular conteúdo]** e o botão **[!UICONTROL Enviar prova]** botão.

1. No **[!UICONTROL Modo]** selecione **[!UICONTROL Substituir do público alvo principal]** para enviar uma prova para um endereço de email ou número de telefone específico ao exibir dados de um perfil existente.

   >[!CAUTION]
   >
   >Se você não selecionou um [público](../audience/about-recipients.md) para o seu delivery, a variável **[!UICONTROL Substituir do público alvo principal]** estará acinzentada e não será possível selecionar perfis de substituição.

1. Clique em **[!UICONTROL Adicionar endereço]** e especifique o endereço de email ou número de telefone que receberá a prova.

   ![](assets/simulate-add-substitution-address.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Você pode inserir qualquer endereço de email ou número de telefone. Isso permite enviar provas para qualquer recipient, mesmo que ele não seja usuário do [!DNL Adobe Campaign].

1. Selecione o perfil do target definido para o delivery a ser usado como substituto. Você também pode permitir [!DNL Adobe Campaign] selecione um perfil aleatório no target. Os dados de perfil do perfil selecionado serão exibidos na prova.

1. Confirme o recipient e repita a operação para adicionar quantos endereços de email ou números de telefone forem necessários.

   ![](assets/simulate-profile-substitute.png){zoomable=&quot;yes&quot;}

1. Para enviar a mensagem final também aos recipients da prova, selecione o **[!UICONTROL Incluir população de teste no público alvo principal]** opção.

1. Depois que os perfis de substituição forem selecionados, você poderá [enviar a prova](#send-test).

## Enviar provas para assinantes de aplicativos {#subscribers}

Ao criar com notificações por push, as provas só podem ser enviadas aos assinantes do aplicativo. Para selecioná-los, siga as etapas abaixo.

1. No conteúdo do delivery de push, clique no link **[!UICONTROL Simular conteúdo]** e o botão **[!UICONTROL Enviar prova]** botão.

   ![](assets/simulate-test-button-push.png){zoomable=&quot;yes&quot;}

1. Se você já tiver selecionado assinantes para [pré-visualizar o delivery](preview-content.md) na tela content simulation, esses perfis são pré-selecionados como assinantes de teste.

   Você pode limpar sua seleção e/ou adicionar mais assinantes usando o botão dedicado.

   ![](assets/simulate-test-subscribers.png){zoomable=&quot;yes&quot;}

1. Para enviar também a notificação por push final aos assinantes de teste, selecione o **[!UICONTROL Incluir população de teste no público alvo principal]** opção.

1. Depois que os assinantes forem selecionados, você poderá [enviar a prova](#send-test).

## Enviar a prova {#send-test}

Para enviar a prova aos recipients selecionados, siga as etapas abaixo.

1. Clique em **[!UICONTROL Enviar prova]** botão.

1. Confirme o envio.

   ![](assets/simulate-send-test.png){zoomable=&quot;yes&quot;}

1. Envie quantas provas forem necessárias até concluir o conteúdo do delivery.

Depois de concluído, você pode preparar e enviar o delivery para o target principal. Saiba mais nas seções dedicadas abaixo:

* [Envie seu email](../monitor/prepare-send.md)
* [Enviar sua notificação por push](../push/send-push.md#send-push)
* [Enviar a entrega de SMS](../sms/send-sms.md#send-sms)

## Acesso a provas enviadas {#access-test-deliveries}

Depois que as provas forem enviadas, você poderá acessar os logs em **[!UICONTROL Simular conteúdo]** tela.

Esses logs permitem acessar todas as provas enviadas para o delivery selecionado e visualizar estatísticas específicas relacionadas ao envio. [Saiba como monitorar os logs de entrega](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable=&quot;yes&quot;}

Você também pode acessar provas enviadas pelo [lista de entrega](../msg/gs-messages.md), como qualquer delivery.

![](assets/simulate-deliveries-list.png){zoomable=&quot;yes&quot;}
