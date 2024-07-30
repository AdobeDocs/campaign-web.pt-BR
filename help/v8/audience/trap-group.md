---
audience: end-user
title: Usar um grupo de cobertura
hide: true
hidefromtoc: true
description: Saiba como usar um grupo de cobertura para a entrega na interface do usuário da Web do Campaign
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# Usar um **[!UICONTROL grupo de interceptação]** {#trap-group}

Um **[!UICONTROL grupo de interceptação]** (também conhecido como **[!UICONTROL lista de propagação]**) é usado para incluir endereços específicos em suas entregas para monitorar e verificar o processo de distribuição ao direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os recipients que estiverem fora do escopo de delivery podem recebê-lo, como qualquer outro recipient target receberia.
Um **[!UICONTROL grupo de interceptação]** é um grupo de **[!UICONTROL seed addresses]**, chamado **[!UICONTROL Perfil de teste]** na interface do usuário do AC Web.

## Por que usar o **[!UICONTROL Grupo de interceptação]**

Você pode usar **[!UICONTROL grupo de interceptação]**:

1. **Como uma prova**: cada membro do **[!UICONTROL grupo de interceptação]** receberá a entrega como se fizesse parte do público-alvo.


1. **Para proteger sua lista de endereçamento**: ao receber o que o público receberá, cada **[!UICONTROL perfil de teste]** do **[!UICONTROL Grupo de interceptação]** será notado se a lista de endereçamento for usada por um terceiro.

>[!NOTE]
>
>O grupo de interceptação é diferente de [enviar provas durante a criação da entrega](../email/create-email.md#preview-test) e do [grupo de controle](control-group.md).


## Sobre o **[!UICONTROL grupo de interceptação]**

Os perfis de teste são excluídos automaticamente dos relatórios nas seguintes estatísticas de entrega: **Cliques**, **Aberturas**, **Cancelamentos de assinatura**. Os relatórios são somente sobre o público real.

Para uma entrega de email, somente o endereço de email é necessário para o **[!UICONTROL Grupo de interceptação]**. A personalização de outros campos será preenchida aleatoriamente pelo Campaign.

## Como configurar um **[!UICONTROL Grupo de interceptação]** na entrega

Para configurar um **[!UICONTROL Grupo de interceptação]**, vá para as configurações de **[!UICONTROL Público]** da sua entrega. Você terá duas opções:
- [Selecionar perfis de teste](#select-test-profile)
- [Criar condição](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Selecionar perfis de teste {#select-test-profiles}

Ao escolher &quot;Selecionar perfis de teste&quot;, você terá a janela abaixo, onde é convidado a **[!UICONTROL Adicionar perfil(s) de teste]**:

![](assets/trap-no-test-profile.png){zoomable="yes"}

Ao clicar no botão, você terá acesso aos perfis de teste aos quais pode adicionar seu **[!UICONTROL grupo de interceptação]**. Marque as que deseja usar.
Você pode criar novos perfis de teste. [Saiba mais](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Ao confirmar seus perfis de teste, verifique se você tem o número correto em **[!UICONTROL Grupo de interceptação]**.

![](assets/trap-check.png){zoomable="yes"}

### Criar condição {#create-condition}

Com a opção **[!UICONTROL Criar condição]**, você obterá uma nova janela onde poderá personalizar uma consulta para definir os perfis de teste que deseja usar:

![](assets/trap-create-condition.png){zoomable="yes"}

Sua consulta será exibida em **[!UICONTROL Grupo de interceptação]**.

![](assets/trap-custom.png){zoomable="yes"}

## Como criar um novo **[!UICONTROL Perfil de teste]** {#create-seed}

Você pode criar um novo **[!UICONTROL perfil de teste]** no **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Membros de propagação]**

![](assets/trap-create.png){zoomable="yes"}

Você pode concluir todos os detalhes sobre seu **[!UICONTROL perfil de teste]** como se ele fosse um perfil de público-alvo:

![](assets/trap-create-contact.png){zoomable="yes"}