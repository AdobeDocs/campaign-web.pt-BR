---
audience: end-user
title: Planos e programas
description: Saiba como criar e configurar planos e programas no Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 5%

---

# Planos e programas {#plan-and-programs}

O Adobe Campaign permite configurar uma hierarquia de pastas para planos e programas de marketing.

Para organizá-los melhor, o Adobe recomenda a seguinte hierarquia: Plan `>` Programs `>` Campaigns

* Um **plano** pode conter vários programas. Define objetivos estratégicos por um período.
* Um **programa** pode conter outros programas, assim como campanhas, fluxos de trabalho e páginas de aterrissagem.
* Uma **campanha** pode conter entregas, fluxos de trabalho e páginas de aterrissagem.

## Criar e configurar um plano {#create-plan}

Para criar um plano, você precisa criar uma pasta com o tipo de pasta **[!UICONTROL Plano]** [Saiba mais sobre como criar uma pasta](../get-started/work-with-folders.md).

![](assets/plan_create.png){zoomable="yes"}

Vá para as **[!UICONTROL Configurações de pasta]** do seu plano para gerenciá-lo.

![](assets/plan_settings.png){zoomable="yes"}

Você pode definir **[!UICONTROL Opções personalizadas]** e definir a data de agendamento do seu plano.

![](assets/plan_options.png){zoomable="yes"}

Para gerenciar as **[!UICONTROL Opções personalizadas]**:

1. Navegue até os **[!UICONTROL Esquemas]**
1. Escolha os esquemas **[!UICONTROL Editáveis]** nos filtros
1. Clique no ícone de **[!UICONTROL Editar detalhes personalizados]**

![](assets/plan_edit.png){zoomable="yes"}

Você pode configurá-los:

![](assets/plan_customfields.png){zoomable="yes"}

## Criar e configurar um programa

Para criar um programa em seu plano ([Saiba mais sobre como criar um plano](#create-plan)), você precisa estar em seu plano e criar uma pasta com o tipo de pasta **[!UICONTROL Programa]** [Saiba mais sobre como criar uma pasta](../get-started/work-with-folders.md).

![](assets/program_create.png){zoomable="yes"}

Vá para as **[!UICONTROL Configurações de pasta]** do seu programa para gerenciá-lo.

![](assets/program_settings.png){zoomable="yes"}

Você pode definir **[!UICONTROL Opções personalizadas]** e definir a data de agendamento do seu programa.

![](assets/program_options.png){zoomable="yes"}

Para gerenciar as **[!UICONTROL Opções personalizadas]**:

1. Navegue até os **[!UICONTROL Esquemas]**
1. Escolha os esquemas **[!UICONTROL Editáveis]** nos filtros
1. Clique no ícone de **[!UICONTROL Editar detalhes personalizados]**

![](assets/program_edit.png){zoomable="yes"}

Você pode configurá-los:

![](assets/program_customfields.png){zoomable="yes"}

## Como vincular uma campanha a um programa

Há duas maneiras de vincular uma campanha a um programa:

### Way #1: Você já tem um programa e deseja criar uma campanha vinculada a ele

Para vincular uma nova campanha ao seu programa, crie uma campanha diretamente no programa:

![](assets/program_campaign_create.png){zoomable="yes"}

As configurações de **[!UICONTROL Pasta]** serão automaticamente arquivadas com o caminho para o seu programa.

![](assets/program_campaign_folder.png){zoomable="yes"}

### Way #2: você já tem uma campanha existente e deseja vinculá-la a um programa existente

Vá para o botão **[!UICONTROL Configurações]** da campanha que deseja vincular ao seu programa:

![](assets/campaign_settings.png){zoomable="yes"}

Em suas **[!UICONTROL Propriedades]**, clique no ícone **[!UICONTROL Pasta]** nas configurações de **[!UICONTROL Pasta]** para escolher sua pasta **[!UICONTROL Programa]**.

![](assets/campaign_folder.png){zoomable="yes"}

Selecione a pasta **[!UICONTROL Programa]** e clique no botão **[!UICONTROL Confirmar]** e depois no botão **[!UICONTROL Salvar e Fechar]**.

![](assets/campaign_linked.png){zoomable="yes"}

Sua campanha agora está listada em seu programa:

![](assets/campaign_in_program.png){zoomable="yes"}
