---
title: Conectar-se à interface web do Adobe Campaign
description: Saiba como se conectar à interface do Adobe Campaign Web
exl-id: 5a8023a9-5b9e-429f-ba56-b01423993e55
source-git-commit: 8006eeb6088d7d6ef99f374b2b846978cd679c01
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 68%

---

# Conexão com o Adobe Campaign {#connect-to-campaign}

A Experience Cloud é a família integrada de aplicativos, produtos e serviços de marketing digital da Adobe. Com sua interface intuitiva, você pode acessar rapidamente os aplicativos em nuvem, recursos do produto e serviços. Saiba como se conectar ao Adobe Experience Cloud e acessar a interface da Web do Adobe Campaign nesta página.

## Fazer logon na Adobe Experience Cloud {#sign-in-to-exc}

Você também pode usar o logon único (SSO) para se conectar ao Campaign. Normalmente, admins da Experience Cloud são responsáveis por conceder acesso a aplicativos e serviços. Siga as etapas no convite para a Experience Cloud enviado por email.

Para fazer logon no Adobe Experience Cloud, siga estas etapas básicas:

1. Navegue até [Adobe Experience Cloud](https://experience.adobe.com/){target="_blank"}.

1. Faça logon usando sua Adobe ID ou Enterprise ID. Saiba mais sobre os tipos de identidade na Adobe em [este artigo](https://helpx.adobe.com/br/enterprise/using/identity.html){target="_blank"}.

   Depois de fazer logon na Experience Cloud, você pode acessar rapidamente todas as soluções e aplicativos.

   ![Captura de tela mostrando a página inicial do Adobe Experience Cloud](assets/exc-home.png){zoomable="yes"}

1. Verifique se você está na organização correta.

   ![Captura de tela mostrando a seleção da organização no Adobe Experience Cloud](assets/exc-orgs.png){zoomable="yes"}{width="50%" align="left"}

   Saiba mais sobre organizações na Adobe Experience Cloud em [este artigo](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=pt-BR){target="_blank"}.

## Acesso ao Adobe Campaign {#access-to-campaign}

Para acessar o ambiente do Campaign, selecione **Campaign** na seção **Acesso rápido** da página inicial da Adobe Experience Cloud.

Se você já estiver conectado a outra solução da Adobe Experience Cloud, navegue até o ambiente do Campaign a partir do alternador de soluções na parte superior direita da tela.

![Captura de tela mostrando o alternador de soluções no Adobe Experience Cloud](assets/solution-switcher.png){zoomable="yes"}

Se você tiver acesso a vários ambientes, incluindo o Painel de controle do Campaign, clique no botão **Iniciar** da instância correta.

![Captura de tela mostrando o botão Iniciar para Adobe Campaign](assets/launch-campaign.png){zoomable="yes"}

Agora você está conectado ao Campaign. Saiba como começar a usar a interface [nesta página](user-interface.md).

### Controle de acesso {#access-control}

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
>abstract="Você não tem permissão para editar este perfil. Se necessário, entre em contato com a sua administração para obter acesso."

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

O controle de acesso restringe o acesso a objetos e dados de listas principais, como deliveries, recipients ou workflows. Essas restrições aplicam-se também à árvore de navegação do Explorer. Além disso, você precisa de permissões para criar, excluir, duplicar e editar objetos na interface.

Todas as permissões no Campaign Web são sincronizadas com as permissões do Console do cliente do Campaign. Somente admins do Campaign podem definir e modificar permissões de usuário. 

Conforme você navega pela interface da Web do Campaign, é possível acessar dados, objetos e recursos, dependendo das suas permissões. Por exemplo, caso não possua permissões de acesso a uma pasta, você não poderá vê-la. Suas permissões também afetam objetos e o gerenciamento de dados. Sem permissões de gravação para uma pasta específica, não é possível criar uma entrega nessa pasta, mesmo que você possa vê-la na interface.

Para aprender a exibir e gerenciar permissões, [consulte esta página](permissions.md).

## Navegação superior da Adobe Experience Cloud {#top-bar}

Navegue na barra superior da interface para:

* Compartilhar feedback sobre a interface do usuário da Web do Campaign.
* Alternar entre suas organizações.
* Alternar entre as soluções e os aplicativos da Adobe Experience Cloud.
* Procure ajuda sobre a [Adobe Experience League](https://experienceleague.adobe.com/docs/?lang=pt-BR){target="_blank"}.
* Verifique as notificações do produto.
* Edite seu perfil do Adobe e gerencie configurações, como [atualizar seu idioma favorito](#language-pref) ou [alternar para o tema claro/escuro](#dark-theme).

![Captura de tela mostrando a barra de navegação superior do Adobe Experience Cloud](assets/do-not-localize/unified-shell.png){zoomable="yes"}{width="50%" align="left"}

## Navegadores compatíveis {#browsers}

O Adobe Campaign Web foi desenvolvido para funcionar de maneira ideal na versão mais recente do Google Chrome, Safari e Microsoft Edge. Você pode encontrar problemas ao usar determinados recursos em versões mais antigas ou outros navegadores.

## Preferências de idioma {#language-pref}

Atualmente, o Adobe Campaign Web está disponível nos seguintes idiomas:

* Inglês (EUA) - EN-US
* Francês - FR
* Alemão - DE
* Italiano - IT
* Espanhol - ES
* Português (Brasil) - PTBR
* Japonês - JP
* Coreano - KR
* Chinês simplificado - CHS
* Chinês tradicional - CHT

O idioma padrão do Campaign Web é determinado pelo idioma preferencial especificado no perfil de usuário. Ele não está relacionado ao idioma do servidor do Campaign e do console do cliente.

Para alterar o idioma:

1. Clique no ícone do perfil, na parte superior direita, e selecione **Preferências**.
1. Clique no link do idioma exibido sob seu endereço de email.
1. Selecione o idioma de sua preferência e clique em **Salvar**. Você pode selecionar um segundo idioma caso o componente usado não esteja traduzido em seu idioma nativo.


## Temas escuro e claro {#dark-theme}

O Adobe Campaign está disponível em temas claros e escuros. Por padrão, a interface é habilitada no tema claro. Para alternar para o tema escuro, clique no ícone do seu perfil e use a opção **Tema escuro** para habilitá-lo ou desabilitá-lo.

As configurações de perfil do usuário e as preferências da conta estão detalhadas [nesta seção](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=pt-BR#preferences){target="_blank"}.

Saiba mais sobre os componentes da interface central da Experience Cloud [nesta documentação](https://experienceleague.adobe.com/docs/core-services/interface/experience-cloud.html?lang=pt-BR){target="_blank"}.