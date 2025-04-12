---
audience: end-user
title: Selecionar atributos e adicioná-los aos favoritos
description: Saiba como trabalhar com atributos e acessar facilmente os atributos favoritos e os usados recentemente.
exl-id: 27663e57-fdab-4371-b7c6-12064ed6526f
source-git-commit: c0c9c5da3369e55269411b7348004006cd3c139e
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 35%

---

# Selecionar atributos e adicioná-los aos favoritos {#folders}

A interface do usuário da Web do Campaign permite que os usuários selecionem atributos do banco de dados em vários locais, dependendo da ação que está sendo executada. Por exemplo, os atributos podem ser selecionados ao definir colunas de saída para um delivery de correspondência direta ou um arquivo a ser extraído. Da mesma forma, os atributos podem ser selecionados ao usar o modelador de consulta para criar regras, filtros ou públicos-alvo.

![Selecione atributos na interface do banco de dados, mostrando as opções de atributo.](assets/attributes-list.png)

Para reutilizar rapidamente os atributos usados com frequência, adicione-os aos favoritos. Isso garante que eles estejam prontamente acessíveis para tarefas futuras. Além dos favoritos, os usuários podem visualizar e usar os atributos selecionados mais recentemente.

A interface também fornece uma ferramenta de distribuição de valores, que permite visualizar a distribuição dos valores de um atributo em uma tabela. Essa ferramenta ajuda a identificar o intervalo e a frequência dos valores, garantindo a consistência dos dados ao criar consultas ou expressões.

## Favoritos e atributos recentes {#favorites}

>[!CONTEXTUALHELP]
>id="acw_attribute_picker_favorites_recents"
>title="Favoritos e recentes"
>abstract="O menu **[!UICONTROL Favoritos e recentes]** do seletor de atributos oferece uma exibição organizada dos atributos adicionados aos favoritos, juntamente com uma lista de atributos usados recentemente. Os atributos favoritos aparecem primeiro, seguidos pelos usados recentemente, facilitando a localização dos atributos necessários."

O menu **[!UICONTROL Favoritos e Recentes]** no seletor de atributos fornece uma exibição organizada dos atributos adicionados aos favoritos, juntamente com uma lista de atributos usados recentemente. Os atributos favoritos aparecem primeiro, seguido pelos usados recentemente, facilitando a localização dos atributos necessários.

![Menu de favoritos e atributos recentes, mostrando os atributos favoritos e usados recentemente.](assets/attributes-favorites.png)

Para adicionar um atributo aos favoritos, passe o mouse sobre o seu botão de informações e selecione o ícone de estrela. O atributo é adicionado automaticamente à lista de favoritos. Para remover um atributo dos favoritos, selecione o ícone de estrela novamente.

Os usuários podem adicionar até 20 atributos aos favoritos. Os atributos favoritos e recentes estão associados a cada usuário em uma organização, garantindo a acessibilidade em máquinas diferentes e fornecendo uma experiência perfeita em todos os dispositivos.

## Identificação da distribuição de valores em uma tabela {#distribution}

O botão **Distribuição de Valores**, disponível no painel de informações de um atributo, permite que os usuários analisem a distribuição de valores para esse atributo dentro da tabela. Esse recurso é útil para entender os valores disponíveis, suas contagens e porcentagens. Também ajuda a evitar problemas como capitalização ou ortografia inconsistente ao criar consultas ou criar expressões.

![Interface da ferramenta de distribuição de valores, mostrando contagens e porcentagens de valores de atributos.](assets/attributes-distribution-values.png)

Para atributos com um grande número de valores, a ferramenta exibe apenas os primeiros vinte. Nesses casos, uma notificação de **[!UICONTROL Carregamento parcial]** parece indicar essa limitação. Aplique filtros avançados para refinar os resultados exibidos e se concentrar em valores ou subconjuntos de dados específicos. Orientações detalhadas sobre o uso de filtros estão disponíveis [aqui](../get-started/work-with-folders.md#filter-the-values).

Para obter informações adicionais sobre como usar a ferramenta de distribuição de valores em contextos diferentes, consulte as seguintes seções:

* [Distribuição de valores em uma pasta](../get-started/work-with-folders.md##distribution-values-folder)
* [Distribuição de valores em uma consulta](../query/build-query.md#distribution-values-query)