---
title: Introdução a perfis
description: Saiba como monitorar e gerenciar perfis na Web do Campaign.
badge: label="Disponibilidade limitada"
source-git-commit: 22b183a739dd92d7c4245fb4694034a247511d75
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 33%

---

# Introdução a perfis {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Visualização total dos perfis"
>abstract="Crie novos perfis e monitore-os com ferramentas e relatórios avançados. Acesse os atributos, as interações e os logs dos perfis. Use as opções de filtro para navegar na lista de perfis, editá-los e atualizá-los."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=pt-BR" text="Consulte as notas de versão"

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Visualização total dos perfis"
>abstract="Crie novos perfis e monitore-os com ferramentas e relatórios avançados. Acesse os atributos, as interações e os logs dos perfis. Use as opções de filtro para navegar na lista de perfis, editá-los e atualizá-los."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=pt-BR" text="Consulte as notas de versão"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfis"
>abstract="Um perfil é uma pessoa selecionada para receber mensagens enviadas pelo Adobe Campaign. Nessa lista, é possível exibir os detalhes dos perfis, com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos dos perfis."

## O que é um perfil? {#what}

Um perfil na Web do Adobe Campaign é um indivíduo armazenado no banco de dados, servindo como um componente-chave para [criar públicos](create-audience.md) para deliveries e [adicionar personalização](../personalization/personalize.md) dados ao seu conteúdo.

O Adobe Campaign permite criar e monitorar perfis diretamente na interface. A partir daí, você pode criar perfis, acessar uma visualização detalhada dos perfis e editá-los.

Outros tipos de perfis são armazenados no banco de dados, como **[!UICONTROL Perfis de teste]**, que são projetados para testar seus deliveries antes que sejam enviados ao público final. [Saiba como trabalhar com perfis de teste](test-profiles.md)

## Acessar a lista de perfis {#access}

Os perfis podem ser acessados e editados na Adobe Campaign Web a partir do **[!UICONTROL Gerenciamento de clientes]** > **Perfis** no painel de navegação esquerdo.

Também é possível acessá-las por meio da **[!UICONTROL Explorer]** exibir, no **[!UICONTROL Perfis e destinos]** > **[!UICONTROL Destinatários]** nó. Ali é possível navegar, criar e gerenciar pastas ou subpastas, bem como verificar permissões associadas. [Saiba como criar pastas](../get-started/permissions.md#folders)

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de perfis armazenados no banco de dados. [Saiba mais sobre permissões](../get-started/permissions.md).

É possível filtrar a variável **[!UICONTROL Perfis]** usando o campo de pesquisa ou os filtros disponíveis no **Mostrar filtros** botão. É possível restringir os resultados a um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png)

Para acessar os detalhes de um perfil, clique no nome na lista. Uma visualização detalhada do perfil é aberta, permitindo explorar seus atributos e os serviços aos quais ele se inscreveu. [Saiba como explorar os detalhes dos perfis](create-profile.md)

Para excluir um perfil, selecione a opção correspondente na **[!UICONTROL Mais ações]** menu.
