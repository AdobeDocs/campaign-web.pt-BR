---
audience: end-user
title: Adicionar fragmentos visuais aos emails
description: Saiba como adicionar fragmentos visuais aos emails
badge: label="Disponibilidade limitada"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: bb7e014a381801566b95839581d0b4d13278524d
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 14%

---

# Adicionar fragmentos visuais aos emails {#use-visual-fragments}

>[!AVAILABILITY]
>
>Esse recurso exige uma atualização do Campaign v8.6.4. Saiba mais nas [notas de versão do console do Campaign v8 Client](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/releases/release-notes).

Você pode usar um fragmento visual em uma [entrega de email](../email/get-started-email-designer.md) ou em um [modelo de conteúdo](../email/use-email-templates.md). As etapas são detalhadas abaixo.

![](assets/do-not-localize/fragments.gif)

>[!NOTE]
>
>Saiba como criar e gerenciar fragmentos de conteúdo no [esta seção](fragments.md).

## Usar um fragmento visual {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Opções de fragmentos"
>abstract="Esse painel fornece opções relacionadas ao fragmento selecionado. Ele permite que você escolha os dispositivos nos quais deseja que o fragmento seja exibido e abra o conteúdo deste fragmento. Use a guia **[!UICONTROL Estilos]** para personalizar ainda mais o fragmento. Também é possível quebrar a herança com o fragmento visual original."

<!-- pas vu dans l'UI-->

Para inserir um fragmento visual em um conteúdo de email, siga as etapas abaixo:

1. Abra qualquer conteúdo de email ou modelo usando a [Designer de email](../email/get-started-email-designer.md).

1. Selecione o ícone **[!UICONTROL Fragmentos]** no painel esquerdo.

   ![](assets/fragments-in-designer.png)

1. A lista de todos os fragmentos visuais criados na sandbox atual é exibida. Você pode:

   * Procure um fragmento específico começando digitando seu rótulo.
   * Classifique os fragmentos em ordem crescente ou decrescente.
   * Altere a forma como os fragmentos são exibidos (cartões ou exibição em lista).

   >[!NOTE]
   >
   >Os fragmentos são classificados por data de criação: os fragmentos adicionados recentemente são mostrados primeiro na lista.

   Se alguns fragmentos visuais foram modificados ou adicionados enquanto você está editando seu conteúdo, clique no ícone **Atualizar** para atualizar a lista com as alterações mais recentes.

1. Arraste e solte qualquer fragmento visual da lista na área em que deseja inseri-lo. Como qualquer outro componente, é possível mover o fragmento no conteúdo.

1. Selecione o fragmento para exibir suas opções no painel direito.

   ![](assets/fragment-right-pane.png)

   Na guia **[!UICONTROL Configurações]**, é possível:

   * Escolha os dispositivos nos quais deseja que o fragmento seja exibido.
   * Clique no botão **Editar conteúdo** para abrir o conteúdo deste fragmento. [Saiba mais](../content/fragments.md#edit-fragments)

     Você pode personalizar ainda mais o fragmento usando a guia **[!UICONTROL Estilos]**.

1. Se necessário, é possível quebrar a herança com o fragmento visual original. [Saiba mais](#break-inheritance)

   Você também pode excluir o fragmento do seu conteúdo ou duplicá-lo. Essas ações podem ser executadas diretamente no menu contextual exibido na parte superior do fragmento.

1. Adicione quantos fragmentos visuais desejar e **[!UICONTROL Salve]** suas alterações.

### Fragmento visual no modo somente leitura {#fragment-readonly}

Os direitos de acesso podem ser aplicados a fragmentos visuais.

Se você não tiver permissões de edição para um fragmento visual específico, o modelo de conteúdo será exibido no **modo somente leitura**. Nesse caso, o botão **[!UICONTROL Editar conteúdo]** é substituído pelo botão **[!UICONTROL Exibir conteúdo]**, permitindo que você visualize o fragmento sem fazer alterações.

![](assets/fragment-readonly.png){zoomable="yes"}

Como mostrado abaixo, todos os ícones de recursos são desativados, limitando a interação somente para visualização.

![](assets/fragment-readonly-view.png){zoomable="yes"}

## Interromper herança {#break-inheritance}

Ao editar um fragmento visual, as alterações são sincronizadas. Eles são propagados automaticamente para todas as entregas de email e modelos de conteúdo que contêm esse fragmento.

Quando adicionados a um email ou modelo de conteúdo, os fragmentos são sincronizados por padrão.

No entanto, é possível quebrar a herança do fragmento original. Nesse caso, o conteúdo do fragmento é copiado para o design atual e as alterações não são mais sincronizadas.

Para interromper a herança, siga as etapas abaixo:

1. Selecione o fragmento visual.

1. Clique no ícone de desbloqueio na barra de ferramentas contextual.

   ![](assets/fragment-break-inheritance.png)

1. Esse fragmento se torna um elemento independente que não está mais vinculado ao fragmento original. Edite-o como qualquer outro componente de conteúdo em seu conteúdo. [Saiba mais](../email/content-components.md)
