---
audience: end-user
title: Configurar um grupo de controle
description: Saiba como definir um grupo de controle para suas mensagens na interface do Campaign Web
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Beta"
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 42%

---

# Configurar um grupo de controle {#control-group}

Um grupo de controle é uma subpopulação excluída da entrega. Você pode definir um grupo de controle para evitar o envio de mensagens para uma parte do público-alvo e comparar o comportamento após o delivery com o público-alvo principal. Essa opção ajuda a medir o impacto da campanha.

## Habilitar grupo de controle{#add-a-control-group}

Para adicionar um grupo de controle, habilite a opção ao definir o público do seu delivery. O grupo de controle pode ser extraído do público-alvo principal e/ou vir de uma população específica. Consequentemente, há duas maneiras principais de definir um grupo de controle:

* Extrair vários perfis do público-alvo principal.
* Excluir alguns perfis de uma lista ou com base nos critérios definidos em uma query.

Você pode combinar ambos os métodos ao definir um grupo de controle.

Todos os perfis que fazem parte do grupo de controle na etapa de preparação da entrega serão removidos do público-alvo principal. Eles não recebem a mensagem.

>[!CAUTION]
>
>Não é possível usar grupos de controle ao carregar a população alvo [a partir de um arquivo externo](file-audience.md).

Para adicionar um grupo de controle a um delivery, ative a variável **[!UICONTROL Ativar grupo de controle]** alternar, no campo **Público** seção da tela de criação do delivery.

![Opção Habilitar grupo de controle](assets/control-group1.png)


## Extrair do público-alvo {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Modo de extração"
>abstract="Um grupo de controle é um conjunto de perfis excluídos do delivery. Para definir um grupo de controle, você pode optar por extrair, aleatoriamente ou com base em uma classificação, uma porcentagem ou um número fixo de perfis do público-alvo."


### Criar um grupo de controle {#build-extract-target}

Para definir um grupo de controle, você pode optar por extrair, aleatoriamente ou com base em uma classificação, uma porcentagem ou um número fixo de perfis do público-alvo. Se preferir adicionar uma população extra, escolha a opção **Sem extração** e selecione a população extra [conforme detalhado aqui](#extra-population).

Primeiro, defina como os perfis são extraídos do público-alvo: aleatoriamente ou com base em uma classificação.

No **Grupo de controle** escolha uma **Modo de extração**:

* **Aleatório**: ao preparar a entrega, o Adobe Campaign extrairá aleatoriamente um número de perfis correspondente à porcentagem ou ao número máximo que você definirá como o limite de tamanho.

* **Classificado por atributo(s)**: essa opção permite excluir um conjunto de perfis com base em atributo(s) específico(s) em uma ordem de classificação específica.


Em seguida, use o **Limite de tamanho** para definir o número de perfis que precisam ser extraídos do público-alvo principal. Pode ser um número bruto (por exemplo, 50 perfis a serem excluídos) ou uma porcentagem do público inicial (por exemplo, 5% do público-alvo principal).


### Amostra do grupo de controle{#control-group-sample}

Por exemplo, para criar um grupo de controle com os 100 novos recipients mais jovens, siga estas etapas:

1. Selecione o **Idade** como um critério de classificação. Deixe a **Crescente** opção de classificação.
1. Adicione o **Data de criação** campo. Altere para a variável **Decrescente** opção de classificação.
1. Defina 100 como o limite no **Limite de tamanho** seção.

   ![](assets/control-group2.png)

Esses 100 novos recipients mais jovens são excluídos do target principal.

### Verifique seu grupo de controle {#check-control-group}

Você pode visualizar os logs para verificar e identificar os perfis excluídos. Vejamos o exemplo de uma exclusão aleatória em cinco perfis.

![](assets/control-group4.png)

Após a preparação do delivery, é possível revisar como as exclusões foram aplicadas:

* No painel de delivery, antes do envio, marque a opção **Para excluir** KPI.

  ![](assets/control-group5.png)

* Nos logs do delivery, a guia Logs mostra a etapa de exclusão.

  ![](assets/control-group-sample-logs.png)
<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png)
-->

* A variável **Causas de exclusão** exibe o número de perfis excluídos para cada regra de tipologia.

  ![](assets/control-group7.png)

Para obter mais informações sobre logs de entrega, consulte esta [seção](../monitor/delivery-logs.md).

## Adicionar uma população extra {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="População extra"
>abstract="Um grupo de controle é um conjunto de perfis excluídos do delivery. Você pode excluir uma população específica do público-alvo da entrega selecionando um público-alvo já existente ou definindo uma consulta."

Outra maneira de definir um grupo de controle é selecionar uma população específica em um público-alvo existente ou definir um query.

Na seção **População extra** do **Grupo de controle** na tela de definição, clique no botão **[!UICONTROL Selecionar público-alvo]**.

![](assets/control-group3.png)

* Para usar um público existente, clique em **Selecionar público-alvo**. Saiba mais [nesta seção](add-audience.md).

* Para definir uma nova consulta, selecione **Criar sua própria** e defina os critérios de exclusão usando o Construtor de regras. Saiba mais [nesta seção](segment-builder.md).

Os perfis incluídos no público ou que correspondem ao resultado do query são **excluído** do target do delivery: eles não recebem nenhuma mensagem.

## Comparar os resultados{#control-group-results}

Depois que o delivery for enviado, você poderá extrair os logs de envio para comparar o comportamento entre os perfis que não receberam a comunicação e o público-alvo efetivo. Você também pode usar os logs do delivery para criar um novo direcionamento.

Para ver quais perfis foram removidos do público-alvo, verifique a **Logs de entrega**. Saiba mais [nesta seção](#check-control-group).


