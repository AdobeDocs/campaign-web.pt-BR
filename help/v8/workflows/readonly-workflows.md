---
audience: end-user
title: Sobre workflows somente leitura
description: Saiba por que os fluxos de trabalho estão no modo somente leitura
source-git-commit: 6985e8cb11f12ab7818cc71441a4d3b41f1a0493
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# Sobre workflows somente leitura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Este workflow é de somente leitura"
>abstract="Não é possível editar este workflow devido aos seus direitos ou ao tipo do workflow."

Alguns workflows podem estar no modo somente leitura. Você pode vê-lo com:

- A menção **[!UICONTROL ** Somente leitura **]**  perto do **[!UICONTROL Configurações]** botão
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
Os workflows técnicos incorporados estão no modo somente leitura para todos, mesmo para os usuários administradores. Mas o usuário pode **pause** ou **stop** se necessário. Essas são as únicas ações permitidas. [Saiba mais aqui](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}