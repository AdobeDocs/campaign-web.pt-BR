---
audience: end-user
title: Configurar um grupo de controle
description: Saiba como definir um grupo de controle para suas mensagens na interface do Campaign Web
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Alpha" type="Positive"
source-git-commit: b5af5099d62e0e424fffdd8eb74d67f12777b0f2
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 100%

---

# Configurar um grupo de controle {#control-group}

Você pode usar grupos de controle para evitar o envio de mensagens para uma parte do público para medir o impacto das campanhas.

Para fazer isso, crie um grupo de controle ao definir o público da sua entrega. Perfis são adicionados ao grupo de controle aleatoriamente, filtrados ou não, ou baseados em critérios. Você poderá comparar o comportamento do público-alvo que recebeu a mensagem com o comportamento dos contatos não direcionados.

O grupo de controle pode ser extraído do público-alvo principal e/ou vir de uma população específica. Consequentemente, há duas maneiras principais de definir um grupo de controle:

* Extrair vários perfis do público-alvo principal.
* Excluir alguns perfis com base em critérios definidos em uma consulta.

Você pode usar ambos os métodos ao definir um grupo de controle.

Todos os perfis que fazem parte do grupo de controle na etapa de preparação da entrega serão removidos do público-alvo principal. Eles não recebem a mensagem.

Para criar um grupo de controle, clique no botão **[!UICONTROL Definir grupo de controle]**, da seção **Público** do assistente de criação de entrega.

![](assets/control-group1.png)

## Extrair do público-alvo {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extrair do público-alvo"
>abstract="Para definir um grupo de controle, você pode optar por extrair, aleatoriamente ou com base em uma classificação, uma porcentagem ou um número fixo de perfis do público-alvo."

Para definir um grupo de controle, você pode optar por extrair, aleatoriamente ou com base em uma classificação, uma porcentagem ou um número fixo de perfis do público-alvo.

Primeiro, defina como os perfis serão extraídos do público-alvo: aleatoriamente ou com base em uma classificação.

Na seção **Extrair do público-alvo**, escolha um **Tipo de exclusão**:

* **Aleatório**: ao preparar a entrega, o Adobe Campaign extrairá aleatoriamente um número de perfis correspondente à porcentagem ou ao número máximo que você definirá como o limite de tamanho.

   ![](assets/control-group.png)

* **Classificado por atributo(s)**: essa opção permite excluir um conjunto de perfis com base em atributo(s) específico(s) em uma ordem de classificação específica.

   ![](assets/control-group2.png)

Em seguida, defina o **Tamanho limite**: você deve definir como limitar o número de perfis extraídos do público-alvo principal.

**Exemplo**

Você pode visualizar os logs para verificar e identificar os perfis excluídos. Vejamos o exemplo de uma exclusão aleatória em cinco perfis.

![](assets/control-group4.png)

Após a preparação da entrega, é possível exibir as exclusões nas seguintes telas:

* O KPI **Para excluir**, no painel da entrega, antes do envio.

   ![](assets/control-group5.png)

* Os **Logs de exclusão** exibem cada perfil e o **Motivo** da exclusão relacionada. 

   ![](assets/control-group6.png)

* As **Causas da exclusão** exibem o número de perfis excluídos para cada regra de tipologia.

   ![](assets/control-group7.png)

Para obter mais informações sobre logs de entrega, consulte esta [seção](../monitor/delivery-logs.md).

## População extra {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="População extra"
>abstract="Outra forma de definir um grupo de controle é excluir uma população específica do direcionamento usando um público alvo ou definindo uma consulta."

Outra forma de definir um grupo de controle é excluir uma população específica do direcionamento usando um público alvo ou definindo uma consulta.

Na seção **População extra** do **Grupo de controle** na tela de definição, clique no botão **[!UICONTROL Selecionar público]**.

![](assets/control-group3.png)

* Para usar um público existente, clique em **Selecionar público**. Consulte esta [seção](add-audience.md).

* Para definir uma nova consulta, selecione **Criar sua própria** e defina os critérios de exclusão usando o Construtor de regras. Consulte esta [seção](segment-builder.md).

Os perfis incluídos no público ou que correspondem ao resultado da consulta são excluídos do público-alvo.