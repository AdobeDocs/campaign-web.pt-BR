---
audience: end-user
title: Usar a atividade de sinal externo
description: Saiba como usar a atividade de workflow de sinal externo
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 11%

---

# Sinal externo {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Sinal externo"
>abstract="A atividade **Sinal externo** permite acionar a execução de um fluxo de trabalho a partir de outro fluxo de trabalho ou de uma chamada de API."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Parâmetros do sinal externo"
>abstract="Parâmetros do sinal externo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Acionadores de término"
>abstract="Acionadores de término"

A atividade **Sinal externo** é uma atividade **Controle de fluxo**. Ela permite acionar a execução de um workflow a partir de outro workflow ou de uma chamada à API.

>[!NOTE]
>
>Esta página apresenta as principais etapas para configurar uma atividade **[!UICONTROL Sinal externo]** na interface de usuário da Web do Campaign e acioná-la a partir de outro fluxo de trabalho ou de uma chamada de API. Informações detalhadas sobre como acionar um fluxo de trabalho e suas práticas recomendadas, e como trabalhar com APIs do Campaign estão disponíveis na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Siga estas etapas para configurar a atividade **Sinal externo** e acionar sua execução:

1. Adicione uma atividade **Sinal externo** ao seu fluxo de trabalho.

1. Conclua a configuração do workflow e inicie sua execução. A atividade **[!UICONTROL Sinal Externo]** é exibida como &quot;Pendente&quot;, aguardando para ser acionada.

   ![](../assets/external-signal-pending.png)

1. Recupere as informações abaixo:

   * O nome interno **do fluxo de trabalho**, que é exibido ao lado de seu rótulo.

     +++Exibir exemplo

     ![](../assets/external-signal-workflow-name.png)

+++

   * O **nome da atividade de sinal externo**, que é exibido nas **[!UICONTROL Opções de execução]** do fluxo de trabalho.

     +++Exibir exemplo

     ![](../assets/external-signal-name.png)

+++

1. Para acionar o fluxo de trabalho, é necessário executar a função JavaScript `PostEvent`. Essa função permite transmitir variáveis com os valores de sua escolha e aproveitá-los no fluxo de trabalho acionado.

   A função `PostEvent` pode ser executada de outro fluxo de trabalho ou de uma chamada de API.

   * Para acionar uma atividade **[!UICONTROL Sinal externo]** de um fluxo de trabalho, execute a função PostEvent a partir do painel **[!UICONTROL Script de inicialização]**, que pode ser acessado a partir das **[!UICONTROL Opções de execução]** da atividade. Para a atividade **[!UICONTROL JavaScript code]**, execute a função do script da atividade.

     A sintaxe é a seguinte:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Exibir exemplo

   Neste exemplo, acionamos a atividade de sinal externo &quot;signal1&quot; que foi adicionada ao workflow cujo nome interno é &quot;WKF12345&quot;. Também estamos transmitindo uma variável chamada &quot;customID&quot;, com o valor &quot;123456&quot;.

   ![](../assets/external-signal-sample.png)

+++

   * Para acionar uma atividade **[!UICONTROL Sinal externo]** a partir de uma chamada à API, siga as etapas detalhadas na documentação da API do Campaign. [Saiba como usar o método estático `PostEvent`](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=pt-BR)
