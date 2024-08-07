---
audience: end-user
title: Adicionar fragmentos visuais aos emails
description: Saiba como adicionar fragmentos visuais aos emails
badge: label="Disponibilidade limitada"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 20%

---

# Adicionar fragmentos visuais aos emails {#use-visual-fragments}

>[!AVAILABILITY]
>
>Esse recurso está na disponibilidade limitada (DL). É restrita aos clientes que estão migrando **do Adobe Campaign Standard para o Adobe Campaign v8** e não pode ser implantada em nenhum outro ambiente.

Você pode usar um fragmento visual em uma [entrega de email](../email/get-started-email-designer.md) ou em um [modelo de conteúdo](../email/use-email-templates.md). As etapas são detalhadas abaixo. [Saiba como criar e gerenciar fragmentos de conteúdo](fragments.md).

![](assets/fragments.gif)

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

## Interromper herança {#break-inheritance}

Ao editar um fragmento visual, as alterações são sincronizadas. Eles são propagados automaticamente para todas as entregas de email e modelos de conteúdo que contêm esse fragmento.

Quando adicionados a um email ou modelo de conteúdo, os fragmentos são sincronizados por padrão.

No entanto, é possível quebrar a herança do fragmento original. Nesse caso, o conteúdo do fragmento é copiado para o design atual e as alterações não são mais sincronizadas.

Para interromper a herança, siga as etapas abaixo:

1. Selecione o fragmento visual.

1. Clique no ícone de desbloqueio na barra de ferramentas contextual.

   ![](assets/fragment-break-inheritance.png)

1. Esse fragmento se torna um elemento independente que não está mais vinculado ao fragmento original. Edite-o como qualquer outro componente de conteúdo em seu conteúdo. [Saiba mais](../email/content-components.md)
