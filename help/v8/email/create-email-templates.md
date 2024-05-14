---
audience: end-user
product: campaign
title: Trabalho com modelos de conteúdo
description: Saiba como criar modelos para reutilizar conteúdo em emails do Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 19%

---

# Trabalho com modelos de conteúdo {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Modelos de conteúdo"
>abstract="Para acelerar e melhorar o processo de criação, é possível criar modelos de email independentes para reutilizar facilmente o conteúdo personalizado no Adobe Campaign. Esses modelos de conteúdo podem ser criados do zero, com base em modelos integrados ou personalizados, criados a partir de um conteúdo já existente ou importados no editor de modelo de conteúdo."

Para um processo de design acelerado e aprimorado, é possível criar modelos independentes para reutilizar facilmente o conteúdo personalizado em [!DNL Adobe Campaign]. Esses modelos de conteúdo podem ser criados do zero, com base em modelos integrados ou personalizados, criados a partir de um conteúdo já existente ou importados no editor de modelo de conteúdo.

Essa funcionalidade permite que os usuários orientados a conteúdo trabalhem em modelos independentes para que os usuários de marketing possam reutilizar e adaptá-los em suas próprias campanhas de email.

>[!NOTE]
>
>Somente no momento **email** modelos de conteúdo são compatíveis.

## Acessar modelos de conteúdo {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Editar o conteúdo do modelo"
>abstract="Clique em **Editar conteúdo** para atualizar o conteúdo com o Designer de email."

Para acessar a lista de templates de conteúdo, navegue até a **[!UICONTROL Gestão de conteúdo]** > **[!UICONTROL Modelos de conteúdo]** no painel esquerdo.

![](assets/content-template-list.png){zoomable=&quot;yes&quot;}

Esse painel mostra todos os modelos de conteúdo disponíveis como uma lista. É possível filtrar em um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png){zoomable=&quot;yes&quot;}

Na lista, você pode editar, duplicar ou excluir modelos de conteúdo existentes. Use o botão na seção superior para criar um template de conteúdo.


## Criar modelos de conteúdo {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Design do modelo de conteúdo"
>abstract="Projete seu modelo de conteúdo de email."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Seleção do modelo de conteúdo"
>abstract="Selecione seu modelo de conteúdo de email."

Os modelos de conteúdo podem ser criados por [salvar um email existente como modelo](#save-as-template)ou da lista de modelos de email, por meio da **Criar modelo de conteúdo** botão, [conforme detalhado abaixo](#create-template-from-scratch).

Depois de salvo, agora você pode usar este modelo ao criar qualquer [email](../email/create-email.md) no prazo de [!DNL Adobe Campaign]. [Saiba como](use-email-templates.md)

>[!NOTE]
>
>* As alterações feitas em modelos de conteúdo não são propagadas para emails.
>
>* Da mesma forma, quando os modelos são usados em um email, as edições feitas no conteúdo do email não afetam o modelo de conteúdo usado anteriormente.

### Criar um novo modelo de conteúdo {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Definir as propriedades do modelo"
>abstract="Defina as propriedades do modelo de conteúdo de email para recuperá-las facilmente quando necessário."

Para criar um novo modelo de conteúdo no painel de modelos de conteúdo, siga estas etapas:

1. Navegue até a lista de modelos de conteúdo na **[!UICONTROL Gestão de conteúdo]** > **[!UICONTROL Modelos de conteúdo]** painel esquerdo.

1. Selecionar **[!UICONTROL Criar modelo]**.

   ![](assets/content-template-create.png){zoomable=&quot;yes&quot;}

1. Insira o rótulo e as propriedades do template. Você pode selecionar a pasta onde deseja armazenar o modelo. Por padrão, os modelos de conteúdo são armazenados em uma pasta dedicada da hierarquia do Adobe Campaign: **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Modelos]** > **[!UICONTROL Modelos de conteúdo]**. Saiba mais sobre pastas em [esta página](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png){zoomable=&quot;yes&quot;}

1. Clique em **[!UICONTROL Criar]** e escolha como deseja criar seu modelo a partir das diferentes opções:

   * [Projetar o conteúdo do zero](create-email-content.md) por meio da interface do Designer de email.

   * [Código ou HTML bruto de copiar e colar](code-content.md) diretamente no Designer de email.

   * [Importar conteúdo de HTML existente](existing-content.md) de um arquivo ou de uma pasta .zip.

   * Use conteúdo existente de uma lista de modelos incorporados ou personalizados. As etapas para usar um template de conteúdo em um email estão descritas em [nesta seção](use-email-templates.md).

   ![](assets/email_designer-templates.png){zoomable=&quot;yes&quot;}

1. O Designer de email é exibido. Edite o conteúdo conforme necessário, da mesma forma que faria para qualquer email, de acordo com a opção selecionada. Saiba como usar o Designer de email no [nesta seção](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Quando o modelo estiver pronto, clique em **[!UICONTROL Salvar]**.

   Se necessário, clique na seta ao lado do nome do template para voltar para a **[!UICONTROL Detalhes]** e editar seu modelo.

   ![](assets/content-template-save-back.png){zoomable=&quot;yes&quot;}

O template está disponível no **[!UICONTROL Modelos de conteúdo]** lista. [Saiba mais](#access-templates)

Agora você pode usar este template para criar um novo conteúdo: ele está disponível na **[!UICONTROL Modelos salvos]** do Designer de email. [Saiba como](use-email-templates.md)

### Salvar conteúdo de email como modelo {#save-as-template}

Uma vez que [criou um email](create-email-content.md), é possível salvar esse conteúdo como um template para reutilização futura. Os modelos salvos estão disponíveis para todos os usuários do seu ambiente Adobe Campaign.

Para salvar um conteúdo de email como modelo, siga as etapas a seguir:

1. No designer de email, clique no link **[!UICONTROL Mais]** botão na parte superior direita da tela.

1. Selecionar **[!UICONTROL Salvar como modelo de conteúdo]** no menu suspenso.

   ![](assets/email_designer-save-template.png){zoomable=&quot;yes&quot;}

1. Insira um nome para esse modelo e salve.

   ![](assets/email_designer-template-name.png){zoomable=&quot;yes&quot;}

O modelo é salvo e exibido no campo **[!UICONTROL Modelos de conteúdo]** lista. Ele se torna um modelo de conteúdo independente que pode ser acessado, editado e excluído como qualquer outro item nessa lista. [Saiba mais](#access-manage-templates)

Agora você pode usar este template para criar um novo conteúdo: ele está disponível na **[!UICONTROL Modelos salvos]** do Designer de email. [Saiba como](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable=&quot;yes&quot;}


>[!NOTE]
>
>Qualquer alteração nesse novo modelo não será propagada para o email de onde vem. Da mesma forma, quando o conteúdo original é editado nesse email, o novo modelo não é modificado.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## Modificar um modelo de conteúdo {#modify-delete}

Para atualizar um template de conteúdo existente, siga estas etapas:

1. Na lista de templates de conteúdo, clique no rótulo do template a ser modificado para editá-lo.

1. Clique em **[!UICONTROL Editar conteúdo]** botão para atualizar seu conteúdo com o [Email Designer](get-started-email-designer.md).

![](assets/content-template-edition.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>As alterações feitas em modelos de conteúdo não são propagadas para emails usando esse modelo de conteúdo.

## Excluir um modelo de conteúdo {#content-delete}

Há duas maneiras de excluir um template de conteúdo:

* na lista de templates de conteúdo, clique no botão reticências e selecione **Excluir**

  ![Excluir um modelo de conteúdo do painel](assets/content-template-list-delete.png)

* no próprio modelo de conteúdo, clique no link **Mais** e selecione **Excluir**


>[!NOTE]
>
>A exclusão de um template de conteúdo não afeta os deliveries criados usando esse template.


## Duplicação de um template de conteúdo {#content-duplicate}

Há duas maneiras de duplicar um template de conteúdo:

* na lista de templates de conteúdo, clique no botão reticências e selecione **Duplicar**

* no próprio modelo de conteúdo, clique no link **Mais** e selecione **Duplicar**

Em ambos os casos, confirme a duplicação para criar o novo template de conteúdo. O rótulo do novo template de conteúdo é **Cópia de`<label of the initial campaign`**. Navegue até as configurações do modelo para atualizar este rótulo.

