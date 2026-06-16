---
audience: end-user
title: Use a atividade End workflow
description: Saiba como usar a atividade End workflow
source-git-commit: a9c701b9c3ac2d16d8a2dda8e851f09ac801a13e
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 20%

---

# Fim {#end}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Finalizar atividade"
>abstract="A atividade **Fim** permite marcar graficamente o final de um fluxo de trabalho. Quando mais de uma transição de entrada estiver disponível, use a seção **Conjuntos para ingressar** para selecionar quais transições se conectar à atividade."

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_sets"
>title="Conjuntos para unir"
>abstract="Verifique as atividades anteriores que deseja conectar como transições de entrada da atividade **End**. As atividades selecionadas são conectadas ao **Fim**. Esta seção é exibida somente quando mais de uma transição de entrada está disponível para ser conectada à atividade."

>[!CONTEXTUALHELP]
>id="acw_orchestration_signal"
>title="Sinal externo"
>abstract="Espaço reservado da seção de sinais externos nos parâmetros da atividade final. Disponível somente para campanhas orquestradas. NÃO EXCLUIR"

A atividade **End** é uma atividade **Flow control**. Ela permite marcar graficamente o final de um workflow. Essa atividade é opcional.

A atividade oferece suporte a várias transições de entrada quando mais de uma transição de entrada está disponível.

Na seção **Conjuntos para ingressar**, marque as atividades anteriores que você deseja conectar como transições de entrada da atividade **Fim**. As atividades selecionadas são vinculadas ao **End** na tela de fluxo de trabalho.

![Processo de configuração de eliminação de duplicação do fluxo de trabalho](../assets/workflow-end.png)
