---
audience: end-user
title: Usar a atividade de workflow AND-join
description: Saiba como usar a atividade de workflow AND-join
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 17%

---


# AND-join {#join}

A variável **Associação AND** a atividade é um **Controle de fluxo** atividade. Ela permite sincronizar várias ramificações de execução de um fluxo de trabalho.

Essa atividade só acionará a transição de saída depois que todas as transições de entrada estiverem ativadas, ou seja, depois que todas as atividades anteriores estiverem concluídas. Isso permite verificar se determinadas atividades foram concluídas antes de continuar a executar o workflow.

## Configuração

Siga estas etapas para configurar o **AND-join** atividade:

1. Adicione várias atividades, como atividades de canal, para formar pelo menos duas ramificações de execução diferentes.
1. Adicionar um **AND-join** atividade a qualquer uma das ramificações.
1. No **Opções de mesclagem** marque todas as atividades anteriores nas quais deseja participar.
1. No **Conjunto principal** escolha a população de transição de entrada que deseja manter. A transição de saída só pode conter uma das populações de transição de entrada.

## Exemplo

O exemplo a seguir mostra duas ramificações de fluxo de trabalho com um delivery de email e SMS. A associação AND será acionada quando ambas as transições de entrada estiverem ativadas. As notificações por push serão enviadas somente após a conclusão de ambos os deliveries.

![](../assets/workflow-andjoin-example.png)