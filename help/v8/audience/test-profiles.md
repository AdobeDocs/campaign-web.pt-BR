---
title: Criar perfis de teste no Campaign
description: Saiba como criar e gerenciar perfis de teste no Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
badge: label="Disponibilidade limitada"
source-git-commit: 78f9bba52f33fac0e444afb3476873d931a873d1
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 3%

---

# Criar e gerenciar perfis de teste {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Criar perfis de teste"
>abstract="Os perfis de teste são criados como seed addresses. Eles são recipients adicionais no banco de dados usados para direcionar perfis fictícios que não correspondem aos critérios de target definidos."

Os perfis de teste são criados como seed addresses. Eles são recipients adicionais no banco de dados usados para direcionar perfis fictícios que não correspondem aos critérios de target definidos. Eles permitem visualizar e testar a personalização e renderização antes de enviar o delivery, enviando provas.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

As etapas para enviar mensagens de teste para seed addresses estão detalhadas em [nesta seção](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>Os perfis de teste são excluídos automaticamente dos relatórios nas seguintes estatísticas de delivery: **[!UICONTROL Cliques]**, **[!UICONTROL Aberturas]**, **[!UICONTROL Cancelamentos de assinatura]**.

## Acessar e gerenciar perfis de teste {#access-test-profiles}

Para acessar a lista de perfis de teste, selecione **[!UICONTROL Gerenciamento de clientes]** > **[!UICONTROL Perfis]** no menu esquerdo e clique na guia **[!UICONTROL Perfis de teste]** guia.

![](assets/test-profile-list.png)

É possível filtrar em um [pasta](../get-started/permissions.md#folders) usando a lista suspensa ou adicione regras usando o [modelador de consultas](../query/query-modeler-overview.md).

![](assets/test-profile-list-filters.png)

Para editar um perfil de teste, clique no item desejado na lista.

Para excluir um perfil de teste, selecione a opção correspondente na **[!UICONTROL Mais ações]** menu.

![](assets/test-profile-list-delete.png)

## Criar um perfil de teste {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Dados adicionais de perfis de teste"
>abstract="Insira os dados de personalização usados para os deliveries criados nos workflows de gestão de dados, aos quais você deseja atribuir um valor específico."

Para criar um perfil de teste, siga as etapas abaixo.

1. Navegue até **[!UICONTROL Gerenciamento de clientes]** > **[!UICONTROL Perfis]** e selecione o **[!UICONTROL Perfis de teste]** guia.

1. Clique em **[!UICONTROL Criar perfil de teste]** botão.

1. Preencha os detalhes do perfil de teste. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >A variável **[!UICONTROL Rótulo]** O campo é preenchido automaticamente com o nome e o sobrenome definidos.

1. Por padrão, os perfis de teste são armazenados no **[!UICONTROL Seed addresses]** pasta. Você pode alterá-la navegando até o local desejado. [Saiba mais](#seed-addresses-folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. No **[!UICONTROL Informações de contato]** insira o endereço de email e outros dados relevantes. O endereço de email é exibido entre colchetes após o rótulo do perfil de teste.

   ![](assets/test-profile-address.png)

1. Se você selecionar a variável **[!UICONTROL Não entrar mais em contato (por qualquer canal)]** , o perfil estará em incluir na lista de bloqueios. Esse recipient não é mais direcionado em nenhum canal (email, SMS, etc.).

1. No **[!UICONTROL Dados adicionais]** insira os dados de personalização usados para os deliveries criados nos workflows de gestão de dados, aos quais você deseja atribuir um valor específico. [Saiba mais sobre workflows](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Verifique se os dados adicionais do público-alvo foram definidos com um pseudônimo iniciado por &#39;@&#39; no **[!UICONTROL Enriquecimento]** atividade de workflow. Caso contrário, você não poderá usá-lo corretamente com seus seed addresses na atividade do delivery. [Saiba mais sobre a atividade de enriquecimento](../workflows/activities/enrichment.md)

1. Clique no botão **[!UICONTROL Save]**.

O perfil de teste que você acabou de criar está pronto para ser usado para enviar um teste. [Saiba mais](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Gerenciar pastas de seed addresses {#seed-addresses-folders}

Os seed addresses são armazenados em um nó dedicado da hierarquia do Adobe Campaign: **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]**.

Para organizar perfis de teste, você pode criar subpastas na lista suspensa Mais ações. [Saiba como criar pastas](../get-started/permissions.md#folders)

![](assets/test-profile-sub-folders.png)

Também é possível criar um perfil de teste a partir de qualquer **[!UICONTROL Seed addresses]** pasta ou subpasta. Preencha todos os detalhes da mesma forma que faria a partir do **[!UICONTROL Gerenciamento de clientes]** > **[!UICONTROL Perfis]** menu. [Saiba mais](#create-test-profile)

Para editar perfis de teste, clique no rótulo na caixa suspensa **[!UICONTROL Perfis de teste]** ou da pasta em que está armazenado.


