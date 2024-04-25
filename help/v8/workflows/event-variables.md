---
audience: end-user
title: Variáveis de evento do fluxo de trabalho
description: Saiba como aproveitar variáveis de evento em seus workflows.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 16%

---

# Variáveis de evento do fluxo de trabalho {#event-variables}

Algumas atividades de workflow permitem editar scripts no editor de expressão para executar ações específicas, como recuperar dados provenientes de atividades anteriores, condições de criação ou calcular nomes de arquivo com base em variáveis de evento.

## O que são variáveis de evento {#scripting}

Os scripts executados no contexto de um fluxo de trabalho acessam uma série de **objetos** como o próprio fluxo de trabalho que está sendo executado (`ìnstance`), as suas várias tarefas (`task`) ou os eventos que ativaram uma determinada tarefa (`event`).

Para cada tipo de **objeto** está associada a uma categoria de **variáveis** que podem ser aproveitadas no editor de expressão ao editar scripts em atividades como **[!UICONTROL Código JavaScript]** ou **[!UICONTROL Teste]**.

* **Variáveis de instância** (`instance.vars.xxx`) são comparáveis às variáveis globais. Eles são compartilhados por todas as atividades.
* **Variáveis de tarefa** (`task.vars.xxx`) são comparáveis às variáveis locais. São utilizadas somente pela tarefa atual. Essas variáveis são utilizadas por atividades persistentes para manter os dados e, às vezes, são utilizadas para troca de dados entre os diferentes scripts de uma mesma atividade.
* **Variáveis de evento** (`vars.xxx`) permitem a troca de dados entre as tarefas primárias de um processo de workflow. Essas variáveis são passadas pela tarefa que ativou a tarefa em andamento. Eles são passados para as atividades seguintes. **Variáveis de evento** são as variáveis usadas com mais frequência e devem ser usadas em detrimento de variáveis de instância.

>[!NOTE]
>
>Informações adicionais sobre scripts e os objetos e variáveis expostos no Adobe Campaign estão disponíveis na documentação do Campaign v8 (console do cliente) em [nesta seção](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Observe que, embora esse recurso ofereça insights valiosos, podem existir discrepâncias, pois ele se aplica especificamente ao console do cliente em vez da interface da Web do Campaign.

## Aproveitar variáveis de evento no editor de expressão {#expression-editor}

As variáveis de evento predefinidas estão disponíveis para uso no painel do lado esquerdo do editor de expressão. Você também pode criar novas variáveis inicializando uma nova variável no código.

![](assets/event-variables.png)

Além dessas variáveis de evento, você também pode aproveitar a variável **[!UICONTROL Condições]** no painel esquerdo para criar condições e a variável **[!UICONTROL Adicionar data atual]** para usar funções relacionadas à formatação de data.
