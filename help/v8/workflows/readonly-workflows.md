---
audience: end-user
title: Sobre fluxos de trabalho de somente leitura
description: Saiba por que os fluxos de trabalho estão no modo somente leitura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 13%

---

# Sobre fluxos de trabalho de somente leitura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Este workflow é de somente leitura"
>abstract="Não é possível editar esse fluxo de trabalho devido aos seus direitos ou ao tipo de fluxo de trabalho."

Alguns fluxos de trabalho estão no modo somente leitura. Os workflows técnicos incorporados são sempre somente leitura, mas essa obstrução também pode ser ativada em outros tipos de workflow.

Os usuários do Campaign podem ter acesso restrito aos dados do Adobe Campaign. Um administrador do Campaign pode conceder a eles o direito de visualizar alguns recursos, mas não de editá-los ou modificá-los. As permissões do usuário em dados são fundamentais para garantir a segurança dos dados e do processo. Saiba mais sobre o gerenciamento de permissões no Campaign em [esta seção](../get-started/permissions.md)

Quando um fluxo de trabalho está no modo somente leitura:

* A menção **[!UICONTROL Somente leitura]** próxima ao botão **[!UICONTROL Configurações]**
* Os botões de ação não estão acessíveis

![](assets/readonly-workflow.png){zoomable="yes"}

Os usuários não podem editar nada em um fluxo de trabalho somente leitura. não é permitido alterar as configurações das atividades.

![](assets/scheduler-readonly.png){zoomable="yes"}

Os usuários não podem excluir o workflow.

![](assets/readonly-rights.png){zoomable="yes"}


## Tipos de workflows somente leitura {#readonly-workflow-types}

De acordo com o tipo de fluxo de trabalho, o modo somente leitura pode ser diferente.

### Fluxos de trabalho da campanha {#readonly-campaign-wf}

No caso de um workflow de campanha somente leitura, o usuário não consegue acessar o botão de monitoramento.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows técnicos {#readonly-tech-wf}

Os workflows técnicos incorporados são somente leitura para todos os usuários do Campaign, até mesmo para o administrador. No entanto, os usuários podem **pausar** ou **parar**, se necessário. Essas são as únicas ações permitidas.

![](assets/readonly-technical-workflow.png){zoomable="yes"}

Saiba mais sobre fluxos de trabalho técnicos em [esta seção](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)
