---
title: Introdução a perfis
description: Saiba como monitorar e gerenciar perfis na Web do Campaign.
exl-id: 0b28741a-28f6-4f46-8c4c-820c5036aeda
source-git-commit: 980c19561c9f82a22a59b626d95d72981781af54
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 13%

---

# Introdução a perfis {#profiles}


<!--additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new" text="See release notes"-->

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfis"
>abstract="Um perfil é um registro que foi direcionado para receber mensagens enviadas pelo Adobe Campaign. Nessa lista, é possível exibir os detalhes dos perfis, com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos dos perfis."

## O que é um perfil? {#what}

A **perfil**, também conhecido como &quot;recipient&quot; no console do cliente, representa um registro armazenado no banco de dados do Campaign, servindo como um componente principal para [criar públicos](create-audience.md) para deliveries e [adicionar personalização](../personalization/personalize.md) dados ao seu conteúdo. O Adobe Campaign permite gerenciar perfis com facilidade, desde a criação de novas entradas até o acesso a uma visualização abrangente de todos os atributos e assinaturas de serviços dos perfis, tudo isso por meio da interface do usuário na Web do Campaign.

Além disso, **[!UICONTROL perfis de teste]**, identificados como &quot;perfis iniciais&quot; no console do cliente, permitem direcionar recipients adicionais que não correspondem aos critérios de direcionamento de um determinado delivery. Esses perfis contêm informações de contato fictícias ou informações de contato controladas pelo remetente. Os perfis de teste são recipients de prova: eles são usados para testar suas mensagens enviando provas. [Saiba como trabalhar com perfis de teste](test-profiles.md)

Perfis e perfis de teste podem ser usados para testar seus deliveries antes que eles atinjam o público-alvo desejado. Ao fazer isso, você pode pré-visualizar o conteúdo e a personalização da mensagem, enviar provas de teste e validação, avaliar a renderização de email em várias plataformas e dispositivos e testar suas landing pages. [Saiba como visualizar e testar deliveries](../preview-test/preview-test.md)

➡️ [Descubra este recurso no vídeo](#video)

## Acessar a lista de perfis {#access}

Os perfis podem ser acessados e editados na Adobe Campaign Web a partir do **[!UICONTROL Gerenciamento de clientes]** > **Perfis** no painel de navegação esquerdo. Você também pode acessá-las no **[!UICONTROL Explorer]** exibir, no **[!UICONTROL Perfis e destinos]** > **[!UICONTROL Destinatários]** nó. Ali é possível navegar, criar e gerenciar pastas ou subpastas, bem como verificar permissões associadas. [Saiba como criar pastas](../get-started/permissions.md#folders)

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de perfis armazenados no banco de dados. [Saiba mais sobre permissões](../get-started/permissions.md).

É possível filtrar a variável **[!UICONTROL Perfis]** usando o campo de pesquisa ou os filtros disponíveis no **Mostrar filtros** botão. É possível restringir os resultados a um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/profiles-list-filters.png){zoomable=&quot;yes&quot;}

Para acessar os detalhes de um perfil, clique no nome na lista. Uma visualização detalhada do perfil é aberta, permitindo explorar seus atributos e os serviços aos quais ele se inscreveu. [Saiba como explorar os detalhes dos perfis](create-profile.md)

Para excluir um perfil, selecione a opção correspondente na **[!UICONTROL Mais ações]** menu.

## Vídeo tutorial {#video}

Saiba como acessar, gerenciar e explorar perfis usando a interface da Web do Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3427293?quality=12)
