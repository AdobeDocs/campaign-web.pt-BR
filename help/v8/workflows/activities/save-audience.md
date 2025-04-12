---
audience: end-user
title: Usar a atividade de fluxo de trabalho Salvar público
description: Saiba como usar a atividade de fluxo de trabalho Bifurcação
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 12%

---

# Salvar público-alvo {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Salvar um público-alvo"
>abstract="Use esta atividade para atualizar um público-alvo já existente ou criar um novo a partir da população calculada upstream em um fluxo de trabalho. Os públicos-alvo criados são adicionados à lista de públicos-alvo e disponibilizados no menu **Públicos-alvo**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Gerar transição de saída"
>abstract="Use esta opção se quiser adicionar uma transição após a atividade **Salvar público-alvo**."

A atividade **Salvar público-alvo** é uma atividade **de Direcionamento**. Esta atividade permite atualizar um público-alvo ou criar um novo público-alvo a partir da população computada upstream em um fluxo de trabalho. Os públicos-alvo criados são adicionados à lista de públicos-alvo do aplicativo e disponibilizados pelo menu **Públicos-alvo**.

Essa atividade é usada principalmente para reter grupos de populações computados no mesmo fluxo de trabalho, convertendo-os em públicos-alvo reutilizáveis. Conecte-a a outras atividades de direcionamento, como uma atividade **Criar público** ou **Combinar**.

## Configurar a atividade Save audience {#save-audience-configuration}

Siga estas etapas para configurar a atividade **Salvar público-alvo**:

![Descrição: Configuração de fluxo de trabalho para a atividade Salvar público-alvo](../assets/workflow-save-audience.png)

1. Adicione uma atividade **Save audience** ao seu fluxo de trabalho.

1. No menu suspenso **Modo**, selecione a ação que deseja executar:

   * **Criar ou atualizar um público existente**: definir um **Rótulo de público-alvo**. Se o público-alvo já existir, ele será atualizado; caso contrário, um novo público-alvo será criado.

   * **Atualizar um público-alvo** existente: escolha o **Público-alvo** que deseja atualizar na lista de públicos-alvo existentes.

1. Selecione o **Modo de atualização** que se aplica aos públicos existentes:

   * **Substituir conteúdo do público-alvo por novos dados**: todo o conteúdo do público-alvo é substituído e os dados antigos são perdidos. Somente os dados da transição de entrada da atividade **Salvar público-alvo** são retidos. Essa opção apaga o tipo de público-alvo e o targeting dimension do público-alvo atualizado.

   * **Concluir público-alvo com novos dados**: o conteúdo antigo do público-alvo é retido e os dados da transição de entrada da atividade **Salvar público-alvo** são adicionados a ele.

1. Marque a opção **Generate an outbound transition** se desejar adicionar uma transição após a atividade **Save audience**.

O conteúdo do público-alvo salvo ficará disponível na exibição detalhada do público-alvo, que pode ser acessada no menu **Públicos-alvo**. As colunas disponíveis nesta exibição correspondem às da transição de entrada da atividade **Salvar público-alvo** do fluxo de trabalho.

## Exemplo {#save-audience-example}

O exemplo a seguir ilustra uma simples atualização de público-alvo do direcionamento. Um scheduler executa o workflow uma vez por mês. Um query recupera todos os perfis que fizeram assinatura nos diferentes aplicativos disponíveis. A atividade **Salvar público-alvo** atualiza o público-alvo removendo os perfis que cancelaram a assinatura do serviço desde a última execução do fluxo de trabalho e adicionando perfis que fizeram assinatura recentemente.