---
audience: end-user
title: Sobre fluxos de trabalho de somente leitura
description: Saiba por que os fluxos de trabalho estão no modo somente leitura
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 4%

---

# Sobre fluxos de trabalho de somente leitura {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="This workflow is read only"
>abstract="You cannot edit this workflow due to your rights or the type of the workflow."

Os usuários do Campaign podem ter acesso restrito aos dados do Adobe Campaign. Um administrador do Campaign pode conceder a ele o direito de exibir determinados recursos, mas não de editá-los ou modificá-los. As permissões do usuário em dados são essenciais para garantir a segurança dos dados e do processo. Saiba mais sobre o gerenciamento de permissões no Campaign em [esta seção](../get-started/permissions.md).

Quando um fluxo de trabalho está no modo somente leitura:

* A menção **[!UICONTROL Somente leitura]** aparece próxima ao botão **[!UICONTROL Configurações]**.
* Os botões de ação não estão acessíveis.

![Interface de fluxo de trabalho somente leitura mostrando o botão de configurações e os botões de ação desabilitados.](assets/readonly-workflow.png){zoomable="yes"}

Os usuários não podem editar nada em um fluxo de trabalho somente leitura. Eles não têm permissão para alterar as configurações das atividades.

![Interface do agendador no modo somente leitura, mostrando opções de configurações desabilitadas.](assets/scheduler-readonly.png){zoomable="yes"}

Os usuários não podem excluir o workflow.

![Interface mostrando direitos restritos para excluir fluxos de trabalho.](assets/readonly-rights.png){zoomable="yes"}

## Tipos de workflows somente leitura {#readonly-workflow-types}

Dependendo do tipo de workflow, o modo somente leitura pode variar.

### Fluxos de trabalho da campanha {#readonly-campaign-wf}

Em um workflow de campanha somente leitura, o usuário não consegue acessar o botão de monitoramento.

![Interface do fluxo de trabalho do Campaign no modo somente leitura, mostrando as opções de monitoramento desabilitadas.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Workflows técnicos {#readonly-tech-wf}

Os workflows técnicos incorporados são somente leitura para todos os usuários do Campaign, incluindo administradores. No entanto, os usuários podem **pausar** ou **parar**, se necessário. Essas são as únicas ações permitidas.

![Interface de fluxo de trabalho técnico no modo somente leitura, mostrando opções para pausar ou parar fluxos de trabalho.](assets/readonly-technical-workflow.png){zoomable="yes"}

Saiba mais sobre fluxos de trabalho técnicos em [esta seção](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).