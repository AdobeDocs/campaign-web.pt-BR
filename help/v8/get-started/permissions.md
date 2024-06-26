---
audience: end-user
title: Gerenciamento de permissões na interface do Campaign Web
description: Saiba mais sobre permissões na interface do Campaign Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: b173afc12a5d8a7c57c688fe92e2c5628323fcad
workflow-type: ht
source-wordcount: '645'
ht-degree: 100%

---

# Acesso e permissões {#access-and-permissions}

>[!CONTEXTUALHELP]
>id="acw_explorer_permissions_create"
>title="Permissão necessária"
>abstract="A administração precisa conceder a permissão para que você possa criar este objeto."

>[!CONTEXTUALHELP]
>id="acw_audiences_read_only"
>title="Este público-alvo é somente de leitura"
>abstract="Você não tem permissões para editar este público-alvo. Se necessário, entre em contato com a sua administração para obter acesso."

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="Este serviço é somente de leitura."
>abstract="Você não tem permissões para editar este serviço. Se necessário, entre em contato com a sua administração para obter acesso."

>[!CONTEXTUALHELP]
>id="acw_recipients_readonlyprofile"
>title="Perfil de somente leitura de destinatários"
>abstract="Você não tem permissões para editar este perfil. Se necessário, entre em contato com a sua administração para obter acesso."

>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="Esta campanha é somente de leitura"
>abstract="Você não tem permissões para editar esta campanha. Se necessário, entre em contato com a sua administração para obter acesso."

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="Esta entrega é somente de leitura"
>abstract="Você não tem permissões para editar esta entrega. Se necessário, entre em contato com a sua administração para obter acesso."


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="Este workflow é de somente leitura"
>abstract="Você não tem permissões para editar este fluxo de trabalho. Se necessário, entre em contato com a sua administração para obter acesso."



O controle de acesso pode restringir o acesso a objetos e dados de listas principais, como entregas, destinatários ou fluxos de trabalho. Estas restrições aplicam-se também à árvore de navegação do **Explorer**. Além disso, você precisa de permissões para criar, excluir, duplicar e editar objetos na interface.

O controle de acesso é gerenciado no console do cliente do Campaign. Todas as permissões no Campaign Web são sincronizadas com as permissões do console do cliente do Campaign. Somente admins do Campaign podem definir e modificar permissões de usuário. Saiba mais sobre permissões de usuário na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/gs-permissions.html?lang=pt-BR){target="_blank"}.

Ao navegar pela interface do Campaign Web, você pode acessar dados, objetos e recursos, dependendo das suas permissões. Por exemplo, caso não possua permissões de acesso a uma pasta, você não poderá vê-la. Suas permissões também afetam objetos e o gerenciamento de dados. Sem permissões de gravação para uma pasta específica, não é possível criar uma entrega nessa pasta, mesmo que você possa vê-la na interface.

## Exibir permissões {#view-permissions}

No **Explorer**, você pode procurar as permissões para cada pasta. Essas permissões são definidas no console do cliente e usadas para organizar e controlar o acesso aos dados do Campaign.

Para exibir as permissões de uma pasta, siga estas etapas:

1. No menu de navegação esquerdo do **Explorer**, selecione uma pasta.
1. Clique nos três pontos no canto superior direito e selecione **Permissões da pasta**.

   ![](assets/permissions-view-menu.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Verifique os detalhes na tela, conforme abaixo:

   ![](assets/permissions-view-screen.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

   Um grupo ou operador(a) pode ter permissões de Leitura, Gravação e/ou Exclusão para dados armazenados na pasta selecionada.

   Se a opção **Propagar** estiver habilitada, todas as permissões definidas para uma pasta serão aplicadas às suas subpastas. Essas permissões podem ser sobrecarregadas para cada subpasta.

   Se a opção **Pasta do sistema** estiver habilitada, o acesso será permitido a todos os operadores, independentemente das permissões.

Saiba mais sobre permissões de pasta na [documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/admin/permissions/folder-permissions.html?lang=pt-BR){target="_blank"}.


## Trabalhar com pastas {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="Propriedades da pasta"
>abstract="Propriedades da pasta"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="Segurança da pasta"
>abstract="Segurança da pasta"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="Restrições da pasta"
>abstract="Restrições da pasta"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Programação da pasta"
>abstract="Programação da pasta"

Você pode criar, renomear, reordenar e mover pastas para organizar seus componentes e dados. Também é possível excluir pastas no mesmo menu.

>[!CAUTION]
>
>Ao excluir uma pasta, todos os dados armazenados nela também são excluídos.

Para criar uma pasta, siga estas etapas:

1. No menu de navegação esquerdo do **Explorer**, selecione uma pasta.
1. Clique nos três pontos no canto superior direito e escolha **Criar nova pasta**.
1. Insira o nome da pasta.

   ![](assets/create-new-subfolder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Selecione o tipo da pasta. Por padrão, o tipo da pasta principal é selecionado, “Entregas”, em nosso exemplo. Para alterar o tipo da pasta, clique no ícone de pasta e selecione qualquer outro tipo.

   ![](assets/create-new-subfolder2.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

1. Clique em **Create**.

   A pasta é adicionada como uma subpasta da pasta atual. Navegue até essa nova pasta para criar componentes diretamente a partir dela. Você também pode criar um componente em qualquer pasta e salvá-lo nessa nova pasta utilizando a seção **Opções adicionais** das propriedades, conforme o exemplo de entrega abaixo:

   ![](assets/delivery-properties-folder.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}
