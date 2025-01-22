---
audience: end-user
title: Sobre fluxos de trabalho de somente leitura
description: Saiba por que os fluxos de trabalho estão no modo somente leitura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 62d4733b9dc6bf3edf06d172069b5f8b1d0ee4a7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 13%

---

# Sobre fluxos de trabalho de somente leitura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Este workflow é de somente leitura"
>abstract="Não é possível editar esse fluxo de trabalho devido aos seus direitos ou ao tipo de fluxo de trabalho."

Alguns workflows podem estar no modo somente leitura. Você pode vê-lo com:

- A menção **[!UICONTROL Somente leitura]** próxima ao botão **[!UICONTROL Configurações]**
- Os botões de ação não estão acessíveis

![](assets/readonly-workflow.png){zoomable="yes"}

Não é possível editar nada em um fluxo de trabalho somente leitura. Você não tem permissão para alterar as configurações das atividades.


![](assets/scheduler-readonly.png){zoomable="yes"}


Você também não tem os direitos para excluir o workflow.

![](assets/readonly-rights.png){zoomable="yes"}

## Por que workflows somente leitura

O modo somente leitura é para usuários que não têm permissão e direitos de acesso para editar esses workflows. [Saiba mais aqui](../get-started/permissions.md)

Um usuário da campanha pode ter restrições nos dados que pode acessar no Adobe Campaign. O administrador pode dar a ele a possibilidade de ver alguns recursos, mas não de trabalhar neles.

## Tipos de workflows somente leitura

De acordo com o tipo de fluxo de trabalho, o modo somente leitura pode ser diferente.

### Fluxos de trabalho da campanha

No caso de um workflow de campanha somente leitura, o usuário não consegue acessar o botão de monitoramento.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows técnicos

Os workflows técnicos estão no modo somente leitura para usuários do Campaign.
Os workflows técnicos incorporados estão no modo somente leitura para todos, mesmo para os usuários administradores. Mas o usuário pode **pausar** ou **parar**, se necessário. Essas são as únicas ações permitidas. [Saiba mais aqui](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}
