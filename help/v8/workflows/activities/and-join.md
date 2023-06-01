---
audience: end-user
title: Usar a atividade de workflow AND-join
description: Saiba como usar a atividade de workflow AND-join
badge: label="Alpha" type="Positive"
source-git-commit: 6ed2c73a5348871348ec4cbdd89fc8119fdbc718
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 4%

---


# AND-join {#join}

A variável **Associação AND** A atividade permite sincronizar várias ramificações de execução de um fluxo de trabalho.

A atividade AND-join só acionará a transição de saída depois que todas as transições de entrada forem ativadas, ou seja, depois que todas as atividades anteriores forem concluídas.

## Configuração

Siga estas etapas para configurar o **AND-join** atividade:

1. Adicione várias atividades, como **Combinar** para formar pelo menos duas ramificações de execução diferentes.
1. Adicionar um **AND-join** atividade a qualquer uma das ramificações.
1. No **Opções de mesclagem** marque todas as atividades anteriores nas quais deseja participar.
1. Selecione o **Conjunto principal** a ser mantido na transição de saída.

## Exemplo

O exemplo a seguir mostra duas ramificações de fluxo de trabalho com um delivery de email e SMS. A associação AND será acionada quando ambas as transições de entrada estiverem ativadas. As notificações por push serão enviadas somente após a conclusão de ambos os deliveries.

![](../assets/workflow-andjoin-example.png)