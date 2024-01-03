---
title: Monitorar e gerenciar perfis
description: Saiba como monitorar e gerenciar perfis na Web do Campaign.
badge: label="Disponibilidade limitada"
source-git-commit: 41c38ff3b18c28fbcb6fd07dd398600a207f53cb
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 7%

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

Perfis podem ser adicionados somente a partir do console do cliente Campaign. No entanto, elas podem ser acessadas no Adobe Campaign Web pelo **Perfis** no painel de navegação esquerdo. Você também pode acessá-las no **Explorer** exibir, onde você pode navegar, criar pastas, subpastas e verificar permissões associadas.

É possível filtrar a lista de perfis usando o campo de pesquisa ou os filtros disponíveis no **Mostrar filtros** botão.

![](assets/profiles-list.png)

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de perfis armazenados no banco de dados. Saiba mais sobre permissões [nesta seção](../get-started/permissions.md).

## Acessar e editar atributos dos perfis {#access}

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_details"
>title="Detalhes básicos"
>abstract="Esta seção oferece insights sobre os detalhes básicos do perfil. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_contactinformation"
>title="Informações de contato"
>abstract="Esta seção oferece insights sobre as informações de contato do perfil. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_address"
>title="Endereço"
>abstract="Esta seção oferece informações sobre o endereço postal do perfil e a qualidade do endereço. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_account"
>title="Detalhes da conta"
>abstract="Esta seção oferece insights sobre os detalhes da conta do perfil. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_nolongercontact"
>title="Os destinatários não contatam mais"
>abstract="Esta seção oferece informações sobre as preferências de contato do perfil. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_customfields"
>title="Campos personalizados"
>abstract="Os campos personalizados são atributos específicos adaptados às suas necessidades que foram configuradas para sua instância. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_othersfields"
>title="Outros"
>abstract="Esta seção fornece atributos incorporados adicionais. Para modificar qualquer informação, faça as alterações diretamente no respectivo campo e clique no **Salvar** localizado no canto superior direito da tela."

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_list"
>title="Lista de assinaturas dos destinatários"
>abstract="Esta guia lista todos os serviços que o perfil assinou."

Para acessar os detalhes de um perfil, clique no nome na lista de perfis.

![](assets/profiles-details.png)

Nessa tela, você pode acessar informações detalhadas sobre o perfil:

* A variável **[!UICONTROL Detalhes]** permite navegar pelos atributos incorporados e personalizados do perfil. Para editar um atributo, faça as alterações no campo desejado e clique no **[!UICONTROL Salvar]** botão.
* A variável **[!UICONTROL Assinaturas]** A guia fornece informações sobre os serviços aos quais o perfil está inscrito. [Saiba como trabalhar com serviços de assinatura](manage-services.md)
* A variável **[!UICONTROL Logs]** O botão, localizado no canto superior direito da tela, permite visualizar um histórico das interações do perfil por meio de envios, exclusões e logs de rastreamento, bem como as propostas apresentadas ao perfil.
