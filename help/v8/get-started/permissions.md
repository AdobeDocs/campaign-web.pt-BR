---
audience: end-user
title: Gerenciamento de permissões na interface do Campaign Web
description: Saiba mais sobre permissões na interface do Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f352f4e726eff50527d0b9a04d0506600c12b822
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 18%

---


# Permissões {#permissions}

Cada usuário no Adobe Campaign tem suas próprias permissões e restrições no aplicativo. O usuário pode fazer parte de um grupo de operadores e herdar as permissões do grupo.

De acordo com suas permissões, um operador pode:

* Acesso a determinados recursos
* Acesso a determinados dados
* Acesso a determinadas ações (criar, modificar, excluir)

O procedimento detalhado para configurar permissões no Adobe Campaign está disponível na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Permissões em pastas {#folder-permissions}

De acordo com seus direitos, você tem a possibilidade de exibir e gerenciar as permissões em pastas nas **[!UICONTROL Configurações de pasta]**.

Veja abaixo um exemplo de uma pasta de delivery:

![](assets/folder_settings.png){zoomable="yes"}

Na seção **[!UICONTROL Segurança]** das **[!UICONTROL Configurações de pasta]**, você pode exibir e gerenciar (adicionar ou excluir) operadores ou grupos que podem acessar a pasta.

![](assets/folder_security.png){zoomable="yes"}

Você pode clicar diretamente nas permissões e alterá-las **[!UICONTROL Permitidas]** ou **[!UICONTROL Negadas]**.

![](assets/folder_security_denied.png){zoomable="yes"}

Se a opção **[!UICONTROL Propagar]** estiver habilitada, todas as permissões definidas para uma pasta serão aplicadas às suas subpastas. Essas permissões podem ser sobrecarregadas para cada subpasta.

Se a opção **[!UICONTROL Pasta do sistema]** estiver marcada, o acesso será permitido para todos os operadores, independentemente de suas permissões.

Você também pode [gerenciar as permissões nas pastas no console do Adobe Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Todas as permissões na interface da Web do Campaign são sincronizadas com as permissões do Console do cliente do Campaign.
