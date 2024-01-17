---
audience: end-user
product: campaign
title: Trabalho com modelos de conteúdo
description: Saiba como criar modelos para reutilizar conteúdo em emails do Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="Disponibilidade limitada"
source-git-commit: 0d9d61e8561d21bca00cb5c274884624119eaa53
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 15%

---

# Trabalho com modelos de conteúdo {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Definir seu próprio conteúdo"
>abstract="Crie um modelo personalizado independente do zero para tornar seu conteúdo reutilizável em vários emails."

Para um processo de design acelerado e aprimorado, é possível criar modelos independentes para reutilizar facilmente o conteúdo personalizado em [!DNL Adobe Campaign].

Essa funcionalidade permite que os usuários orientados a conteúdo trabalhem em modelos independentes para que os usuários de marketing possam reutilizar e adaptá-los em suas próprias campanhas de email.

>[!NOTE]
>
>Somente no momento **email** modelos de conteúdo são compatíveis.

## Acessar e gerenciar modelos  {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Editar o conteúdo do modelo"
>abstract="Clique em **Editar conteúdo** para atualizar o conteúdo com o Designer de email."

Para acessar a lista de modelos de conteúdo, selecione **[!UICONTROL Gestão de conteúdo]** > **[!UICONTROL Modelos de conteúdo]** no menu esquerdo.

![](assets/content-template-list.png)

Todos os modelos criados - de um email usando o [Salvar como modelo](#save-as-template) opção, seja a partir da variável **[!UICONTROL Modelos de conteúdo]** - são exibidos.

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

É possível filtrar em um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

Para editar o conteúdo de um modelo, clique no item desejado na lista. Você pode:

* Editar suas propriedades.

* Clique em **[!UICONTROL Editar conteúdo]** botão para atualizar seu conteúdo com o [Email Designer](get-started-email-designer.md).

![](assets/content-template-edition.png)

Para excluir um template, selecione a opção correspondente no **[!UICONTROL Mais ações]** menu.

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>Quando um template é excluído, os deliveries criados usando esse template não são afetados.

## Criar modelos de conteúdo {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Design do modelo de conteúdo"
>abstract="Design do modelo de conteúdo"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Seleção do modelo de conteúdo"
>abstract="Seleção do modelo de conteúdo"

Há duas maneiras de criar modelos de conteúdo:

* Criar um modelo de conteúdo do zero, usando o painel esquerdo **[!UICONTROL Modelos de conteúdo]** menu. [Saiba como](#create-template-from-scratch)

* Ao criar um email, salve seu conteúdo de email como template. [Saiba como](#save-as-template)

Depois de salvo, seja criado do zero ou de um email anterior, agora é possível usar esse modelo ao criar qualquer [email](../email/create-email.md) no prazo de [!DNL Adobe Campaign]. [Saiba como](use-email-templates.md)

>[!NOTE]
>
>* As alterações feitas em modelos de conteúdo não são propagadas para emails.
>
>* Da mesma forma, quando os modelos são usados em um email, as edições feitas no conteúdo do email não afetam o modelo de conteúdo usado anteriormente.

### Criar modelo do zero {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Definir as propriedades do modelo"
>abstract="Ao criar um modelo do zero, defina suas propriedades para que ele possa ser recuperado com facilidade, quando necessário."

Para criar um template de conteúdo do zero, siga as etapas abaixo.

1. Acesse a lista de templates de conteúdo por meio da **[!UICONTROL Gestão de conteúdo]** > **[!UICONTROL Modelos de conteúdo]** menu esquerdo.

1. Selecionar **[!UICONTROL Criar modelo]**.

   ![](assets/content-template-create.png)

1. Preencha os detalhes do template. Você pode selecionar a pasta onde deseja armazenar o modelo. Por padrão, os modelos de conteúdo são armazenados em uma pasta dedicada da hierarquia do Adobe Campaign: **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Modelos]** > **[!UICONTROL Modelos de conteúdo]**. [Saiba como criar pastas](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >Atualmente, somente o **E-mail** canal e **HTML** tipo são compatíveis.

1. Clique em **[!UICONTROL Criar]** e escolha como deseja criar seu modelo a partir das diferentes opções:

   * [Projetar o email do zero](create-email-content.md) por meio da interface do Designer de email.

   * [Código ou HTML bruto de copiar e colar](code-content.md) diretamente no Designer de email.

   * [Importar conteúdo de HTML existente](existing-content.md) de um arquivo ou de uma pasta .zip.

   * Use conteúdo existente de uma lista de modelos incorporados ou personalizados. As etapas para usar um template de conteúdo em um email estão descritas em [nesta seção](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. A variável [Email Designer](get-started-email-designer.md) é exibido. Edite o conteúdo conforme necessário, da mesma forma que faria para qualquer email, de acordo com a opção selecionada.

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Quando o modelo estiver pronto, clique em **[!UICONTROL Salvar]**.

   Se necessário, clique na seta ao lado do nome do template para voltar para a **[!UICONTROL Detalhes]** e editar seu modelo.

   ![](assets/content-template-save-back.png)

O modelo é salvo na pasta padrão da hierarquia do Adobe Campaign (**[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Modelos]** > **[!UICONTROL Modelos de conteúdo]**). [Saiba mais sobre pastas](../get-started/permissions.md#folders)

Ele também é exibido na **[!UICONTROL Modelos de conteúdo]** lista. [Saiba mais](#access-manage-templates)

Agora você pode usar este template para criar um novo conteúdo: ele está disponível na **[!UICONTROL Modelos salvos]** do Designer de email. [Saiba como](use-email-templates.md)

### Salvar conteúdo de email como modelo {#save-as-template}

Uma vez que [criou um email](create-email-content.md), é possível salvar esse conteúdo como um template para reutilização futura. Os modelos salvos estão disponíveis para todos os usuários do seu ambiente Adobe Campaign.

Para salvar um conteúdo de email como modelo, siga as etapas a seguir:

1. No designer de email, clique no link **[!UICONTROL Mais]** botão na parte superior direita da tela.

1. Selecionar **[!UICONTROL Salvar como modelo de conteúdo]** no menu suspenso.

   ![](assets/email_designer-save-template.png)

1. Insira um nome para esse modelo e salve.

   ![](assets/email_designer-template-name.png)

O modelo é salvo na pasta padrão da hierarquia do Adobe Campaign (**[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Modelos]** > **[!UICONTROL Modelos de conteúdo]**). [Saiba mais sobre pastas](../get-started/permissions.md#folders)

Ele também é exibido na **[!UICONTROL Modelos de conteúdo]** lista. Ele se torna um modelo de conteúdo independente que pode ser acessado, editado e excluído como qualquer outro item nessa lista. [Saiba mais](#access-manage-templates)

Agora você pode usar este template para criar um novo conteúdo: ele está disponível na **[!UICONTROL Modelos salvos]** do Designer de email. [Saiba como](use-email-templates.md)

![](assets/email_designer-saved-template.png)

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



