---
title: Trabalhar com destinatários e públicos-alvo
description: Saiba como trabalhar com recipients do Campaign Web
badge: label="Beta"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 25%

---

# Trabalhar com destinatários e públicos-alvo {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="360 visualização dos seus recipients"
>abstract="Crie novos recipients e monitore-os com ferramentas e relatórios avançados. Acesse os atributos, as interações e os logs do recipient. Use as opções de filtro para navegar na lista de destinatários, editar e atualizar seus perfis."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Consulte as notas de versão"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Perfis"
>abstract="Um perfil é um indivíduo selecionado para receber mensagens enviadas pelo Adobe Campaign. No Adobe Campaign, os recipients são os perfis padrão selecionados para envio de entregas (emails, SMS). Nessa lista, é possível exibir o perfil do recipient com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos do recipient."

Um recipient é um perfil selecionado para receber mensagens enviadas pelo Adobe Campaign. No Adobe Campaign, os recipients são os perfis padrão direcionados para envio de entregas (emails, SMS etc.). Os dados do recipient armazenados no banco de dados permitem criar públicos-alvo que receberão qualquer entrega e adicionar dados de personalização ao conteúdo de entrega. Outros tipos de perfis são armazenados no banco de dados. Eles foram projetados para diferentes usos: por exemplo, perfis iniciais são feitos para testar suas entregas antes que elas sejam enviadas ao público final.

Os recipients só podem ser adicionados do console do cliente do Campaign. No entanto, elas estão visíveis na Web do Campaign, no **Destinatários** entrada do painel de navegação esquerdo. Também é possível editar os atributos do recipient nessa tela.

Para editar os dados do destinatário, clique nos três pontos ao lado do respectivo nome e escolha **Editar...**.

![Editar um perfil de destinatário](assets/recipient-edit.png)

É possível atualizar um conjunto limitado de atributos, que são: nome, sobrenome, email e número de telefone.

![Atualizar um perfil de destinatário](assets/recipient-update.png)

>[!NOTE]
>
>Este formulário de edição de perfil limitado é fornecido apenas para testes de programas Beta. Ele será aprimorado na próxima versão. Ele permite que o usuário adicione rapidamente um endereço de email e um número de telefone a qualquer perfil para que possa testar os canais de email e SMS e receber as mensagens enviadas.

É possível filtrar os destinatários usando o campo de pesquisa, da variável **Mostrar filtros** botão.

Você também pode acessar recipients do **Explorer** exibir, procurar e criar pastas e subpastas e verificar as permissões associadas.

![Lista de destinatários na exibição do Explorer](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de recipients armazenados no banco de dados. Saiba mais sobre permissões [nesta seção](../get-started/permissions.md).

Além disso, é possível gerenciar a subscrição e unsubscription de recipients para serviços como boletins informativos. Saiba como trabalhar com serviços de assinatura no [esta página](manage-services.md)

Você pode criar workflows para desduplicar, enriquecer, combinar perfis e criar públicos. Saiba mais [nesta seção](../workflows/gs-workflows.md).
