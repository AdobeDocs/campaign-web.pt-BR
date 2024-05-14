---
audience: end-user
title: Usar a atividade de workflow de código JavaScript
description: Saiba como usar a atividade de workflow de código JavaScript
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 30%

---

# Código JavaScript {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="Código JavaScript"
>abstract="A atividade **Código JavaScript** permite executar um código JavaScript no contexto de um fluxo de trabalho. Ela permite executar ações ou coletar informações do banco de dados. Use atividades de código JavaScript **simples** para executar um trecho de código na execução do fluxo de trabalho. As atividades de código JavaScript **Avançadas** permitem executar operações mais complexas, executando dois trechos de código diferentes em ordem sequencial. Na primeira vez que o fluxo de trabalho é iniciado, a primeira chamada é executada. Cada vez que o fluxo de trabalho é executado novamente, o código definido na segunda chamada é executado."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="Trecho de JavaScript"
>abstract="Defina o script a ser executado durante a execução da atividade. Se estiver configurando uma atividade JavaScript **Avançada**, será necessário editar dois trechos de código: o primeiro código de chamada a ser executado na primeira execução do fluxo de trabalho e o próximo código de chamada a ser executado nas demais chamadas do fluxo de trabalho."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="Execução de JavaScript"
>abstract="Configure o atraso de execução para interromper a atividade após um período de execução. Por padrão, a fase de execução não pode exceder 1 hora. Após esse atraso, o processo será interrompido com uma mensagem de erro e a execução da atividade falhará. Para ignorar esse limite, defina o valor como 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Transição de JavaScript"
>abstract="Se quiser adicionar várias transições de saída, clique no botão **[!UICONTROL Adicionar transições]**. Isso permite, por exemplo, acionar uma transição específica com base em uma condição específica definida na atividade Código JavaScript. Essa opção está disponível somente para atividades de código JavaScript **Avançadas**."

A variável **Código JavaScript** a atividade é um **Gestão de dados** atividade. Use esta atividade para executar um script JavaScript no contexto de um workflow. Isso permite coletar informações do banco de dados ou executar outras operações complexas.

## Configurar a atividade do código JavaScript {#javascript-code-configuration}

Siga estas etapas para configurar o **Código JavaScript** atividade:

1. Adicionar um **Código JavaScript** atividade no seu workflow.

1. Escolha o tipo de atividade que deseja criar:

   * **Simples**: Execute um trecho de código.
   * **Avançado**: essa opção permite executar operações mais avançadas executando dois snippets de código diferentes. [Saiba como configurar uma atividade avançada do JavaScript](#advanced)

   >[!NOTE]
   >
   >Com a interface do usuário da Web do Campaign, consolidamos duas atividades em uma unindo ambas **Simples** e **Avançado** Funcionalidades de código JavaScript. Essa consolidação não afeta a funcionalidade da atividade de forma alguma.

1. Confirme e clique no botão **[!UICONTROL Editar código]** botão para abrir o editor de expressão. O painel do lado esquerdo fornece sintaxes predefinidas que você pode aproveitar para criar seu código, incluindo variáveis de evento. [Saiba como trabalhar com variáveis de evento e o editor de expressão](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. No **[!UICONTROL Execução]** , configure o atraso para interromper a atividade após um período de execução. Por padrão, a fase de execução não pode exceder 1 hora. Após esse atraso, o processo será interrompido com uma mensagem de erro e a execução da atividade falhará. Para ignorar esse limite, defina o valor como 0.

   ![](../assets/javascript-config.png)

1. Ative a **[!UICONTROL Processar erros]** opção para manter os erros que ocorrem durante a execução do script em uma transição de saída adicional.

## Atividades avançadas de código JavaScript {#advanced}

As atividades avançadas do JavaScript permitem executar operações complexas. Ele permite:

* Execute dois trechos de código diferentes. O primeiro trecho de código é executado na primeira vez que o workflow é iniciado. Cada vez que o workflow é executado novamente, o trecho de código definido na segunda chamada é executado.
* Adicione várias transições de saída com as quais você pode interagir dinamicamente usando um script.

Para configurar uma atividade de código JavaScript avançada, siga estas etapas:

1. Selecione o **Avançado** digite e configure os trechos de código a serem executados:

   * Clique em **[!UICONTROL Editar código da primeira chamada]** para definir o script a ser executado durante a primeira chamada.
   * Clique em **[!UICONTROL Editar código da próxima chamada]** para definir o script a ser executado durante as próximas chamadas do workflow. (opcional)

1. Para adicionar uma ou várias transições de saída, clique no link **[!UICONTROL Adicionar transições]** e especifique um rótulo e um nome interno para cada transição.

   Neste exemplo, configuramos duas transições que são ativadas pelo script no trecho de código com base em condições específicas.

   ![](../assets/javascript-transitions.png)

1. Conclua a configuração da atividade e inicie o workflow.

## Exemplo {#javascript-code-example}

### Inicializar variáveis com base na população recebida {#example1}

Este exemplo mostra como inicializar uma variável com base no número de perfis direcionados por um fluxo de trabalho.

![](../assets/javascript-example1.png)

Aqui, estamos direcionando perfis de VIP de nosso banco de dados. Queremos criar uma variável chamada &quot;canal&quot; com um valor que depende do número de perfis direcionados pela atividade Criar público:

* Se mais de 1000 perfis forem direcionados, inicialize a variável com o valor &quot;email&quot;.
* Caso contrário, inicialize-o com o valor &quot;sms&quot;.

Para fazer isso, siga estes passos:

1. Adicionar um **Código JavaScript** atividade com o tipo **Simples** depois que a variável **Criar público-alvo** atividade.

1. Clique em **Editar código** e configure o trecho de código conforme abaixo:

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. Inicie o workflow. A variável &quot;channel&quot; é criada com o valor &quot;email&quot; ou &quot;sms&quot;, dependendo do número de perfis direcionados pelo **Criar público-alvo** atividade.

### Acione transições com base no valor de uma variável {#example2}

Este exemplo mostra como acionar uma transição com base no valor de uma variável.

![](../assets/javascript-example2-transitions.png)

Aqui, o workflow começa com um **Sinal externo** atividade, na qual uma variável (`interest`) é transmitido de outro workflow. O valor da variável é &quot;running&quot; ou &quot;yoga&quot;, dependendo das operações de filtragem executadas no workflow inicial.

Queremos acionar transições diferentes no fluxo de trabalho, com base no valor da variável.

Para fazer isso, siga estes passos:

1. Adicionar um **Código JavaScript** atividade após a atividade External signal com o tipo **Avançado**.

1. Adicione duas transições: uma para cada valor variável possível (&quot;running&quot;, &quot;yoga&quot;).

1. Clique em **Editar código da primeira chamada** e configure o trecho de código conforme abaixo:

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Conclua a configuração de cada transição para atender às suas necessidades e, em seguida, inicie o fluxo de trabalho. Uma das duas transições de saída é ativada, com base no valor de `interest` variável que foi passada pela variável **Sinal externo** atividade.
