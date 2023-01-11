---
audience: end-user
title: Trabalhar com o Construtor de segmentos
description: Documentação da Web do Campaign v8
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 1%

---

# Definir um público-alvo com o construtor de regras {#segment-builder}

![](../assets/do-not-localize/badge.png)

Esta seção descreve como criar um público-alvo ao criar um novo email. O público-alvo criado só pode ser usado neste email.

O construtor de regras permite definir a população direcionada pela mensagem filtrando os dados contidos no banco de dados. Se desejar selecionar um público-alvo existente, consulte esta [seção](add-audience.md).

Para obter mais informações sobre o construtor de regras, consulte [Documentação do Serviço de segmentação](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-builder.html).

Para criar um novo público-alvo ao criar um email, siga estas etapas:

1. No **Público** seção do assistente de criação de delivery, clique no link **[!UICONTROL Seleção do público-alvo]** botão.

   ![](assets/segment-builder0.png)

1. Selecionar **Crie seu próprio**. O construtor de regras é exibido.

   ![](assets/segment-builder.png)

## A paleta

A paleta, localizada no lado esquerdo, contém todos os elementos que podem ser filtrados para criar o público-alvo. Os blocos contidos na paleta devem ser movidos para a tela central para serem configurados e considerados. A paleta é dividida em duas guias:

* **Atributos**: essa guia permite acessar todos os campos disponíveis no schema. A lista de campos depende do schema de direcionamento definido no template de email.

   ![](assets/segment-builder2.png){width="70%" align="left"}

* **Públicos-alvo**: essa guia permite filtrar usando um dos públicos-alvo existentes definidos no console do Campaign Classic ou do Adobe Experience Platform.

   ![](assets/segment-builder3.png){width="70%" align="left"}

   >[!NOTE]
   >
   >Para aproveitar os públicos-alvo do Adobe Experience Platform, é necessário configurar a integração com Destinos. Consulte a [Documentação de destinos](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=pt-BR).

Você pode usar a barra de pesquisa para localizar elementos rapidamente.

## A tela

A tela é a zona central na qual você pode configurar e combinar regras com base nos elementos adicionados da paleta. Para adicionar uma nova regra, arraste um bloco da paleta e solte-o na tela. Em seguida, você verá opções específicas do contexto de acordo com o tipo de dados que está sendo adicionado.

![](assets/segment-builder4.png){width="70%" align="left"}

## O painel de propriedades da regra

No lado direito, a variável **Propriedades da regra** permite executar as seguintes ações:

![](assets/segment-builder5.png){width="70%" align="left"}

* **Ver resultados:** exibe a lista de recipients direcionados pelo público-alvo
* **Visualização de código**: exibe uma versão baseada em código do público-alvo no SQL.
* **Exibir atributos avançados**: marque esta opção se quiser exibir a lista completa de atributos na paleta esquerda: nós, agrupamentos, links 1-1, links 1-N.
* **Atributos**: exibe uma descrição do público-alvo criado.

## Exemplo

Neste exemplo, criaremos um público-alvo para direcionar todos os clientes que moram em Atlanta ou Seattle e nascem depois de 1980.

1. No **Atributos** da paleta, procure pela guia **Data de nascimento** campo. Arraste o bloco e solte-o na tela.

   ![](assets/segment-builder6.png)

1. Na tela, escolha a **Depois** e insira a data desejada.

   ![](assets/segment-builder7.png)

1. Na paleta, procure a variável **Cidade** e adicione-o à tela abaixo da primeira regra.

   ![](assets/segment-builder8.png)

1. No campo de texto, digite o nome da cidade e pressione enter.

   ![](assets/segment-builder9.png)

1. Repita essa ação para o nome da segunda cidade.

   ![](assets/segment-builder10.png)

1. Clique em **Exibir resultados** para exibir a lista e o número de recipients correspondentes ao query. Também é possível adicionar colunas para visualizar e verificar os dados. No nosso exemplo, adicione a variável **Cidade** e devem ver Atlanta e Seattle.

   ![](assets/segment-builder11.png)

1. Clique em **Confirm**.

Seu público-alvo está definido e pronto para ser usado em seu email.