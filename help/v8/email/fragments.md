---
audience: end-user
title: Criar fragmentos de conteúdo
description: Saiba como criar com fragmentos de conteúdo
hide: true
hidefromtoc: true
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 23%

---

# Criar fragmentos de conteúdo {#fragments}


>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Definir seus próprios fragmentos"
>abstract="Um fragmento é um componente reutilizável que pode ser referenciado em um ou mais emails em campanhas. Este recurso é usado para pré-criar vários blocos de conteúdo personalizados, que podem ser usados por usuários de marketing para montar rapidamente os conteúdos de email em um processo de design aprimorado."

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Salvar fragmentos"
>abstract="Salvar fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Definir seus próprios fragmentos"
>abstract="Um fragmento é um componente reutilizável que pode ser referenciado em um ou mais emails em campanhas."

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Propriedades dos fragmentos"
>abstract="Propriedades dos fragmentos"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Tipo de fragmento"
>abstract="Selecione o tipo de fragmento. Por enquanto, somente fragmentos visuais para emails estão disponíveis."

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Definir seus próprios fragmentos"
>abstract="Um fragmento é um componente reutilizável que pode ser referenciado em um ou mais emails em campanhas. Você também pode usar fragmentos em seus modelos de email. Por enquanto, somente fragmentos visuais estão disponíveis."

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Detalhes de fragmentos"
>abstract="Detalhes de fragmentos"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="Definir seus próprios fragmentos"
>abstract="Um fragmento é um componente reutilizável que pode ser referenciado em um ou mais emails em campanhas."

Um fragmento é um componente reutilizável que pode ser referenciado em um ou mais emails em campanhas. Ao modificar um fragmento, todo o conteúdo que o usa é atualizado.

Essa funcionalidade permite pré-criar vários blocos de conteúdo personalizados que podem ser usados por usuários de marketing para reunir rapidamente o conteúdo de email em um processo de design aprimorado.

![](assets/fragments.gif)


Para aproveitar ao máximo os fragmentos:

* Crie seus próprios fragmentos visuais, conforme detalhado abaixo.
* Use-os quantas vezes forem necessárias em seu conteúdo, por meio do Designer de email. Consulte [Adicionar fragmentos visuais aos seus emails](../email/use-visual-fragments.md).

## Criar um fragmento visual {#create-fragments}

Há duas maneiras de criar fragmentos:

* Crie um fragmento do zero, usando o menu dedicado **[!UICONTROL Fragmentos]**. [Saiba como](#create-from-scratch)

* Ao criar o conteúdo, salve uma parte do conteúdo como fragmento. [Saiba como](#save-as-fragment)

Depois de salvo, o fragmento fica disponível para uso em um email ou modelo de email. Seja criado do zero ou a partir de um conteúdo existente, agora é possível usar esse fragmento ao criar qualquer conteúdo no Campaign. Consulte [Adicionar fragmentos visuais](../email/use-visual-fragments.md).

### Criar um fragmento do zero {#create-from-scratch}

Para criar um fragmento do zero, siga as etapas abaixo.

1. [Acesse a lista de fragmentos](#access-manage-fragments) por meio do menu esquerdo **[!UICONTROL Gerenciamento de Conteúdo]** > **[!UICONTROL Fragmentos]**.

   ![](assets/fragments-list.png)

1. Selecione **[!UICONTROL Criar fragmento]**.

1. Insira o rótulo do fragmento.

   ![](assets/fragment-create.png)

1. Se necessário, você pode definir opções adicionais, como o nome interno do fragmento, sua pasta e uma descrição.

   >[!NOTE]
   >
   >Por enquanto, só é possível criar fragmentos visuais.

1. Clique no botão **Criar** para configurar o conteúdo do fragmento.

1. O [Designer de email](../email/get-started-email-designer.md) é exibido. Edite seu conteúdo conforme necessário, da mesma forma que faria para qualquer email dentro de uma campanha. Você pode adicionar imagens, links, campos de personalização e conteúdo dinâmico.

   ![](assets/fragment-designer.png)

1. Quando o fragmento estiver pronto, clique em **[!UICONTROL Salvar e fechar]**. Foi adicionado à [lista de fragmentos](#access-manage-fragments).

Este fragmento agora está pronto para ser usado ao criar qualquer [email](../email/get-started-email-designer.md) ou [modelo de conteúdo](use-email-templates.md) no Campaign. [Saiba como](../email/use-visual-fragments.md)


### Salvar um conteúdo como fragmento {#save-as-fragment}

Qualquer conteúdo de email pode ser salvo como fragmento para futura reutilização. Ao criar uma entrega de [modelo de conteúdo](use-email-templates.md) ou de [email](../email/get-started-email-designer.md), você pode salvar uma parte do seu conteúdo como fragmento visual. Para fazer isso, siga as etapas abaixo:

1. No [Designer de Email](../email/get-started-email-designer.md), clique no botão **Mais** na parte superior direita da tela.

1. Selecione **[!UICONTROL Salvar como fragmento]** no menu suspenso.

   ![](assets/fragment-save-as.png)

1. A tela **[!UICONTROL Salvar como fragmento]** é exibida. Lá, selecione os elementos que deseja incluir no fragmento, incluindo campos de personalização e conteúdo dinâmico.

   >[!CAUTION]
   >
   >Você só pode selecionar seções adjacentes entre si. Não é possível selecionar uma estrutura vazia ou outro fragmento.

   ![](assets/fragment-save-as-screen.png)

1. Clique em **[!UICONTROL Criar]**. Preencha o nome do fragmento e salve-o.

   ![](assets/fragment-save-confirm.png)

   Este conteúdo agora é um fragmento independente, adicionado à [lista de fragmentos](#manage-fragments) e acessível pelo menu dedicado. Agora você pode usar este fragmento ao criar qualquer [email](../email/get-started-email-designer.md) ou [modelo de conteúdo](use-email-templates.md) no Campaign. [Saiba como](../email/use-visual-fragments.md)

>[!NOTE]
>
>Qualquer alteração nesse novo fragmento não é propagada para o email ou modelo de onde vem. Da mesma forma, quando o conteúdo original é editado nesse email ou modelo, o novo fragmento não é modificado.

## Gerenciar os fragmentos {#manage-fragments}

É possível editar, atualizar, duplicar ou excluir um fragmento da lista de fragmentos.

### Editar e atualizar um fragmento {#edit-fragments}

Para editar um fragmento, siga as etapas abaixo.

1. Clique no nome do fragmento para editar na lista **[!UICONTROL Fragmentos]**.
1. Clique no botão **Editar conteúdo** para abrir o conteúdo deste fragmento.

   ![](assets/fragment-edit-content.png)

1. Faça as alterações necessárias e salve as modificações.

>[!CAUTION]
>
>Qualquer alteração em um fragmento é propagada para os deliveries de email ou templates que o utilizam.


### Excluir um fragmento {#delete-fragments}

Para excluir um fragmento, siga estas etapas:

1. Navegue até a lista de fragmentos e clique no botão **[!UICONTROL Mais ações]** ao lado do fragmento a ser excluído.
1. Clique em **Excluir** e confirme.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Ao excluir um fragmento de conteúdo, os deliveries de email e os modelos que o utilizam são atualizados: o fragmento é removido do conteúdo do email, mas ainda é referenciado. Para manter o conteúdo do fragmento nessas entregas e modelos, você deve interromper a herança antes de excluir o fragmento, [conforme detalhado nesta seção](use-visual-fragments.md#break-inheritance).
>

### Duplicação de um fragmento {#duplicate-fragments}

É possível duplicar facilmente um fragmento para criar um novo. Para duplicar um fragmento existente, siga estas etapas:

1. Navegue até a lista de fragmentos e clique no botão **[!UICONTROL Mais ações]** ao lado do fragmento a ser excluído.
1. Clique em **Duplicar** e confirme.
1. Insira o rótulo do novo fragmento e salve as alterações.

   O fragmento é adicionado à lista de fragmentos. Você pode editá-la e configurá-la conforme necessário.
