---
audience: end-user
title: Crie um público com o construtor de regras do Campaign
description: Saiba como trabalhar com o construtor de regras
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: 9992ae7007b5af80e927dd96b6fff25840d8c3e1
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 60%

---

# Trabalhar com o construtor de regras {#segment-builder}


O construtor de regras permite definir a população direcionada pelo delivery filtrando os dados contidos no banco de dados. É possível usá-lo para criar um público-alvo a partir de um fluxo de trabalho usando um **[!UICONTROL Criar público-alvo]** ou diretamente ao criar um delivery para criar um público-alvo único.

* [Saiba como criar um público-alvo](create-audience.md)
* [Saiba como criar um público-alvo único para uma entrega](one-time-audience.md)

## A paleta

A paleta, localizada no lado esquerdo, contém todos os elementos que podem ser filtrados para criar o público-alvo. Você pode usar a barra de pesquisa para localizar elementos rapidamente. Os blocos gráficos contidos na paleta devem ser movidos para a tela central para serem configurados e considerados.

![](assets/segment-builder2.png){width="70%" align="left"}

A paleta é dividida em duas guias:

* **Atributos**: essa guia permite acessar todos os campos disponíveis no schema. A lista de campos depende do schema de direcionamento definido no template de email.

* **Públicos-alvo**: essa guia permite filtrar usando um dos públicos-alvo existentes definidos no console Campaign Classic ou no Adobe Experience Platform. [Saiba como monitorar e gerenciar públicos](manage-audience.md)

  >[!NOTE]
  >
  >Para aproveitar os públicos-alvo da Adobe Experience Platform, é necessário configurar a integração com o serviço de Destinos. Consulte a [Documentação de destinos do Adobe Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR){target="_blank"}.

## A tela

A tela é a área central onde você pode configurar e combinar regras com base nos elementos adicionados da paleta. Para adicionar uma nova regra, arraste um bloco da paleta e solte-o na tela. Você pode receber opções específicas do contexto, de acordo com o tipo de dado que está sendo adicionado.

![](assets/segment-builder4.png){width="70%" align="left"}

## O painel de propriedades da regra

No lado direito, a variável **Propriedades da regra** permite executar as ações listadas abaixo.

![](assets/segment-builder5.png){width="70%" align="left"}

* **Exibir resultados:** exibe a lista de recipients direcionados pelo público-alvo.
* **Visualização de código**: exibe uma versão baseada em código do público-alvo em SQL.
* **Exibir atributos avançados**: marque esta opção se quiser exibir a lista completa de atributos na paleta esquerda: nós, agrupamentos, links 1-1, links 1-N.
* **Calcular**: atualiza e exibe o número de perfis segmentados pelo seu query.
* **Selecionar ou salvar filtro**: use um filtro predefinido para filtrar sua consulta ou salve a consulta como um novo filtro para reutilização futura. [Saiba como trabalhar com filtros predefinidos](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Nessa versão do produto, alguns filtros predefinidos não estão disponíveis na interface. Você ainda pode usá-los. [Saiba mais](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Atributos**: exibe uma descrição do público-alvo criado.

## Exemplo

Neste exemplo, criamos um público-alvo para direcionar todos os clientes que moram em Atlanta ou Seattle e nasceram depois de 1980.

1. Na guia **Atributos** da paleta, procure pelo campo **Data de nascimento**. Arraste o bloco e solte-o na tela.

   ![](assets/segment-builder6.png)

1. Na tela, escolha o operador **Após** e insira a data desejada.

   ![](assets/segment-builder7.png)

1. Na paleta, procure o campo **Cidade** e adicione-o na tela abaixo da primeira regra.

   ![](assets/segment-builder8.png)

1. No campo de texto, digite o nome da cidade e pressione Enter.

   ![](assets/segment-builder9.png)

1. Repita essa ação para o nome da segunda cidade.

   ![](assets/segment-builder10.png)

1. Clique em **Exibir resultados** para exibir a lista e o número de recipients correspondentes à consulta. Também é possível adicionar colunas para visualizar e verificar os dados. No nosso exemplo, adicione a coluna **Cidade** e as opções Atlanta e Seattle deverão ser exibidas.

   ![](assets/segment-builder11.png)

1. Clique em **Confirmar**.