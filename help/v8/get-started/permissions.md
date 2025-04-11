---
audience: end-user
title: Gerenciamento de permissões na interface do Campaign Web
description: Saiba mais sobre permissões na interface do Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 14%

---

# Permissões {#permissions}

Cada usuário no Adobe Campaign tem permissões e restrições específicas no aplicativo. O usuário pode pertencer a um grupo de operadores e herdar as permissões do grupo.

Com base em suas permissões, um operador pode:

* Acessar determinados recursos
* Acessar determinados dados
* Acessar determinadas ações (criar, modificar, excluir)

Um procedimento detalhado para configurar permissões no Adobe Campaign está disponível na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.

## Permissões de pastas {#folder-permissions}

Com base nos seus direitos, você pode exibir e gerenciar permissões em pastas nas **[!UICONTROL Configurações de pasta]**.

Veja abaixo um exemplo de uma pasta de delivery:

![Exemplo de configurações de pasta no Adobe Campaign](assets/folder_settings.png){zoomable="yes"}

Na seção **[!UICONTROL Segurança]** das **[!UICONTROL Configurações de pasta]**, você pode exibir e gerenciar (adicionar ou excluir) operadores ou grupos que podem acessar a pasta.

![Exemplo de configurações de segurança de pasta no Adobe Campaign](assets/folder_security.png){zoomable="yes"}

Você pode clicar diretamente nas permissões e alterá-las para **[!UICONTROL Permitidas]** ou **[!UICONTROL Negadas]**.

![Exemplo de permissões negadas nas configurações de segurança da pasta](assets/folder_security_denied.png){zoomable="yes"}

Se a opção **[!UICONTROL Propagar]** estiver habilitada, todas as permissões definidas para uma pasta serão aplicadas a todas as suas subpastas. Essas permissões podem ser substituídas para cada subpasta.

Se a opção **[!UICONTROL Pasta do sistema]** for selecionada, o acesso será permitido a todos os operadores, independentemente de suas permissões.

Também é possível [gerenciar as permissões nas pastas do console do Adobe Campaign](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Todas as permissões na interface da Web do Campaign são sincronizadas com as permissões do Console do cliente do Campaign.