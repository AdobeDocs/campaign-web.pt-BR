---
audience: end-user
title: Adicionar fragmentos visuais aos emails
description: Saiba como adicionar fragmentos visuais aos emails
hide: true
source-git-commit: a882087bc608ea4029e53ed38ecf699e127be065
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 4%

---

# Adicionar fragmentos visuais aos emails {#use-visual-fragments}

É possível usar um fragmento visual em uma [delivery de email](get-started-email-designer.md)ou em um [template de conteúdo](use-email-templates.md). As etapas são detalhadas abaixo.


>[!NOTE]
>
>Saiba como criar e gerenciar fragmentos no [nesta seção](fragments.md).


## Usar um fragmento {#use-fragment}

Para inserir um fragmento em um conteúdo de email, siga as etapas abaixo:

1. Abra qualquer conteúdo de email ou modelo usando o [Email Designer](get-started-email-designer.md).

1. Selecione o **[!UICONTROL Fragmentos]** no painel esquerdo.

   ![](assets/fragments-in-designer.png)

1. A lista de todos os fragmentos visuais criados na sandbox atual é exibida. Você pode:

   * Procure um fragmento específico começando digitando seu rótulo.
   * Classifique os fragmentos em ordem crescente ou decrescente.
   * Altere a forma como os fragmentos são exibidos (cartões ou exibição em lista).

   >[!NOTE]
   >
   >Os fragmentos são classificados por data de criação: os fragmentos visuais adicionados recentemente são mostrados primeiro na lista.

   Se alguns fragmentos foram modificados ou adicionados enquanto você está editando o conteúdo, clique no link **Atualizar** ícone para atualizar a lista com as alterações mais recentes.

1. Arraste e solte qualquer fragmento da lista na área em que deseja inseri-lo. Como qualquer outro componente, é possível mover o fragmento no conteúdo.

1. Selecione o fragmento para exibir suas opções no painel direito.

   ![](assets/fragment-right-pane.png)

   No **[!UICONTROL Configurações]** é possível:

   * Escolha os dispositivos nos quais deseja que o fragmento seja exibido.
   * Abra o fragmento em uma nova guia para editá-lo, se necessário. [Saiba mais](../email/fragments.md#edit-fragments)

   É possível personalizar ainda mais o fragmento usando o **[!UICONTROL Estilos]** guia.

1. Se necessário, é possível quebrar a herança com o fragmento original. [Saiba mais](#break-inheritance)
Você também pode excluir o fragmento do seu conteúdo ou duplicá-lo. Essas ações podem ser executadas diretamente no menu contextual exibido na parte superior do fragmento.

1. Adicione quantos fragmentos desejar e **[!UICONTROL Salvar]** suas alterações.

## Interromper herança {#break-inheritance}

Ao editar um fragmento visual, as alterações são sincronizadas. Eles são propagados automaticamente para todas as entregas de email e modelos de conteúdo que contêm esse fragmento.

Quando adicionados a um email ou modelo de conteúdo, os fragmentos são sincronizados por padrão.

No entanto, é possível quebrar a herança do fragmento original. Nesse caso, o conteúdo do fragmento é copiado para o design atual e as alterações não são mais sincronizadas.

Para interromper a herança, siga as etapas abaixo:

1. Selecione o fragmento.

1. Clique no ícone de desbloqueio na barra de ferramentas contextual.

   ![](assets/fragment-break-inheritance.png)

1. Esse fragmento se torna um elemento independente que não está mais vinculado ao fragmento original. Edite-o como qualquer outro componente de conteúdo em seu conteúdo. [Saiba mais](content-components.md)
