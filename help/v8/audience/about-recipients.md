---
title: Introdução a perfis
description: Saiba como monitorar e gerenciar perfis na Web do Campaign.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 5a4bf85a1f70a0282405aededfb31038f9db17a8
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 14%

---

# Introdução a perfis {#profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfis"
>abstract="Um perfil é um registro que foi direcionado para receber mensagens enviadas pelo Adobe Campaign. Nessa lista, é possível exibir os detalhes dos perfis, com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos dos perfis."

## O que é um perfil? {#what}

Um **perfil**, também conhecido como &quot;destinatário&quot; no console do cliente, representa um registro armazenado no banco de dados do Campaign, servindo como um componente chave para [criar públicos-alvo](create-audience.md) para entregas e [adicionar dados de personalização](../personalization/personalize.md) ao seu conteúdo. O Adobe Campaign permite gerenciar perfis com facilidade, desde a criação de novas entradas até o acesso a uma visualização abrangente de todos os atributos e assinaturas de serviços dos perfis, tudo isso por meio da interface do usuário na Web do Campaign.

Além disso, os **[!UICONTROL perfis de teste]**, identificados como &quot;perfis iniciais&quot; no console do cliente, permitem direcionar recipients adicionais que não correspondem aos critérios de direcionamento de uma determinada entrega. Esses perfis contêm informações de contato fictícias ou informações de contato controladas pelo remetente. Os perfis de teste são recipients de prova: eles são usados para testar suas mensagens enviando provas. [Saiba como trabalhar com perfis de teste](test-profiles.md)

Perfis e perfis de teste podem ser usados para testar seus deliveries antes que eles atinjam o público-alvo desejado. Ao fazer isso, você pode pré-visualizar o conteúdo e a personalização da mensagem, enviar provas de teste e validação, avaliar a renderização de email em várias plataformas e dispositivos e testar suas landing pages. [Saiba como visualizar e testar entregas](../preview-test/preview-test.md)

➡️ [Conheça este recurso no vídeo](#video)

## Acessar a lista de perfis {#access}

Os perfis podem ser acessados e editados na Adobe Campaign Web a partir da entrada **[!UICONTROL Gerenciamento de clientes]** > **Perfis** no painel de navegação esquerdo. Você também pode acessá-las no modo de exibição **[!UICONTROL Explorer]**, no nó **[!UICONTROL Perfis e Destinos]** > **[!UICONTROL Destinatários]**. Ali é possível navegar, criar e gerenciar pastas ou subpastas, bem como verificar permissões associadas. [Saiba como criar pastas](../get-started/permissions.md#folders)

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de perfis armazenados no banco de dados. [Saiba mais sobre permissões](../get-started/permissions.md).

Você pode filtrar a lista **[!UICONTROL Perfis]** usando o campo de pesquisa ou os filtros disponíveis no botão **Mostrar filtros**. Você pode restringir os resultados a uma [pasta](../get-started/permissions.md#folders) específica usando a lista suspensa ou adicionar regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable="yes"}

Para acessar os detalhes de um perfil, clique no nome na lista. Uma visualização detalhada do perfil é aberta, permitindo explorar seus atributos e os serviços aos quais ele se inscreveu. [Saiba como explorar os detalhes dos perfis](create-profile.md)

Para excluir um perfil, selecione a opção correspondente no menu **[!UICONTROL Mais ações]**.

## Vídeo tutorial {#video}

Saiba como acessar, gerenciar e explorar perfis usando a interface da Web do Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
