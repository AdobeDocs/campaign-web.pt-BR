---
audience: end-user
title: Trabalhar com o modelador de consultas
description: Saiba como trabalhar com o modelador de consultas à Web do Adobe Campaign.
badge: label="Disponibilidade limitada"
source-git-commit: 9c72d73b5279a01492ea3ccd295e513e91f0c050
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 39%

---

# Trabalhar com o modelador de consultas {#segment-builder}


>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Novo modelador de consultas"
>abstract="O Adobe Campaign Web apresenta um modelador de consultas que simplifica o processo de filtragem de bancos de dados, selecionando itens específicos com base em vários critérios. Isso inclui o uso de expressões e operadores avançados. O modelador de consulta está disponível em todo contexto onde é preciso definir regras para filtrar dados."

<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Novo modelador de consultas"
>abstract="O Adobe Campaign Web apresenta um modelador de consultas que simplifica o processo de filtragem de bancos de dados, selecionando itens específicos com base em vários critérios. Isso inclui o uso de expressões e operadores avançados. O modelador de consulta está disponível em todo contexto onde é preciso definir regras para filtrar dados."

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Modelador de consulta"
>abstract="Defina os critérios de filtragem para destinatários ou qualquer outra dimensão de direcionamento do banco de dados. Aproveite o público da Adobe Experience Platform para refinar ainda mais o seu público-alvo e maximizar o impacto da campanha."

O Adobe Campaign Web apresenta um modelador de consultas que simplifica o processo de filtragem de bancos de dados, selecionando itens específicos com base em vários critérios. Isso inclui o uso de expressões e operadores avançados.

## Acessar o modelador de consultas

O modelador de consulta está disponível em todo contexto onde é preciso definir regras para filtrar dados.

| Uso | Exemplo |
|  ---  |  ---  |
| **Definir públicos**: especifique a população que deseja direcionar em suas mensagens ou fluxos de trabalho e crie facilmente novos públicos-alvo personalizados para suas necessidades. | ![](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **Personalizar atividades de fluxo de trabalho**: aplique regras em atividades de workflow, como Split e Reconciliation, para alinhar-se aos requisitos específicos. | ![](assets/access-workflow.png){width="200" align="center" zoomable="yes"} |
| **Filtros predefinidos**: crie filtros predefinidos que servem como atalhos durante várias operações de filtragem, independentemente de você estar trabalhando com listas de dados ou formando o público para um delivery. | ![](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **Filtrar dados de relatórios**: adicione uma regra para filtrar os dados exibidos nos relatórios. | ![](assets/access-reports.png){width="200" align="center" zoomable="yes"} |
| **Personalizar listas**: crie regras personalizadas para filtrar os dados exibidos em listas como recipients, listas de deliveries, etc. | ![](assets/access-lists.png){width="200" align="center" zoomable="yes"} |

<!--**Dynamize content**: make your content dynamic by creating conditions that define which content should be displayed to different recipients, ensuring personalized and relevant messaging.

+++Example

![](assets/access-audience.png)

 +++
-->

## Interface do modelador de consultas {#interface}

O modelador de consultas fornece uma tela central onde você cria a consulta e um painel direito fornecendo informações sobre a consulta.

![](assets/query-interface.png)

### A tela central {#canvas}

A tela central do modelador de consultas é onde você adiciona e combina os diferentes componentes que constroem sua consulta. [Saiba como criar uma consulta](build-query.md)

A barra de ferramentas localizada no canto superior direito da tela fornece opções para manipular facilmente os componentes da consulta e navegar na tela:

* **Modo de seleção múltipla**: selecione vários componentes de filtragem para copiá-los e colá-los no local de sua escolha.
* **Girar**: Alterne a tela de desenho verticalmente.
* **Ajustar à tela**: adapte o nível de zoom da tela de desenho à sua tela.
* **Menos zoom** / **Mais zoom**: Reduza ou na tela de desenho.
* **Exibir mapa**: abre um instantâneo da tela mostrando que você está localizado.

### O painel de propriedades Regra {#rule-properties}

No lado direito, a variável **[!UICONTROL Propriedades da regra]** fornece informações sobre a consulta. Ela permite executar várias operações para verificar a consulta e garantir que ela atenda às suas necessidades. [Saiba como verificar e validar seu query](build-query.md#check-and-validate-your-query)
