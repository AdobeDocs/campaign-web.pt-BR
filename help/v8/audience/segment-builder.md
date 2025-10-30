---
audience: end-user
title: Crie um público com o construtor de regras do Campaign
description: Saiba como trabalhar com o construtor de regras
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 24%

---

# Trabalhar com o construtor de regras {#segment-builder}

O construtor de regras permite que você defina a população direcionada pelo delivery filtrando os dados contidos no banco de dados. Use-a para criar um público-alvo a partir de um fluxo de trabalho usando uma atividade **[!UICONTROL Criar público-alvo]** ou diretamente ao criar uma entrega para criar um público-alvo único.

* [Saiba como criar e salvar um público-alvo](create-audience.md)
* [Saiba como criar um público-alvo único para uma entrega](one-time-audience.md)

## A paleta

A paleta, localizada no lado esquerdo, contém todos os elementos que você pode filtrar para criar seu público-alvo. Use a barra de pesquisa para localizar elementos rapidamente. Mova os blocos gráficos contidos na paleta para a tela central para configurá-los e levá-los em consideração.

![A interface da paleta mostrando opções e guias de filtragem](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

A paleta é dividida em duas guias:

* **Atributos**: esta guia fornece acesso a todos os campos disponíveis do esquema. A lista de campos depende do esquema de direcionamento definido no modelo de email.

* **Públicos-alvo**: essa guia permite filtrar usando um dos públicos-alvo existentes definidos no console do Campaign Classic ou no Adobe Experience Platform. Saiba como monitorar e gerenciar públicos-alvo no [nesta seção](manage-audience.md).

  >[!NOTE]
  >
  >Para usar os públicos da Adobe Experience Platform, configure a integração com os Destinos. Consulte a [documentação de Destinos do Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR){target="_blank"}.

## A tela

A tela é a zona central onde você pode configurar e combinar regras com base nos elementos adicionados da paleta. Para adicionar uma nova regra, arraste um bloco da paleta e solte-o na tela. As opções específicas do contexto são apresentadas com base no tipo de dados que está sendo adicionado.

![A interface da tela mostrando as opções de configuração da regra](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## O painel de propriedades da regra

No lado direito, o painel **Propriedades da regra** permite executar as ações listadas abaixo.

![O painel de propriedades da regra mostrando as ações disponíveis](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Exibir resultados:** Exibe a lista de perfis segmentados pelo público-alvo.
* **Visualização de código**: mostra uma versão baseada em código da audiência no SQL.
* **Exibir atributos avançados**: marque esta opção para exibir a lista completa de atributos na paleta esquerda, incluindo nós, agrupamentos, links 1-1 e links 1-N.
* **Calcular**: atualiza e exibe o número de perfis segmentados por sua consulta.
* **Selecionar ou salvar filtro**: use um filtro predefinido para filtrar sua consulta ou salve sua consulta como um novo filtro para reutilização futura. [Saiba como trabalhar com filtros predefinidos](../get-started/predefined-filters.md).

  >[!IMPORTANT]
  >
  >Nesta versão do produto, alguns filtros predefinidos não estão disponíveis na interface. Você ainda pode usá-los. [Saiba mais](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **Atributos**: exibe uma descrição do público-alvo criado.

## Exemplo

Neste exemplo, um público-alvo é criado para direcionar todos os clientes que moram em Atlanta ou Seattle e nascem após 1980.

1. Na guia **Atributos** da paleta, procure pelo campo **Data de nascimento**. Arraste o bloco e solte-o na tela.

   ![Adicionando o campo Data de nascimento à tela](assets/segment-builder6.png){zoomable="yes"}

1. Na tela, escolha o operador **Após** e insira a data desejada.

   ![Configurando o operador After para o campo Data de nascimento](assets/segment-builder7.png){zoomable="yes"}

1. Na paleta, procure o campo **Cidade** e adicione-o na tela abaixo da primeira regra.

   ![Adicionando o campo Cidade à tela](assets/segment-builder8.png){zoomable="yes"}

1. No campo de texto, digite o nome da cidade e pressione Enter.

   ![Inserindo o primeiro nome de cidade no campo Cidade](assets/segment-builder9.png){zoomable="yes"}

1. Repita essa ação para o nome da segunda cidade.

   ![Inserindo o nome da segunda cidade no campo Cidade](assets/segment-builder10.png){zoomable="yes"}

1. Clique em **Exibir resultados** para exibir a lista e o número de destinatários correspondentes à consulta. Adicione colunas para visualizar e verificar os dados. Neste exemplo, adicione a coluna **Cidade** para ver Atlanta e Seattle.

   ![Exibindo resultados com a coluna Cidade adicionada](assets/segment-builder11.png){zoomable="yes"}

1. Clique em **Confirmar**.