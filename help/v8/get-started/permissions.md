---
audience: end-user
title: Gerenciamento de permissões na Web do Campaign
description: Saiba mais sobre permissões no Campaign web v8
badge: label="Beta"
source-git-commit: 5c7d60b3f59de2a5176a55d9556a3f1c6d2a7651
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---


# Acesso e permissões {#access-and-permissions}

O controle de acesso pode restringir o acesso a objetos e dados de listas principais, como deliveries, recipients ou workflows. Essas restrições também se aplicam à árvore de navegação do Explorer. Além disso, você precisa de permissões para criar, excluir, duplicar e editar objetos na interface do usuário. O controle de acesso é gerenciado no Console do cliente. Todas as permissões na Web do Campaign são sincronizadas com as permissões do Console do cliente do Campaign. Somente administradores do Campaign podem definir e modificar permissões de usuário. Saiba mais sobre permissões de usuário no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html){target="_blank"}.

Ao navegar pela interface do usuário da Web do Campaign, você pode acessar dados, objetos e recursos dependendo das suas permissões. Por exemplo, se você não tiver permissões de acesso a uma pasta, não poderá vê-la. Suas permissões também afetam objetos e o gerenciamento de dados. Sem permissões de Gravação para uma pasta específica, não é possível criar um delivery nessa pasta, mesmo que você possa vê-lo na interface do usuário.

## Exibir permissões {#view-permissions}

No **Explorer**, você pode procurar permissões para cada pasta. Essas permissões são definidas no console do cliente e usadas para organizar e controlar o acesso aos dados do Campaign.


Para exibir permissões de uma pasta, siga estas etapas:

1. No **Explorer** selecione uma pasta no menu de navegação esquerdo.
1. Clique nos três pontos no canto superior direito e selecione **Permissões de pasta**.

   ![](assets/permissions-view-menu.png){width="70%" align="left" zoomable="yes"}

1. Verifique os detalhes na tela, conforme abaixo:

   ![](assets/permissions-view-screen.png){width="70%" align="left" zoomable="yes"}

   Um grupo ou operador pode ter permissões de Leitura, Gravação e/ou Exclusão nos dados armazenados na pasta selecionada.

   Se a variável **Propagar** estiver ativada, todas as permissões definidas para uma pasta serão aplicadas a todas as suas subpastas. Essas permissões podem ser sobrecarregadas para cada subpasta.

   Se a variável **Pasta do sistema** estiver ativada, o acesso será permitido a todos os operadores, independentemente das permissões.

Saiba mais sobre permissões de pasta em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html){target="_blank"}.


## Trabalhar com pastas {#folders}

Você pode criar, renomear, reordenar e mover pastas para organizar seus componentes e dados. Também é possível excluir pastas do mesmo menu.

>[!CAUTION]
>
>Ao excluir uma pasta, todos os dados armazenados nela também são excluídos.

Para criar uma pasta, siga estas etapas:

1. No **Explorer** selecione uma pasta no menu de navegação esquerdo.
1. Clique nos três pontos no canto superior direito e escolha **Criar nova subpasta**.
1. Insira o nome da pasta e salve.

   ![](assets/create-new-subfolder.png){width="70%" align="left" zoomable="yes"}

   A pasta é adicionada como uma subpasta da pasta atual. Navegue até essa nova pasta para criar componentes diretamente nela. Você também pode criar um componente de qualquer pasta e salvá-lo nessa nova pasta, na **Opções adicionais** das propriedades, conforme mostrado abaixo para um delivery:

   ![](assets/delivery-properties-folder.png){width="70%" align="left" zoomable="yes"}

