---
audience: end-user
title: Crie um público com o construtor de regras do Campaign
description: Saiba como trabalhar com o construtor de regras
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 57%

---

# Trabalhar com o construtor de regras {#segment-builder}

O construtor de regras permite definir a população direcionada pelo delivery filtrando os dados contidos no banco de dados. Você pode usá-lo para criar um público-alvo a partir de um fluxo de trabalho usando uma atividade **[!UICONTROL Criar público-alvo]** ou diretamente ao criar uma entrega para criar um público-alvo único.

* [Saiba como criar e salvar um público-alvo](create-audience.md)
* [Saiba como criar um público-alvo único para uma entrega](one-time-audience.md)

## A paleta

A paleta, localizada no lado esquerdo, contém todos os elementos que podem ser filtrados para criar o público-alvo. Você pode usar a barra de pesquisa para localizar elementos rapidamente. Os blocos gráficos contidos na paleta devem ser movidos para a tela central para serem configurados e considerados.

![](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

A paleta é dividida em duas guias:

* **Atributos**: essa guia permite acessar todos os campos disponíveis no schema. A lista de campos depende do schema de direcionamento definido no template de email.

* **Públicos-alvo**: esta guia permite filtrar usando um dos públicos-alvo existentes definidos no console de Campaign Classic ou no Adobe Experience Platform. Saiba como monitorar e gerenciar públicos [nesta seção](manage-audience.md)

  >[!NOTE]
  >
  >Para aproveitar os públicos-alvo da Adobe Experience Platform, é necessário configurar a integração com o serviço de Destinos. Consulte a [documentação de Destinos do Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR){target="_blank"}.

## A tela

A tela é a área central onde você pode configurar e combinar regras com base nos elementos adicionados da paleta. Para adicionar uma nova regra, arraste um bloco da paleta e solte-o na tela. Você pode receber opções específicas do contexto, de acordo com o tipo de dado que está sendo adicionado.

![](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## O painel de propriedades da regra

No lado direito, o painel **Propriedades da regra** permite executar as ações listadas abaixo.

![](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"}

* **Exibir resultados:** exibe a lista de perfis segmentados pelo público-alvo.
* **Visualização de código**: exibe uma versão baseada em código do público-alvo em SQL.
* **Exibir atributos avançados**: marque esta opção se quiser exibir a lista completa de atributos na paleta esquerda: nós, agrupamentos, links 1-1, links 1-N.
* **Calcular**: atualiza e exibe o número de perfis segmentados por sua consulta.
* **Selecionar ou salvar filtro**: use um filtro predefinido para filtrar sua consulta ou salve sua consulta como um novo filtro para reutilização futura. [Saiba como trabalhar com filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Nessa versão do produto, alguns filtros predefinidos não estão disponíveis na interface. Você ainda pode usá-los. [Saiba mais](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Atributos**: exibe uma descrição do público-alvo criado.

## Exemplo

Neste exemplo, criamos um público-alvo para direcionar todos os clientes que moram em Atlanta ou Seattle e nasceram depois de 1980.

1. Na guia **Atributos** da paleta, procure pelo campo **Data de nascimento**. Arraste o bloco e solte-o na tela.

   ![](assets/segment-builder6.png){zoomable="yes"}

1. Na tela, escolha o operador **Após** e insira a data desejada.

   ![](assets/segment-builder7.png){zoomable="yes"}

1. Na paleta, procure o campo **Cidade** e adicione-o na tela abaixo da primeira regra.

   ![](assets/segment-builder8.png){zoomable="yes"}

1. No campo de texto, digite o nome da cidade e pressione Enter.

   ![](assets/segment-builder9.png){zoomable="yes"}

1. Repita essa ação para o nome da segunda cidade.

   ![](assets/segment-builder10.png){zoomable="yes"}

1. Clique em **Exibir resultados** para exibir a lista e o número de destinatários correspondentes à consulta. Também é possível adicionar colunas para visualizar e verificar os dados. No nosso exemplo, adicione a coluna **Cidade** e as opções Atlanta e Seattle deverão ser exibidas.

   ![](assets/segment-builder11.png){zoomable="yes"}

1. Clique em **Confirmar**.