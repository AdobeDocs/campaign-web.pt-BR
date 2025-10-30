---
audience: end-user
title: Definir um grupo de controle
description: Saiba como definir um grupo de controle para suas mensagens na interface da Web do Campaign
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 22%

---

# Definir um grupo de controle {#control-group}

Um grupo de controle é uma subpopulação excluída da entrega. Você pode definir um grupo de controle para evitar o envio de mensagens para uma parte do público-alvo e comparar o comportamento após o delivery com o público-alvo principal. Essa opção ajuda a medir o impacto da campanha.

➡️ [Conheça este recurso no vídeo](create-audience.md#video)

## Habilitar grupo de controle {#add-a-control-group}

Para adicionar um grupo de controle, habilite a opção ao definir o público do seu delivery. O grupo de controle pode ser extraído aleatoriamente do target principal ou selecionado de uma população específica. Consequentemente, há duas formas principais de definir um grupo de controle:

* Extrair vários perfis do público-alvo principal.
* Excluir alguns perfis de uma lista ou com base nos critérios definidos em uma query.

Você pode combinar ambos os métodos ao definir um grupo de controle.

Todos os perfis incluídos no grupo de controle na etapa de preparação do delivery são removidos do público-alvo principal. Eles não recebem a mensagem.

>[!CAUTION]
>
>Não é possível usar grupos de controle ao carregar a população alvo [a partir de um arquivo externo](file-audience.md).

Para adicionar um grupo de controle a uma entrega, ative o botão de alternância **[!UICONTROL Habilitar grupo de controle]** na seção **Público-alvo** da tela de criação da entrega.

![Habilitar opção de grupo de controle na tela de criação de entrega](assets/control-group1.png)

## Extrair do público-alvo {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Modo de extração"
>abstract="Um grupo de controle é um conjunto de perfis excluídos da entrega. Para definir um grupo de controle, você pode optar por extrair, aleatoriamente ou com base em uma classificação, uma porcentagem ou um número fixo de perfis da população de destino."

### Criar um grupo de controle {#build-extract-target}

Para definir um grupo de controle, escolha extrair, aleatoriamente ou com base em uma classificação, uma porcentagem ou um número fixo de perfis da população do público-alvo. Se estiver adicionando uma população extra, escolha a opção **Sem extração** e selecione a população extra [conforme detalhado aqui](#extra-population).

Primeiro, defina como os perfis são extraídos do público-alvo: aleatoriamente ou com base em uma classificação.

Na seção **Grupo de controle**, escolha um **Modo de extração**:

* **Aleatório**: ao preparar a entrega, o Adobe Campaign extrai aleatoriamente um número de perfis correspondente à porcentagem ou ao número máximo definido como o limite de tamanho.
* **Classificado por atributo(s)**: essa opção exclui um conjunto de perfis com base em atributos específicos em uma ordem de classificação específica.

Em seguida, use a seção **Limite de tamanho** para definir o número de perfis a serem extraídos do público-alvo principal. Pode ser um número bruto (por exemplo, 50 perfis a serem excluídos) ou uma porcentagem do público inicial (por exemplo, 5% do público-alvo principal).

### Amostra do grupo de controle {#control-group-sample}

Por exemplo, para criar um grupo de controle com os 100 perfis mais novos, siga estas etapas:

1. Selecione o campo **Idade** como um critério de classificação. Deixe a opção de classificação **Crescente**.
1. Adicione o campo **Data de Criação**. Altere para a opção de classificação **Decrescente**.
1. Defina 100 como o limite na seção **Limite de tamanho**.

   ![Configuração do grupo de controle para os perfis mais jovens](assets/control-group2.png){zoomable="yes"}

Esses 100 perfis mais jovens são excluídos do público-alvo principal.

### Verifique seu grupo de controle {#check-control-group}

Visualize os logs para verificar e identificar os perfis excluídos. Por exemplo, considere uma exclusão aleatória de cinco perfis.

![Exemplo de perfis excluídos em logs](assets/control-group4.png){zoomable="yes"}

Após a preparação do delivery, analise como as exclusões foram aplicadas:

* No painel de entrega, antes de enviar, marque o KPI **To exclude**.

  ![Painel de entrega mostrando o KPI &quot;A ser excluído&quot;](assets/control-group5.png){zoomable="yes"}

* Nos logs do delivery, a guia Logs mostra a etapa de exclusão.

  ![Logs de entrega mostrando a etapa de exclusão](assets/control-group-sample-logs.png){zoomable="yes"}

<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}

-->

* A guia **Causas de exclusão** exibe o número de perfis excluídos para cada regra de tipologia.

  ![A guia Exclusion causes mostra exclusões de regra de tipologia](assets/control-group7.png){zoomable="yes"}

Para obter mais informações sobre logs de entrega, consulte esta [seção](../monitor/delivery-logs.md).

## Adicionar uma população extra {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="População extra"
>abstract="Um grupo de controle é um conjunto de perfis excluídos da entrega. É possível excluir uma população específica do público-alvo da entrega selecionando um público-alvo já existente ou definindo uma consulta."

Outra maneira de definir um grupo de controle é selecionar uma população específica em um público-alvo existente ou definir um query.

Na seção **População extra** do **Grupo de controle** na tela de definição, clique no botão **[!UICONTROL Selecionar público-alvo]**.

![Tela de seleção de população extra](assets/control-group3.png){zoomable="yes"}

* Para usar um público existente, clique em **Selecionar público-alvo**. Saiba mais [nesta seção](add-audience.md).
* Para definir uma nova consulta, selecione **Criar sua própria** e defina os critérios de exclusão usando o modelador de consultas. Saiba mais [nesta seção](../query/query-modeler-overview.md).

Os perfis incluídos na audiência ou que correspondem ao resultado da consulta foram **excluídos** do público-alvo da entrega. Eles não recebem nenhuma mensagem.

## Comparar os resultados {#control-group-results}

Depois que o delivery for enviado, extraia os logs de envio para comparar o comportamento entre os perfis que não receberam a comunicação e o público-alvo efetivo. Use os logs do delivery para criar um novo direcionamento.

Para ver quais perfis foram removidos do destino, verifique os **Logs de entrega**. Saiba mais [nesta seção](#check-control-group).