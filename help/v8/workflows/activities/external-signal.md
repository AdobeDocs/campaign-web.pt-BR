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

A variável **Sinal externo** a atividade é um **Controle de fluxo** atividade. Ela permite acionar a execução de um workflow a partir de outro workflow ou de uma chamada à API.

>[!NOTE]
>
>Esta página apresenta as principais etapas para configurar uma **[!UICONTROL Sinal externo]** atividade na interface da Web do Campaign e acioná-la a partir de outro workflow ou chamada de API. Informações detalhadas sobre como acionar um workflow e suas práticas recomendadas e como trabalhar com APIs do Campaign estão disponíveis na [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Siga estas etapas para configurar o **Sinal externo** atividade e acionar sua execução:

1. Adicionar um **Sinal externo** atividade no seu workflow.

1. Conclua a configuração do workflow e inicie sua execução. A variável **[!UICONTROL Sinal externo]** A atividade é exibida como &quot;Pendente&quot;, aguardando para ser acionada.

   ![](../assets/external-signal-pending.png)

1. Recupere as informações abaixo:

   * A variável **nome interno do fluxo de trabalho**, que é exibido ao lado do rótulo.

     +++Exibir exemplo

     ![](../assets/external-signal-workflow-name.png)

+++

   * A variável **Nome da atividade de sinal externo**, que é exibido no do workflow **[!UICONTROL Opções de execução]**.

     +++Exibir exemplo

     ![](../assets/external-signal-name.png)

+++

1. Para acionar o workflow, é necessário executar o `PostEvent` Função JavaScript. Essa função permite transmitir variáveis com os valores de sua escolha e aproveitá-los no fluxo de trabalho acionado.

   A variável `PostEvent` A função pode ser executada de outro workflow ou de uma chamada à API.

   * Para acionar um **[!UICONTROL Sinal externo]** atividade de um workflow, execute a função PostEvent a partir do **[!UICONTROL Script de inicialização]** painel, que pode ser acessado no painel **[!UICONTROL Opções de execução]**. Para o **[!UICONTROL Código JavaScript]** execute a função do script de atividade.

     A sintaxe é a seguinte:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Exibir exemplo

   Neste exemplo, acionamos a atividade de sinal externo &quot;signal1&quot; que foi adicionada ao workflow cujo nome interno é &quot;WKF12345&quot;. Também estamos transmitindo uma variável chamada &quot;customID&quot;, com o valor &quot;123456&quot;.

   ![](../assets/external-signal-sample.png)

+++

   * Para acionar um **[!UICONTROL Sinal externo]** atividade de uma chamada de API, siga as etapas detalhadas na Documentação da API do Campaign. [Saiba como usar o estático `PostEvent` método](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html?lang=pt-BR)
