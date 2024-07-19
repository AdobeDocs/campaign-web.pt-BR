---
audience: end-user
title: Usar a atividade Subscription services
description: Saiba como usar a atividade de workflow de serviços de assinatura
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 0e5b5e916309b2a337ac86f3741bcb83237b3fad
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 18%

---

# Serviços de assinatura {#subscription-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Atividade Serviços de assinatura"
>abstract="A atividade Serviços de assinatura permite que vários perfis sejam inscritos ou removidos de um serviço em uma única ação."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Parâmetros gerais do serviço de assinatura"
>abstract="Escolha o serviço desejado e escolha a ação a ser executada (assinatura ou cancelamento de assinatura). Ative a opção **Enviar mensagem de confirmação** para notificar a população sobre sua assinatura ou sobre o cancelamento da mesma no serviço selecionado."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Gerar uma transição de saída"
>abstract="Ative a opção **Gerar uma transição de saída** para adicionar uma transição após a atividade."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="Informações adicionais"
>abstract="Informações adicionais"

A atividade **Serviços de assinatura** é uma atividade de **Gerenciamento de Dados**. Ele permite criar ou excluir uma subscrição para um serviço de informações para a população especificada na transição.

## Configurar a atividade de serviços de assinatura {#subscription-services-configuration}

Siga estas etapas para configurar a atividade **Serviços de assinatura**:

1. Adicione uma atividade de **Serviços de assinatura** ao seu fluxo de trabalho. Você pode usar essa atividade após direcionar perfis ou importar um arquivo com dados identificados.

1. Selecione o serviço para o qual deseja gerenciar as assinaturas usando uma das seguintes opções:

   * **[!UICONTROL Selecione um serviço específico]**: selecione manualmente um serviço usando o campo **[!UICONTROL Serviço]**.

   * **[!UICONTROL Da transição de entrada]**: use o serviço especificado na transição de entrada. Por exemplo, é possível importar um arquivo que especifica o serviço a ser gerenciado para cada linha. O serviço no qual executar a operação é então selecionado dinamicamente para cada perfil.

   ![](../assets/workflow-subscription-service.png)

1. Selecione a operação a ser executada: **Assinar** ou **Cancelar assinatura**.

   Se o serviço for definido na transição de entrada, você poderá escolher como recuperar essa operação:

   * **Selecione um tipo de operação específico**: selecione manualmente a operação a ser executada (**Assinar** ou **Cancelar assinatura**)

   * **Selecione um tipo de operação em um caminho de transição de entrada**: selecione a coluna dos dados de entrada que especifica a operação a ser executada para cada registro. Por exemplo, você pode importar um arquivo que especifica a operação a ser executada para cada linha em uma coluna &quot;operação&quot;.

     Somente campos booleanos ou inteiros podem ser selecionados aqui. Verifique se os dados que contêm a operação a ser executada correspondem a esse formato. Por exemplo, se você estiver carregando dados de uma atividade Load file, verifique se definiu corretamente o formato da coluna que contém a operação na atividade **[!UICONTROL Load file]**. Um exemplo é apresentado em [esta seção](#uc2).

     >[!CAUTION]
     >
     >Por padrão, se você selecionar esta opção, a atividade **Serviços de assinatura** espera ter uma definição de link para a tabela **Serviços (nms)** configurada no fluxo de trabalho. Para fazer isso, verifique se você configurou um link de reconciliação em uma **atividade de Enriquecimento** para cima no fluxo de trabalho. Um exemplo de uso dessa opção está disponível [aqui](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Para notificar os destinatários que a assinatura do serviço selecionado foi realizada ou cancelada, ative a opção **[!UICONTROL Enviar mensagem de confirmação]**. O conteúdo dessa notificação é definido em um template do delivery associado ao serviço de informação.

1. Se você estiver usando dados de uma transição de entrada, uma seção de **[!UICONTROL Informações adicionais]** será exibida, permitindo especificar os dados e a origem da assinatura para cada registro. Você pode deixar essa seção vazia, nesse caso, nenhuma data ou origem será definida ao executar o workflow.

   * Se os dados de entrada tiverem uma coluna indicando a data de assinatura do perfil para o serviço, você poderá selecioná-la no campo **[!UICONTROL Data]**.

   * No campo **[!UICONTROL Caminho de origem]**, defina a origem da assinatura. Você pode defini-la como um dos campos dos dados de entrada ou como um valor constante de sua escolha marcando a opção **[!UICONTROL Definir uma constante como origem]**.

   ![](../assets/workflow-subscription-service-additional.png)

1. Para adicionar uma transição de saída após a atividade, alterne a opção **[!UICONTROL Generate an outbound transition]** para.

## Exemplos {#example}

### Subscrever um público-alvo a um serviço específico {#uc1}

Este fluxo de trabalho abaixo mostra como assinar um público-alvo para um serviço existente.

![](../assets/workflow-subscription-service-uc1.png)

* Uma atividade de **[!UICONTROL Build audience]** é direcionada a um público-alvo existente.

* Uma atividade de **[!UICONTROL Serviços de assinatura]** permite que você selecione o serviço para o qual os perfis devem ser assinados.

### Atualização de vários status de subscrição diretamente de um arquivo {#uc2}

O fluxo de trabalho abaixo mostra como importar um arquivo contendo perfis e atualizar sua assinatura para vários serviços especificados no arquivo.

![](../assets/workflow-subscription-service-uc2.png)

* Uma atividade **[!UICONTROL Load file]** carrega um arquivo CSV contendo os dados e define a estrutura das colunas importadas. As colunas &quot;service&quot; e &quot;operation&quot; especificam o serviço a ser atualizado e a operação a ser executada (subscrição ou unsubscription).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Como você pode ter notado, a operação é especificada no arquivo como &quot;sub&quot; ou &quot;unsub&quot;. O sistema espera que um valor **Booliano** ou **Integer** reconheça a operação a ser executada: &quot;0&quot; para cancelar a assinatura e &quot;1&quot; para assinar. Para atender a esse requisito:
   * O **Tipo de dados** da coluna &quot;operação&quot; está definido como inteiro.
   * Um **Remapeamento de valor** deve ser executado para corresponder aos valores &quot;sub&quot; e &quot;unsub&quot; com os valores &quot;1&quot; e &quot;0&quot;.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Se o arquivo já usar &quot;0&quot; e &quot;1&quot; para identificar a operação, não é necessário remapear esses valores. Verifique somente se a coluna é processada como um **Booleano** ou **Inteiro** nas colunas do arquivo de exemplo.

* Uma atividade **[!UICONTROL Reconciliation]** identifica os dados do arquivo como pertencente à dimensão do perfil do banco de dados do Adobe Campaign. O campo **email** do arquivo corresponde ao campo **email** do recurso de perfil.

  ![](../assets/workflow-subscription-service-uc2-reconciliation.png)

* Uma atividade **[!UICONTROL Enrichment]** cria um link de reconciliação para a tabela &quot;Services (nms)&quot;, com uma simples associação entre a coluna &quot;service&quot; do arquivo carregado e o campo &quot;internal name&quot; de serviços no banco de dados.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* Os **[!UICONTROL Serviços de Assinatura]** identificam os serviços a serem atualizados como provenientes da transição.

  O **[!UICONTROL Tipo de operação]** é identificado como proveniente do campo **operação** do arquivo. Somente os campos Booliano ou Integer podem ser selecionados aqui. Se a coluna do arquivo que contém a operação a ser executada não aparecer na lista, verifique se você definiu corretamente o formato da coluna na atividade **[!UICONTROL Carregar arquivo]**, conforme explicado anteriormente neste exemplo.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
