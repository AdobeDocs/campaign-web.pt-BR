---
audience: end-user
title: Usar a atividade de workflow Test
description: Saiba como usar a atividade de workflow de teste
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Teste {#test}

A atividade **Test** é uma atividade **Flow control**. Ela permite ativar transições com base em condições especificadas.

## Configurar a atividade Test {#test-configuration}

Siga estas etapas para configurar a atividade **Test**:

1. Adicione uma atividade **Test** no seu fluxo de trabalho.

1. Por padrão, a atividade **[!UICONTROL Test]** apresenta um teste booleano simples. Se a condição definida na transição &quot;True&quot; for atendida, essa transição será ativada. Caso contrário, uma transição padrão &quot;Falso&quot; será ativada.

1. Para configurar a condição associada a uma transição, clique no ícone **[!UICONTROL Abrir caixa de diálogo de personalização]**. Use o editor de expressão para definir as regras necessárias para ativar essa transição. Você também pode aproveitar variáveis de evento, condições e funções de data/hora. [Saiba como trabalhar com variáveis de evento e o editor de expressão](../event-variables.md)

   Além disso, você pode modificar o campo **[!UICONTROL Rótulo]** para personalizar o nome da transição na tela do fluxo de trabalho.

   ![](../assets/workflow-test-default.png)

1. Você pode adicionar várias transições de saída a uma atividade **[!UICONTROL Test]**. Para fazer isso, clique no botão **[!UICONTROL Adicionar condição]** e configure o rótulo e a condição associada para cada transição.

1. Durante a execução do workflow, cada condição é testada sequencialmente até que uma delas seja atendida. Se nenhuma das condições for atendida, o fluxo de trabalho continuará no caminho da **[!UICONTROL Condição padrão]**. Se nenhuma condição padrão for ativada, os workflows serão interrompidos nesse ponto.

## Exemplo {#example}

Neste exemplo, transições diferentes são ativadas com base no número de perfis segmentados por uma atividade **[!UICONTROL Criar público-alvo]**:
* Se mais de 10.000 perfis forem alvos, uma mensagem de email será enviada.
* Para 1.000 a 10.000 perfis, um SMS é enviado.
* Se os perfis direcionados ficarem abaixo de 1.000, serão direcionados para uma transição &quot;não entrar em contato&quot;.

![](../assets/workflow-test-example.png)

Para fazer isso, a variável de evento `vars.recCount` foi aproveitada nas condições &quot;email&quot; e &quot;sms&quot; para contar o número de perfis direcionados e ativar a transição apropriada.

![](../assets/workflow-test-example-config.png)
