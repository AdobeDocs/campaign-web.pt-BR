---
audience: end-user
title: Planos e programas
description: Saiba como criar e configurar planos e programas no Adobe Campaign
exl-id: 0307bcb7-7ab5-4226-bad1-cb7cf10e97fc
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 3%

---

# Planos e programas {#plan-and-programs}

O Adobe Campaign permite configurar uma hierarquia de pastas para planos e programas de marketing.

Para organizar melhor esses componentes, a Adobe recomenda a seguinte hierarquia: Planejar `>` Programas `>` Campanhas.

* Um **plano** pode conter vários programas. Define objetivos estratégicos para um período específico.
* Um **programa** pode conter outros programas, assim como campanhas, fluxos de trabalho e páginas de aterrissagem.
* Uma **campanha** pode conter entregas, fluxos de trabalho e páginas de aterrissagem.

## Criar e configurar um plano {#create-plan}

Para criar um plano, crie uma pasta do tipo **[!UICONTROL Plano]**. [Saiba mais sobre como criar uma pasta](../get-started/work-with-folders.md)

![Captura de tela mostrando a criação de uma pasta de plano](assets/plan_create.png){zoomable="yes"}

Vá para as **[!UICONTROL Configurações de pasta]** do seu plano para gerenciá-lo.

![Captura de tela mostrando as configurações de pasta de um plano](assets/plan_settings.png){zoomable="yes"}

Defina as **[!UICONTROL Opções personalizadas]** e defina a data de agendamento do seu plano.

![Captura de tela mostrando as opções personalizadas de um plano](assets/plan_options.png){zoomable="yes"}

Para gerenciar as **[!UICONTROL Opções personalizadas]**:

1. Navegue até **[!UICONTROL Esquemas]**.
1. Escolha os esquemas **[!UICONTROL Editáveis]** nos filtros.
1. Clique no ícone **[!UICONTROL Editar detalhes personalizados]**.

![Captura de tela mostrando a edição de detalhes personalizados para um plano](assets/plan_edit.png){zoomable="yes"}

Configure as opções personalizadas:

![Captura de tela mostrando a configuração de campos personalizados para um plano](assets/plan_customfields.png){zoomable="yes"}

## Criar e configurar um programa

Para criar um programa em seu plano ([Saiba mais sobre como criar um plano](#create-plan)), navegue até seu plano e crie uma pasta com o tipo de pasta **[!UICONTROL Programa]**. [Saiba mais sobre como criar uma pasta](../get-started/work-with-folders.md).

![Captura de tela mostrando a criação de uma pasta de programa](assets/program_create.png){zoomable="yes"}

Vá para as **[!UICONTROL Configurações de pasta]** do seu programa para gerenciá-lo.

![Captura de tela mostrando as configurações de pasta de um programa](assets/program_settings.png){zoomable="yes"}

Defina as **[!UICONTROL Opções personalizadas]** e defina a data de agendamento do seu programa.

![Captura de tela mostrando as opções personalizadas de um programa](assets/program_options.png){zoomable="yes"}

Para gerenciar as **[!UICONTROL Opções personalizadas]**:

1. Navegue até **[!UICONTROL Esquemas]**.
1. Escolha os esquemas **[!UICONTROL Editáveis]** nos filtros.
1. Clique no ícone **[!UICONTROL Editar detalhes personalizados]**.

![Captura de tela mostrando a edição de detalhes personalizados para um programa](assets/program_edit.png){zoomable="yes"}

Configure as opções personalizadas:

![Captura de tela mostrando a configuração de campos personalizados para um programa](assets/program_customfields.png){zoomable="yes"}

## Como vincular uma campanha a um programa

Há duas maneiras de vincular uma campanha a um programa:

### Way #1: Você já tem um programa e deseja criar uma campanha vinculada a ele

Para vincular uma nova campanha ao seu programa, crie a campanha diretamente no programa.

![Captura de tela mostrando a criação de uma campanha em um programa](assets/program_campaign_create.png){zoomable="yes"}

As configurações de **[!UICONTROL Pasta]** serão preenchidas automaticamente com o caminho para o seu programa.

![Captura de tela mostrando as configurações da pasta para uma campanha vinculada a um programa](assets/program_campaign_folder.png){zoomable="yes"}

### Way #2: você já tem uma campanha existente e deseja vinculá-la a um programa existente

Vá para o botão **[!UICONTROL Configurações]** da campanha que deseja vincular ao seu programa.

![Captura de tela mostrando o botão de configurações para uma campanha](assets/campaign_settings.png){zoomable="yes"}

Em suas **[!UICONTROL Propriedades]**, clique no ícone **[!UICONTROL Pasta]** nas configurações de **[!UICONTROL Pasta]** para escolher sua pasta **[!UICONTROL Programa]**.

![Captura de tela mostrando a seleção de pastas para vincular uma campanha a um programa](assets/campaign_folder.png){zoomable="yes"}

Selecione a pasta **[!UICONTROL Programa]**, clique no botão **[!UICONTROL Confirmar]** e clique no botão **[!UICONTROL Salvar e Fechar]**.

![Captura de tela mostrando uma campanha vinculada a um programa](assets/campaign_linked.png){zoomable="yes"}

Sua campanha agora está listada em seu programa.

![Captura de tela mostrando uma campanha listada em um programa](assets/campaign_in_program.png){zoomable="yes"}