---
audience: end-user
title: Criar e gerenciar públicos
description: Saiba como criar e gerenciar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
source-git-commit: ab445f332b62baa98f9f9e84a80cc336cd88efe0
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 1%

---


# Criar públicos {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="Nessa tela, você pode acessar a lista de todos os públicos-alvo que podem ser direcionados em seus deliveries. Clique em **Criar** para criar novos públicos em uma tela visual usando várias atividades de fluxo de trabalho, como **Split** ou **Excluir**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configurações do público-alvo"
>abstract="Insira o nome do público-alvo e as opções adicionais e clique no link **Criar público-alvo** botão."

O Campaign Web permite criar novos públicos-alvo em uma tela de fluxo de trabalho visual. Além de começar do zero para criar um público-alvo simples, você também pode aproveitar as atividades do fluxo de trabalho para refinar seu público-alvo. Por exemplo, você pode combinar vários públicos-alvo em um único, enriquecer o público-alvo com atributos externos ou dividi-lo em vários públicos-alvo com base em regras de sua escolha.

Depois de criar o fluxo de trabalho, os públicos resultantes são automaticamente armazenados no banco de dados do Campaign junto com os existentes. Esses públicos-alvo podem ser direcionados em campanhas ou deliveries independentes.

## Criar seu primeiro público-alvo {#create}

Para criar um público-alvo, siga estas etapas:

1. Navegue até a **[!UICONTROL Públicos-alvo]** e clique no botão **[!UICONTROL Criar público-alvo]** localizado no canto superior direito.
1. Forneça um rótulo para o público.
1. Expanda a **[!UICONTROL Opções adicionais]** seção para configurar parâmetros avançados de público-alvo.

   Por padrão, os públicos-alvo são criados na **[!UICONTROL Perfis e públicos alvo]** / **[!UICONTROL Listas]** menu do explorador. É possível alterar o local de armazenamento padrão usando o **[!UICONTROL Pasta]** campo.

   ![](assets/audiences-settings.png)

1. Depois de definir as configurações de público-alvo, clique no **[!UICONTROL Criar público-alvo]** botão. Uma tela de workflow é exibida, apresentando duas atividades padrão:

   * **[!UICONTROL Criar público-alvo]**: este é o ponto de partida do fluxo de trabalho, permitindo criar um público-alvo e usá-lo como base para ele.

   * **[!UICONTROL Salvar público-alvo]**: representa a etapa final do fluxo de trabalho, permitindo salvar os resultados do fluxo de trabalho como um novo público-alvo.

1. Abra o **[!UICONTROL Criar público-alvo]** atividade e use o construtor de regras para definir a população a ser incluída no público-alvo filtrando os dados contidos no banco de dados. [Saiba como configurar uma atividade Criar público-alvo](../workflows/activities/build-audience.md)

1. Se você quiser executar operações adicionais no público direcionado para o workflow, adicione quantas atividades forem necessárias e conecte-as. Para obter mais informações sobre como configurar atividades de workflow, consulte [documentação de workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >As atividades de canal não estão disponíveis para uso em fluxos de trabalho de público.

   ![](assets/audience-creation-canvas.png)

1. Configure o **[!UICONTROL Salvar público-alvo]** atividade para especificar como você deseja salvar a população computada upstream no workflow. [Saiba como configurar uma atividade Salvar público](../workflows/activities/save-audience.md)

1. Quando o workflow estiver pronto, clique em **[!UICONTROL Início]** para executá-lo.

O workflow é salvo na variável **[!UICONTROL Fluxos de trabalho]** lista, enquanto os públicos resultantes estão acessíveis na **[!UICONTROL Públicos-alvo]** lista.

## Exemplo de fluxo de trabalho de público {#example}

O exemplo abaixo mostra um fluxo de trabalho de público-alvo configurado para direcionar clientes do sexo feminino que moram em Nova York e criar dois novos públicos-alvo, dependendo de sua compra mais recente (Yoga ou Running gear).

![](assets/audiences-example.png)

1. A variável **[!UICONTROL Criar público-alvo]** A atividade segmenta todas as perfis femininas que vivem em Nova York.
1. A variável **[!UICONTROL Enriquecimento]** A atividade de enriquece o público-alvo com informações da tabela Purchases para identificar o tipo de produto que os clientes compraram.
1. A variável **[!UICONTROL Split]** A atividade divide o fluxo de trabalho em dois caminhos com base na compra mais recente dos clientes.
1. A variável **[!UICONTROL Salvar público-alvo]** as atividades no final de cada caminho criam dois novos públicos-alvo no banco de dados, incluindo a população calculada em cada caminho.

## Monitorar e gerenciar públicos {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Erro de público"
>abstract="Os dados do público-alvo não estão disponíveis. Aguarde o fim da execução do fluxo de trabalho."

A lista de públicos-alvo disponíveis para uso no Campaign Web pode ser acessada no **[!UICONTROL Públicos-alvo]** menu.

![](assets/audiences-list.png)

Os públicos-alvo podem se originar de várias fontes. A variável **[!UICONTROL Origem]** indica onde um determinado público-alvo foi criado:

* **[!UICONTROL Adobe Campaign]**: esses públicos-alvo são criados no console do Adobe Campaign V8. Saiba mais em [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html?lang=pt-BR){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Esses públicos-alvo são criados no Adobe Experience Platform e integrados ao Campaign Web usando a integração Adobe Fontes e Destinos. Saiba como configurar essa integração no [Documentação do Campaign v8 (console do cliente)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL WebUI do Adobe Campaign]**: esses públicos são criados usando workflows de público-alvo da Web do Campaign. [Saiba como criar públicos](create-audience.md)

Para obter mais informações sobre um público, abra-o na lista. As propriedades do público são exibidas junto com o número de perfis incluídos no público. É possível atualizar a contagem de públicos-alvo a qualquer momento usando o **[!UICONTROL Calcular]** botão.

A variável **[!UICONTROL Dados]** permite visualizar os perfis que fazem parte do público-alvo. Você pode personalizar essa visualização adicionando mais colunas ou utilizando filtros avançados para refinar os dados exibidos.

![](assets/audiences-details.png)

Para duplicar ou excluir um público-alvo, clique no **[!UICONTROL Mais ações]** botão disponível na lista públicos-alvo ao lado do nome do público-alvo ou dentro de uma tela de detalhes do público-alvo.
