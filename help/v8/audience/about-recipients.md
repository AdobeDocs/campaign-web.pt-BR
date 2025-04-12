---
title: Introdução a perfis
description: Saiba como monitorar e gerenciar perfis na Web do Campaign.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 11%

---

# Introdução a perfis {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfis"
>abstract="Um perfil é um registro direcionado para receber mensagens enviadas pelo Adobe Campaign. Nessa lista, é possível exibir os detalhes dos perfis, com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos dos perfis."

## O que é um perfil? {#what}

Um **perfil**, também conhecido como &quot;recipient&quot; no console do cliente, representa um registro armazenado no banco de dados do Campaign. Ele serve como um componente principal para [criar públicos-alvo](create-audience.md) para entregas e [adicionar dados de personalização](../personalization/personalize.md) ao seu conteúdo. O Adobe Campaign permite o gerenciamento perfeito de perfis, incluindo a criação de novas entradas e o acesso a uma visualização abrangente de todos os atributos e assinaturas de serviço dos perfis, por meio da interface do usuário na Web do Campaign.

Além disso, os **[!UICONTROL perfis de teste]**, identificados como &quot;perfis iniciais&quot; no console do cliente, permitem o direcionamento de recipients adicionais que não correspondem aos critérios de direcionamento de uma determinada entrega. Esses perfis contêm informações de contato fictícias ou informações de contato controladas pelo remetente. Os perfis de teste são recipients de prova usados para testar mensagens enviando provas. [Saiba como trabalhar com perfis de teste](test-profiles.md)

Os perfis e os perfis de teste são úteis para testar as entregas antes que elas atinjam o público-alvo desejado. Isso permite a visualização do conteúdo e da personalização da mensagem, o envio de provas para teste e validação, a avaliação da renderização de email em várias plataformas e dispositivos e o teste de landing pages. [Saiba como visualizar e testar entregas](../preview-test/preview-test.md)

➡️ [Conheça este recurso no vídeo](#video)

## Acessar a lista de perfis {#access}

Os perfis podem ser acessados e editados na Adobe Campaign Web a partir da entrada **[!UICONTROL Gerenciamento de clientes]** > **Perfis** no painel de navegação esquerdo. Eles também podem ser acessados na exibição **[!UICONTROL Explorer]**, no nó **[!UICONTROL Perfis e Destinos]** > **[!UICONTROL Destinatários]**. Nela, navegue, crie e gerencie pastas ou subpastas, bem como verifique as permissões associadas. [Saiba como criar pastas](../get-started/permissions.md#folders).

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de perfis armazenados no banco de dados. [Saiba mais sobre permissões](../get-started/permissions.md)

Filtre a lista **[!UICONTROL Perfis]** usando o campo de pesquisa ou os filtros disponíveis no botão **Mostrar filtros**. Restrinja os resultados a uma [pasta](../get-started/permissions.md#folders) específica usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![Filtros disponíveis na lista de perfis](assets/profiles-list-filters.png){zoomable="yes"}

Para acessar os detalhes de um perfil, clique no nome na lista. Uma visualização detalhada do perfil é aberta, permitindo a exploração de seus atributos e os serviços aos quais o perfil se inscreveu. [Saiba como explorar os detalhes dos perfis](create-profile.md)

Para excluir um perfil, selecione a opção correspondente no menu **[!UICONTROL Mais ações]**.

## Vídeo tutorial {#video}

Saiba como acessar, gerenciar e explorar perfis usando a interface da Web do Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)