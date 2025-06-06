---
audience: end-user
title: Usar a atividade de workflow Test
description: Saiba como usar a atividade de workflow de teste
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 37%

---


# Teste {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Atividade de teste"
>abstract="A atividade **Teste** é uma atividade de **Controle de fluxo**. Ela permite habilitar transições com base nas condições especificadas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Condições"
>abstract="A atividade **Teste** pode ter várias transições de saída. Durante a execução do fluxo de trabalho, cada condição é testada sequencialmente até que uma delas seja atendida. Se nenhuma das condições for atendida, o fluxo de trabalho continuará com base na **[!UICONTROL condição padrão]**. Se nenhuma condição padrão for ativada, o fluxo de trabalho é interrompido neste ponto."

A atividade **Teste** é uma atividade de **Controle de fluxo**. Ela permite habilitar transições com base nas condições especificadas.

## Configurar a atividade Test {#test-configuration}

Siga estas etapas para configurar a atividade **Test**:

1. Adicione uma atividade **Test** no seu fluxo de trabalho.

1. Por padrão, a atividade **[!UICONTROL Test]** apresenta um teste booleano simples. Se a condição definida na transição &quot;True&quot; for atendida, essa transição será ativada. Caso contrário, uma transição padrão &quot;Falso&quot; será ativada.

1. Para configurar a condição associada a uma transição, clique no ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**. Use o editor de expressão para definir as regras necessárias para ativar essa transição. Você também pode usar variáveis de evento, condições e funções de data/hora. [Saiba como trabalhar com variáveis de evento e o editor de expressão](../event-variables.md).

   Além disso, modifique o campo **[!UICONTROL Rótulo]** para personalizar o nome da transição na tela do fluxo de trabalho.

   ![Configuração padrão da atividade Test](../assets/workflow-test-default.png)

1. Adicione várias transições de saída a uma atividade **[!UICONTROL Test]**. Para fazer isso, clique no botão **[!UICONTROL Adicionar condição]** e configure o rótulo e a condição associada para cada transição.

1. Durante a execução do fluxo de trabalho, cada condição é testada sequencialmente até que uma delas seja atendida. Se nenhuma das condições for atendida, o fluxo de trabalho continuará com base na **[!UICONTROL condição padrão]**. Se nenhuma condição padrão for ativada, o fluxo de trabalho é interrompido neste ponto.

## Exemplo {#example}

Neste exemplo, transições diferentes são ativadas com base no número de perfis segmentados por uma atividade **[!UICONTROL Criar público-alvo]**:
* Se mais de 10.000 perfis forem alvos, uma mensagem de email será enviada.
* Para 1.000 a 10.000 perfis, um SMS é enviado.
* Se os perfis direcionados ficarem abaixo de 1.000, serão direcionados para uma transição &quot;não entrar em contato&quot;.

![Exemplo de transições de atividade de teste](../assets/workflow-test-example.png)

Para isso, a variável de evento `vars.recCount` é usada nas condições &quot;email&quot; e &quot;sms&quot; para contar o número de perfis segmentados e ativar a transição apropriada.

![Configuração do exemplo de atividade Test](../assets/workflow-test-example-config.png)
