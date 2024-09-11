---
audience: end-user
title: Usar um grupo de cobertura
description: Saiba como usar um grupo de cobertura para a entrega na interface do usuário da Web do Campaign
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: dfd5f2e000b02d4382eaac0c9bb00fe940a99f79
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 17%

---

# Usar um grupo de cobertura {#trap-group}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Grupo de interceptação"
>abstract="Você pode usar um grupo de cobertura para incluir endereços específicos nas suas entregas a fim de monitorar e verificar o processo de distribuição ao direcionar perfis que não correspondem aos critérios de direcionamento definidos."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

Um **[!UICONTROL grupo de interceptação]** (também conhecido como **[!UICONTROL lista de propagação]**) é usado para incluir endereços específicos em suas entregas para monitorar e verificar o processo de distribuição ao direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os destinatários que estiverem fora do escopo de entrega podem recebê-lo, como qualquer outro destinatário target receberia.

Um **[!UICONTROL grupo de interceptação]** é um grupo de **[!UICONTROL seed addresses]**, chamado **[!UICONTROL Perfil de teste]** na interface do usuário da Web do Campaign.

## Por que usar um grupo de cobertura {#why-trap-group}

Você pode usar o **[!UICONTROL grupo de interceptação]**:

1. **Como uma prova**: cada membro do **[!UICONTROL grupo de interceptação]** receberá a entrega como se fizesse parte do público-alvo.

1. **Para proteger sua lista de endereçamento**: ao receber o que o público receberá, cada **[!UICONTROL perfil de teste]** do **[!UICONTROL Grupo de interceptação]** será notado se a lista de endereçamento for usada por um terceiro.

>[!NOTE]
>
>Além de [enviar provas durante a criação da entrega](../email/create-email.md#preview-test) e do [grupo de controle](control-group.md), adicionar um grupo de interceptação é uma boa maneira de testar seu público.

## Sobre grupos de trapping {#about-trap-group}

Os perfis de teste são excluídos automaticamente dos relatórios nas seguintes estatísticas de entrega: **Cliques**, **Aberturas**, **Cancelamentos de assinatura**. Os relatórios são somente sobre o público real.

Para uma entrega de email, somente o endereço de email é necessário para o **[!UICONTROL Grupo de interceptação]**. A personalização de outros campos será preenchida aleatoriamente pelo Campaign.

## Adicionar um grupo de Interceptação em uma entrega {#trap-group-in-delivery}

Para configurar um **[!UICONTROL Grupo de interceptação]**, vá para as configurações de **[!UICONTROL Público]** da sua entrega. Você terá duas opções:

* [Selecionar perfis de teste](#select-test-profile)
* [Criar condição](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Selecionar perfis de teste {#select-test-profiles}

Ao escolher **Selecionar perfis de teste**, você pode usar o botão **Adicionar perfil(s) de teste** como mostrado abaixo:

![](assets/trap-no-test-profile.png){zoomable="yes"}

Ao clicar no botão, você tem acesso aos perfis de teste que podem ser adicionados ao seu **[!UICONTROL grupo de interceptação]**. Selecione os que deseja usar.

Você também pode criar novos perfis de teste. [Saiba mais](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Ao confirmar seus perfis de teste, verifique se você tem o número correto em **[!UICONTROL Grupo de interceptação]**.

![](assets/trap-check.png){zoomable="yes"}

### Criar condição {#create-condition}

Com a opção **[!UICONTROL Criar condição]**, você pode criar uma consulta para definir os perfis de teste que deseja usar:

![](assets/trap-create-condition.png){zoomable="yes"}

Sua consulta é exibida em **[!UICONTROL Grupo de interceptação]**.

![](assets/trap-custom.png){zoomable="yes"}

## Criar um novo perfil de teste {#create-seed}

Você pode criar um novo **[!UICONTROL perfil de teste]** a partir da pasta **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membros de origem]**.

![](assets/trap-create.png){zoomable="yes"}

Defina todas as configurações sobre seu **[!UICONTROL perfil de teste]** como para qualquer perfil:

![](assets/trap-create-contact.png){zoomable="yes"}
