---
title: Trabalhar com recipients e públicos
description: Saiba como trabalhar com recipients do Campaign Web
badge: label="Beta"
source-git-commit: 2b4928f6e5897d04889f822921e355a7c1360c80
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 27%

---


# Trabalhar com recipients e públicos {#about-recipients}

## O que são recipients? {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Recipients"
>abstract="Um recipient é um perfil selecionado para receber mensagens enviadas pelo Adobe Campaign. No Adobe Campaign, os recipients são os perfis padrão direcionados para envio de deliveries (emails, SMS). Nessa lista, é possível exibir o perfil do recipient com base nas suas permissões. Use as opções de filtro para navegar nesta lista. É possível editar e atualizar um pequeno conjunto de atributos do recipient."

Um recipient é um perfil selecionado para receber mensagens enviadas pelo Adobe Campaign. No Adobe Campaign, os recipients são os perfis padrão direcionados para envio de deliveries (emails, SMS etc.). Os dados do recipient armazenados no banco de dados permitem criar públicos-alvo que receberão qualquer entrega e adicionar dados de personalização ao conteúdo de entrega. Outros tipos de perfis são armazenados no banco de dados. Eles foram projetados para diferentes usos: por exemplo, perfis iniciais são feitos para testar suas entregas antes que elas sejam enviadas ao público final.

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
>Dependendo das suas permissões, talvez você não tenha acesso à lista completa de recipients armazenados no banco de dados. Saiba mais sobre permissões no [nesta seção](../get-started/permissions.md).

Além disso, é possível gerenciar a subscrição e unsubscription de recipients para serviços como boletins informativos. [Saiba como trabalhar com serviços de assinatura](manage-services.md)

Você pode criar workflows para desduplicar, enriquecer, combinar perfis e criar públicos. Saiba mais [nesta seção](../workflows/gs-workflows.md).

## O que são públicos-alvo? {#audiences}

O público-alvo é o principal foco da sua entrega: os destinatários que receberão as mensagens O tipo de público-alvo depende do target mapping definido no modelo de entrega. [Saiba o que é um modelo de entrega](../msg/delivery-template.md).

Para definir a população de um público-alvo, é possível:

* [Criar novos públicos](create-audience.md) do **[!UICONTROL Públicos-alvo]** menu,
* [Selecionar um público existente](add-audience.md) criado como uma lista no console do cliente,
* [Selecionar um público-alvo da Adobe Experience Platform](aep-audience.md),
* [Criar um público-alvo novo com o criador de regras definindo e combinando critérios de filtro,](segment-builder.md)
* [Usar um público-alvo de um arquivo externo](file-audience.md). Essa opção só está disponível para deliveries de email independentes e não pode ser usada em deliveries de campanha.

Ao direcionar um público-alvo, você também pode definir **grupos de controle** para evitar o envio de mensagens para uma parte do público-alvo e medir o impacto das campanhas. [Saiba como definir um grupo de controle](control-group.md)

>[!NOTE]
>
>Ao enviar mensagens no contexto de um workflow de campanha, o público-alvo é definido em um **Criar público-alvo** atividade de workflow. Nesse contexto, não é possível carregar um público-alvo de um arquivo para uma entrega de email, e o público-alvo é definido somente nessa atividade dedicada. Saiba como definir o público-alvo da sua entrega em um workflow de campanha [nesta seção](../workflows/activities/build-audience.md)

## Dimensões de direcionamento {#targeting-dimensions}

Targeting dimension, também conhecido como. target mapping, é o tipo de dados que uma operação está tratando. Ele permite definir a população direcionada: recipients, beneficiários de contrato, operadores, assinantes etc.

O targeting dimension de um workflow é definido pelo primeiro **[!UICONTROL Criar público-alvo]** e é usada em todas as outras atividades até o fim do workflow. Por exemplo, se você realizar um query nos recipients do banco de dados, a transição de saída conterá dados do tipo recipient e será transmitida para a próxima atividade.

Observe que é possível alternar o targeting dimension em um workflow usando um **[!UICONTROL Alterar dimensão]** atividade. [Saiba mais](../workflows/activities/change-dimension.md). Isso permite, por exemplo, consultar o banco de dados em uma tabela específica, como compras ou assinaturas, e alterar o targeting dimension para Recipients para enviar deliveries aos recipients correspondentes.

Por padrão, templates de delivery de email e SMS têm como target **[!UICONTROL Destinatários]**. O target dimension, portanto, usa os campos da variável **nms:recipient** tabela. Para notificações por push, a dimensão de destino padrão é **Aplicativos de assinante nms:appSubscriptionRcp**, que está vinculado à tabela de recipients.

Você também pode usar outros target mappings integrados nos workflows e deliveries listados abaixo:

| Nome | Uso para | Schema |
|---|---|---|
| Recipients | Entregar aos destinatários (tabela de destinatários integrada) | nms:recipient |
| Visitantes | Enviar delivery aos visitantes cujos perfis foram coletados por meio de referência (marketing viral), por exemplo. | mns:visitor |
| Subscrições | Enviar delivery aos recipients que assinam um serviço de informações, como um boletim informativo | nms:subscription |
| Assinaturas do visitante | Enviar delivery aos visitantes que são inscritos em um serviço de informações | nms:visitorSub |
| Operadores | Enviar delivery aos operadores do Adobe Campaign | nms:operator |
| Arquivo externo | Enviar delivery por meio de um arquivo que contenha todas as informações necessárias para o delivery | Nenhum schema vinculado, nenhum target inserido |
| Aplicativos de assinante | Enviar delivery aos recipients que assinaram um aplicativo | nms:appSubscriptionRcp |

Além disso, você pode criar um novo target mapping dependendo das suas necessidades. Isso é executado no console do cliente. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
