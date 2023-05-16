---
audience: end-user
title: Criar emails usando o Designer de email
description: Saiba como criar o conteúdo de um email do zero
exl-id: 23e71da3-434d-4619-a48a-334281592d85
badge: label="Alpha" type="Positive"
source-git-commit: d7e19b2d8730cacbbff1ad42f1956b32c84a309a
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 100%

---

# Criar o conteúdo do email do zero {#create-email-content}

>[!CONTEXTUALHELP]
>id="ac_structure_components_email"
>title="Sobre os componentes de estrutura"
>abstract="Os componentes de estrutura definem o layout do email."

>[!CONTEXTUALHELP]
>id="ac_structure_components_landing_page"
>title="Sobre os componentes de estrutura"
>abstract="Os componentes de estrutura definem o layout da landing page."

>[!CONTEXTUALHELP]
>id="ac_structure_components_fragment"
>title="Sobre os componentes de estrutura"
>abstract="Os componentes de estrutura definem o layout do fragmento."

>[!CONTEXTUALHELP]
>id="ac_structure_components_template"
>title="Sobre os componentes de estrutura"
>abstract="Os componentes de estrutura definem o layout do modelo."


>[!CONTEXTUALHELP]
>id="ac_edition_columns_email"
>title="Definição de colunas de email"
>abstract="O Designer de email permite definir facilmente o layout do email definindo a estrutura da coluna."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_landing_page"
>title="Definir as colunas da landing page"
>abstract="O Designer de email permite definir facilmente o layout da landing page definindo a estrutura da coluna."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_fragment"
>title="Definição de colunas do fragmento"
>abstract="O Designer de email permite definir facilmente o layout do fragmento definindo a estrutura da coluna."

>[!CONTEXTUALHELP]
>id="ac_edition_columns_template"
>title="Definição de colunas de modelo"
>abstract="O Designer de email permite definir facilmente o layout do modelo definindo a estrutura da coluna."

O Designer de email permite definir a estrutura do email com facilidade. Ao adicionar e mover elementos estruturais com ações simples de arrastar e soltar, você pode criar o corpo do seu email em segundos.

Para começar a criar o conteúdo de email, siga as etapas abaixo:

1. Na página inicial do Designer de email, selecione a opção **[!UICONTROL Criar do zero]**.

   ![](assets/email_designer.png)

1. Comece a criar o conteúdo de email arrastando e soltando **[!UICONTROL componentes de estrutura]** na tela para definir o layout do email.

   >[!NOTE]
   >
   >O empilhamento de colunas não é compatível com todos os programas de email. Se o recurso não for compatível, as colunas não serão empilhadas.

   <!--Once placed in the email, you cannot move nor remove your components unless there is already a content component or a fragment placed inside. This is not true in AJO - TBC?-->

   ![](assets/email_designer_2.png)

1. Adicione quantos **[!UICONTROL componentes de estrutura]** for necessário e edite suas configurações no painel dedicado à direita.

   Selecione o componente **[!UICONTROL coluna n:n]** para definir um número de colunas (entre 3 e 10). Você também pode definir a largura de cada coluna movendo as setas na parte inferior de cada coluna.

   >[!NOTE]
   >
   >O tamanho de cada coluna não pode ser inferior a 10% da largura total do componente de estrutura. Não é possível remover uma coluna que não esteja vazia.

1. Expanda a seção **[!UICONTROL Componentes de conteúdo]** e adicione quantos elementos forem necessários em um ou mais componentes de estrutura. [Saiba mais sobre componentes de conteúdo](content-components.md)

1. Cada componente pode ser personalizado ainda mais usando as **[!UICONTROL Configurações do componente]** no painel à direita. Por exemplo, é possível alterar o estilo do texto, o preenchimento ou a margem de cada componente. [Saiba mais sobre alinhamento e preenchimento](alignment-and-padding.md)

   ![](assets/email_designer_5.png)

1. Insira campos de personalização para personalizar seu conteúdo de email a partir de dados de perfis. [Saiba mais sobre a personalização de conteúdo](../personalization/personalize.md)

1. Clique na guia **[!UICONTROL Links]** no painel esquerdo para exibir todos os URLs do conteúdo que devem ser rastreados. Você pode modificar o **[!UICONTROL Tipo de rastreamento]** ou o **[!UICONTROL Rótulo]** e adicionar **[!UICONTROL Categorias]** se necessário. [Saiba mais sobre links e rastreamento de mensagens](message-tracking.md)

   ![](assets/email_designer_7.png)

1. Se necessário, é possível personalizar ainda mais o email clicando em **[!UICONTROL Alternar para o editor de código]** no menu avançado. Isso permite editar o código-fonte do email, por exemplo, para adicionar rastreamento ou tags de HTML personalizadas. [Saiba mais sobre o editor de código](code-content.md)

   >[!CAUTION]
   >
   >Não é possível reverter para o designer visual desse email após alternar para o editor de código.

1. Quando o conteúdo estiver pronto, clique em **[!UICONTROL Simular conteúdo]** para verificar a renderização do email. Você pode escolher exibir no desktop ou em um dispositivo móvel. [Saiba mais sobre como visualizar seu email](../preview-test/preview-test.md)

   ![](assets/email_designer_28.png)

1. Quando o email estiver pronto, clique em **[!UICONTROL Salvar]**.

