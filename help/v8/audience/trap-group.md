---
audience: end-user
title: Usar um grupo de cobertura
description: Saiba como usar um grupo de cobertura para a entrega na interface do usuário da Web do Campaign
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 4%

---

# Usar um grupo de cobertura {#trap-group}

Um **[!UICONTROL grupo de interceptação]** (também conhecido como **[!UICONTROL lista de propagação]**) é usado para incluir endereços específicos em suas entregas para monitorar e verificar o processo de distribuição ao direcionar perfis que não correspondem aos critérios de destino definidos. Dessa forma, os recipients que estiverem fora do escopo de delivery podem recebê-lo, como qualquer outro recipient target.

Um **[!UICONTROL grupo de interceptação]** é um grupo de **[!UICONTROL seed addresses]**, chamado **[!UICONTROL Perfil de teste]** na interface do usuário da Web do Campaign.

## Por que usar um grupo de cobertura {#why-trap-group}

Você pode usar um **[!UICONTROL grupo de interceptação]**:

1. **Como uma prova**: cada membro do **[!UICONTROL grupo de interceptação]** recebe a entrega como se fosse parte do público-alvo.

1. **Para proteger sua lista de endereçamento**: ao receber o que o público receberá, cada **[!UICONTROL Perfil de teste]** do **[!UICONTROL Grupo de interceptação]** será notado se a lista de endereçamento for usada por um terceiro.

>[!NOTE]
>
>Além de [enviar provas durante a criação da entrega](../email/create-email.md#preview-test) e do [grupo de controle](control-group.md), adicionar um grupo de interceptação é uma boa maneira de testar seu público.

## Sobre grupos de trapping {#about-trap-group}

Os perfis de teste são excluídos automaticamente dos relatórios nas seguintes estatísticas de entrega: **Cliques**, **Aberturas**, **Cancelamentos de assinatura**. Os relatórios se concentram somente no público-alvo real.

Para uma entrega de email, somente o endereço de email é necessário para o **[!UICONTROL Grupo de interceptação]**. A personalização de outros campos é preenchida aleatoriamente pelo Campaign.

## Adicionar um grupo de Interceptação em uma entrega {#trap-group-in-delivery}

Para configurar um **[!UICONTROL grupo de interceptação]**, vá para as configurações de **[!UICONTROL Público]** da sua entrega. Você terá duas opções:

* [Selecionar perfis de teste](#select-test-profiles)
* [Criar condição](#create-condition)

[Captura de tela da interface de configurações do grupo de interceptação](assets/trap-group.png){zoomable="yes"}

### Selecionar perfis de teste {#select-test-profiles}

Ao escolher **Selecionar perfis de teste**, use o botão **Adicionar perfil(s) de teste** como mostrado abaixo:

[Adicionar captura de tela do botão de perfil de teste](assets/trap-no-test-profile.png){zoomable="yes"}

Ao clicar no botão, você pode acessar os perfis de teste para adicionar ao seu **[!UICONTROL grupo de interceptação]**. Selecione os que deseja usar.

Você também pode criar novos perfis de teste. [Saiba mais](#create-seed)

[Selecionar captura de tela da interface de perfis de teste](assets/trap-select-test-profiles.png){zoomable="yes"}

Depois de confirmar seus perfis de teste, verifique se o número correto aparece em **[!UICONTROL Grupo de interceptação]**.

[Captura de tela de confirmação do grupo de interceptação](assets/trap-check.png){zoomable="yes"}

### Criar condição {#create-condition}

Com a opção **[!UICONTROL Criar condição]**, crie uma consulta para definir os perfis de teste que deseja usar:

[Criar captura de tela da interface de condição](assets/trap-create-condition.png){zoomable="yes"}

Sua consulta é exibida em **[!UICONTROL Grupo de interceptação]**.

[Captura de tela para exibição da consulta do grupo de interceptação](assets/trap-custom.png){zoomable="yes"}

## Criar um novo perfil de teste {#create-seed}

Você pode criar um novo **[!UICONTROL perfil de teste]** a partir da pasta **[!UICONTROL Explorer]** > **[!UICONTROL Recursos]** > **[!UICONTROL Gerenciamento de Campanhas]** > **[!UICONTROL Membros de propagação]**.

[Criar captura de tela de navegação do perfil de teste](assets/trap-create.png){zoomable="yes"}

Defina todas as configurações para seu **[!UICONTROL perfil de teste]** da mesma maneira que você faria para qualquer perfil:

[Testar captura de tela de configuração de perfil](assets/trap-create-contact.png){zoomable="yes"}