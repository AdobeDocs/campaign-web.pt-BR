---
audience: end-user
title: Adicionar fragmentos visuais a emails
description: Saiba como adicionar fragmentos visuais aos emails
badge: label="Disponibilidade limitada"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 13%

---

# Adicionar fragmentos visuais a emails {#use-visual-fragments}

>[!AVAILABILITY]
>
>Esse recurso exige uma atualização do Campaign v8.6.4. Saiba mais nas [notas de versão do console do Campaign v8 Client](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/releases/release-notes).

Na interface da Web do Campaign, os **fragmentos visuais** são blocos visuais predefinidos que podem ser reutilizados em várias [entregas de email](../email/get-started-email-designer.md) ou em [modelos de conteúdo](../content/use-email-templates.md). Saiba como criar e gerenciar fragmentos de conteúdo no [esta seção](fragments.md).

![Representação visual de fragmentos visuais em uso](assets/do-not-localize/fragments.gif)

## Usar um fragmento visual {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Opções de fragmentos"
>abstract="Esse painel fornece opções relacionadas ao fragmento selecionado. Ele permite que você escolha os dispositivos nos quais deseja que o fragmento seja exibido e abra o conteúdo deste fragmento. Use a guia **[!UICONTROL Estilos]** para personalizar ainda mais o fragmento. Também é possível quebrar a herança com o fragmento visual original."

<!-- pas vu dans l'UI-->

Para inserir um fragmento visual no conteúdo de email, siga estas etapas:

1. Abra qualquer conteúdo de email ou modelo usando a [Designer de email](../email/get-started-email-designer.md).

1. Selecione o ícone **[!UICONTROL Fragmentos]** no painel esquerdo.

   ![Captura de tela mostrando o ícone Fragmentos na interface do Designer de email](assets/fragments-in-designer.png)

1. A lista de todos os fragmentos visuais criados na sandbox atual é exibida. Você pode:

   * Procure um fragmento específico digitando seu rótulo.
   * Classifique os fragmentos em ordem crescente ou decrescente.
   * Altere a forma como os fragmentos são exibidos (cartões ou exibição em lista).

   >[!NOTE]
   >
   >Os fragmentos são classificados por data de criação. Fragmentos adicionados recentemente aparecem primeiro na lista.

   Se fragmentos visuais forem modificados ou adicionados enquanto você estiver editando seu conteúdo, clique no ícone **Atualizar** para atualizar a lista com as alterações mais recentes.

1. Arraste e solte qualquer fragmento visual da lista na área em que deseja inseri-lo. Como qualquer outro componente, é possível mover o fragmento no conteúdo.

1. Selecione o fragmento para exibir suas opções no painel direito.

   ![Captura de tela mostrando as opções do fragmento no painel direito](assets/fragment-right-pane.png)

   Na guia **[!UICONTROL Configurações]**, é possível:

   * Escolha os dispositivos nos quais deseja que o fragmento seja exibido.
   * Clique no botão **Editar conteúdo** para abrir o conteúdo deste fragmento. [Saiba mais](../content/fragments.md#edit-fragments)

     Você pode personalizar ainda mais o fragmento usando a guia **[!UICONTROL Estilos]**.

1. Se necessário, quebre a herança com o fragmento visual original. [Saiba mais](#break-inheritance)

   Você também pode excluir o fragmento do seu conteúdo ou duplicá-lo. Execute essas ações diretamente no menu contextual exibido na parte superior do fragmento.

1. Adicione quantos fragmentos visuais forem necessários e **[!UICONTROL Salve]** suas alterações.

### Fragmento visual no modo somente leitura {#fragment-readonly}

Os direitos de acesso podem se aplicar a fragmentos visuais.

Se a edição de permissão não for concedida para um fragmento visual específico, o modelo de conteúdo será exibido no **modo somente leitura**. Nesse caso, o botão **[!UICONTROL Editar conteúdo]** é substituído pelo botão **[!UICONTROL Exibir conteúdo]**, permitindo que você visualize o fragmento sem fazer alterações.

![Captura de tela mostrando um fragmento visual no modo somente leitura](assets/fragment-readonly.png){zoomable="yes"}

Como mostrado abaixo, todos os ícones de recursos são desativados, limitando a interação somente para visualização.

![Captura de tela mostrando ícones de recursos desativados no modo somente leitura](assets/fragment-readonly-view.png){zoomable="yes"}

## Interromper herança {#break-inheritance}

Ao editar um fragmento visual, as alterações são sincronizadas e propagadas automaticamente para todos os deliveries de email e modelos de conteúdo que contêm esse fragmento.

Por padrão, os fragmentos são sincronizados quando adicionados a um email ou modelo de conteúdo.

No entanto, é possível quebrar a herança do fragmento original. Nesse caso, o conteúdo do fragmento é copiado para o design atual e as alterações não são mais sincronizadas.

Para interromper a herança, siga estas etapas:

1. Selecione o fragmento visual.

1. Clique no ícone de desbloqueio na barra de ferramentas contextual.

   ![Captura de tela mostrando o ícone de desbloqueio para interromper a herança](assets/fragment-break-inheritance.png)

1. O fragmento se torna um elemento independente que não está mais vinculado ao fragmento original. Edite-o como qualquer outro componente de conteúdo em seu conteúdo. [Saiba mais](../email/content-components.md)