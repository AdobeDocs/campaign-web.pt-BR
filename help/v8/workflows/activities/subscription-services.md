---
audience: end-user
title: Usar a atividade Subscription services
description: Saiba como usar a atividade de workflow de serviços de assinatura
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 13%

---

# Serviços de assinatura {#subscriptipon-services}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Atividade de Serviços de assinatura"
>abstract="Use a nova atividade de fluxo de trabalho Serviços de assinatura para gerenciar assinaturas de um serviço. É possível assinar ou cancelar a assinatura de uma população, além de atualizar várias assinaturas de um arquivo externo. Como opção, também é possível enviar uma mensagem de confirmação para notificar seus assinantes."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"


>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Atividade de serviços de assinatura"
>abstract="A atividade Subscription services permite que vários perfis tenham uma subscrição ou sejam cancelados de um serviço em uma única ação."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Parâmetros gerais do serviço de assinatura"
>abstract="Escolha o serviço desejado e escolha a ação a ser executada (subscrição ou unsubscription). Ative a **Enviar mensagem de confirmação** opção ativada para notificar a população que a subscrição do serviço selecionado foi realizada ou cancelada."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Gerar uma transição de saída"
>abstract="Ative a opção **Gerar uma transição de saída** para adicionar uma transição após a atividade."

A variável **Serviços de assinatura** a atividade é um **Gerenciamento de dados** atividade. Ele permite criar ou excluir uma subscrição para um serviço de informações para a população especificada na transição.

## Configurar a atividade de serviços de assinatura {#subscription-services-configuration}

Siga estas etapas para configurar o **Serviços de assinatura** atividade:

1. Adicionar um **Serviços de assinatura** atividade no seu workflow. Você pode usar essa atividade após direcionar perfis ou importar um arquivo com dados identificados.

1. Selecione o serviço para o qual deseja gerenciar as assinaturas usando uma das seguintes opções:

   * **[!UICONTROL Selecionar um serviço específico]**: selecione manualmente um serviço usando o **[!UICONTROL Serviço]** campo.

   * **[!UICONTROL Da transição de entrada]**: use o serviço especificado na transição de entrada. Por exemplo, é possível importar um arquivo que especifica o serviço a ser gerenciado para cada linha. O serviço no qual executar a operação é então selecionado dinamicamente para cada perfil.

   ![](../assets/workflow-subscription-service.png)

1. Selecione a operação a ser executada: **Assinar** ou **Cancelar inscrição**.

   Se o serviço for definido na transição de entrada, você poderá escolher como recuperar essa operação:

   * **Selecionar um tipo de operação específico**: selecione manualmente a operação a ser executada (**Assinar** ou **Cancelar inscrição**)

   * **Selecione um tipo de operação em um caminho de transição de entrada**: selecione a coluna dos dados de entrada que especifica a operação a ser executada para cada registro. Por exemplo, você pode importar um arquivo que especifica a operação a ser executada para cada linha em uma coluna &quot;operação&quot;.

     >[!NOTE]
     >
     >Somente campos booleanos ou inteiros podem ser selecionados aqui. Verifique se os dados que contêm a operação a ser executada correspondem a esse formato. Por exemplo, se você estiver carregando dados de uma atividade Load file, verifique se definiu corretamente o formato da coluna que contém a operação na variável **[!UICONTROL Carregar arquivo]** atividade. Um exemplo é apresentado em [nesta seção](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Para notificar os destinatários que a subscrição do serviço selecionado foi realizada ou cancelada, alterne o **[!UICONTROL Enviar uma mensagem de confirmação]** opção ativada. O conteúdo dessa notificação é definido em um template do delivery associado ao serviço de informação.

1. Se estiver usando dados de uma transição de entrada, uma variável **[!UICONTROL Informações adicionais]** é exibida, permitindo especificar os dados e a origem da assinatura para cada registro. Você pode deixar essa seção vazia, nesse caso, nenhuma data ou origem será definida ao executar o workflow.

   * Se os dados de entrada tiverem uma coluna indicando a data de assinatura do perfil para o serviço, você poderá selecioná-la na **[!UICONTROL Data]** campo.

   * No **[!UICONTROL Caminho de origem]** defina a origem da assinatura. Você pode defini-la como um dos campos dos dados de entrada ou como um valor constante de sua escolha, marcando a opção **[!UICONTROL Definir uma constante como origem]** opção.

   ![](../assets/workflow-subscription-service-additional.png)

1. Para adicionar uma transição de saída após a atividade, alterne a variável **[!UICONTROL Gerar uma transição de saída]** opção ativada.

## Exemplos {#example}

### Subscrever um público-alvo a um serviço específico {#uc1}

Este fluxo de trabalho abaixo mostra como assinar um público-alvo para um serviço existente.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL Criar público-alvo]** A atividade segmenta um público-alvo existente.

* A **[!UICONTROL Serviços de assinatura]** A atividade permite selecionar o serviço para o qual os perfis devem ser inscritos.

### Atualização de vários status de subscrição diretamente de um arquivo {#uc2}

O fluxo de trabalho abaixo mostra como importar um arquivo contendo perfis e atualizar sua assinatura para vários serviços especificados no arquivo.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Carregar arquivo]** A atividade carrega um arquivo CSV contendo os dados e define a estrutura das colunas importadas. As colunas &quot;service&quot; e &quot;operation&quot; especificam o serviço a ser atualizado e a operação a ser executada (subscrição ou unsubscription).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Como você pode ter notado, a operação é especificada no arquivo como &quot;sub&quot; ou &quot;unsub&quot;. O sistema espera que um valor **Booliano** ou **Integer** reconheça a operação a ser executada: &quot;0&quot; para cancelar a assinatura e &quot;1&quot; para assinar. Para corresponder a esse requisito, um remapeamento de valores deve ser executado no detalhe da coluna &quot;operação&quot; na tela de configuração do arquivo de amostra.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Se o arquivo já usar &quot;0&quot; e &quot;1&quot; para identificar a operação, não é necessário remapear esses valores. Verifique apenas se a coluna é processada como um **Booleano** ou **Integer** nas colunas do arquivo de amostra.

* A **[!UICONTROL Reconciliação]** A atividade identifica os dados do arquivo como pertencente à dimensão do perfil do banco de dados do Adobe Campaign. A variável **email** O campo do arquivo corresponde ao campo **email** do recurso de perfil.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* Um **[!UICONTROL Enriquecimento]** A atividade cria um link para a tabela &quot;Serviços (nms)&quot; e um join simples entre a coluna &quot;serviço&quot; do arquivo carregado e o campo &quot;nome interno&quot; dos serviços no banco de dados.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Desduplicação]** com base no **email** o campo identifica duplicatas. É importante eliminar duplicatas, caso contrário, haverá falha para todos os dados na assinatura para um serviço.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)

* A **[!UICONTROL Serviços de assinatura]** identifica os serviços a serem atualizados como provenientes da transição, por meio do link criado no **[!UICONTROL Reconciliação]** atividade.

  A variável **[!UICONTROL Tipo de operação]** é identificado como proveniente da **operação** do arquivo. Somente os campos Booliano ou Integer podem ser selecionados aqui. Se a coluna do arquivo que contém a operação a ser executada não aparecer na lista, verifique se você definiu corretamente o formato da coluna no **[!UICONTROL Carregar arquivo]** atividade, conforme explicado anteriormente neste exemplo.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
