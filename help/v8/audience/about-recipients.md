---
title: Monitorar e gerenciar perfis
description: Saiba como monitorar e gerenciar perfis na Web do Campaign.
source-git-commit: 543f8b2de616f63f747fbb622053f5edd492d90d
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 9%

---

# Monitorar e gerenciar perfis {#profiles}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Visualização 360 dos seus perfis"
>abstract="Crie novos perfis e monitore-os com ferramentas e relatórios avançados. Acesse os atributos, as interações e os logs dos perfis. Use as opções de filtro para navegar na lista de perfis, editar e atualizar seus perfis."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulte as notas de versão"

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfis"
>abstract="Um perfil é um indivíduo selecionado para receber mensagens enviadas pelo Adobe Campaign. Nessa lista, é possível visualizar os detalhes dos perfis com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos de seus perfis."

## Introdução a perfis {#gs}

Um perfil na Adobe Campaign Web é um indivíduo armazenado no banco de dados, atuando como um componente chave para criar públicos-alvo para deliveries e adicionar dados de personalização ao seu conteúdo. Vários tipos de perfis são armazenados no banco de dados, como Perfis de teste, que são projetados para testar seus deliveries antes que sejam enviados ao público final. [Saiba como trabalhar com perfis de teste](test-profiles.md)

Os perfis podem ser acessados no **Perfis** no painel de navegação esquerdo. Você também pode acessá-las no **Explorer** exibir, onde você pode navegar, criar pastas, subpastas e verificar permissões associadas.

É possível filtrar a lista de perfis usando o campo de pesquisa ou os filtros disponíveis no **Mostrar filtros** botão.

![](assets/profiles-list.png)

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de perfis armazenados no banco de dados. Saiba mais sobre permissões [nesta seção](../get-started/permissions.md).

## Acessar e editar atributos dos perfis {#access}

Para acessar os detalhes de um perfil, clique no nome na lista de perfis.

![](assets/profiles-details.png)

Nessa tela, você pode acessar informações detalhadas sobre o perfil:

* A variável **[!UICONTROL Detalhes]** permite navegar pelos atributos do perfil. Para editar um atributo, faça as alterações no campo desejado e clique no **[!UICONTROL Salvar]** botão.
* A variável **[!UICONTROL Assinaturas]** A guia fornece informações sobre os serviços aos quais o perfil está inscrito. [Saiba como trabalhar com serviços de assinatura](manage-services.md)
* A variável **[!UICONTROL Logs]** O botão, localizado no canto superior direito da tela, permite visualizar um histórico das interações do perfil por meio de envios, exclusões e logs de rastreamento, bem como as propostas apresentadas ao perfil.
