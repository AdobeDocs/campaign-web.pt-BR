---
audience: end-user
title: Utilização da atividade de workflow Divisão
description: Saiba como usar a atividade de workflow Divisão
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 72%

---

# Divisão {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Atividade Divisão"
>abstract="A atividade **Divisão** permite segmentar as populações recebidas em vários subconjuntos com base em diferentes critérios de seleção, como regras de filtragem ou tamanho da população."

A atividade **Split** é uma atividade de **Direcionamento** que segmenta as populações que entram em vários subconjuntos com base em critérios de seleção diferentes, como regras de filtragem ou tamanho de população.

## Configurar a atividade de divisão {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segmentos para a atividade de divisão"
>abstract="Adicione quantos subconjuntos desejar para segmentar a população recebida. Quando a Atividade de **divisão** é executada, a população é segmentada nos diferentes subconjuntos na ordem em que são adicionados à atividade. Antes de iniciar o fluxo de trabalho, certifique-se de ter ordenado os subconjuntos na ordem que atenda às suas necessidades usando os botões de seta."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Filtro da atividade de divisão"
>abstract="Para aplicar uma condição de filtragem ao subconjunto, clique em **[!UICONTROL Criar filtro]** e configure a regra de filtragem desejada usando o modelador de consultas. Por exemplo, inclua perfis da população recebida cujo endereço de email já exista no banco de dados."
>additional-url="https://experienceleague.adobe.com/pt-br/docs/campaign-web/v8/query-database/query-modeler-overview" text="Trabalhar com o modelador de consultas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Limite da atividade de divisão"
>abstract="Para limitar o número de perfis selecionados pelo subconjunto, ative a opção **[!UICONTROL Habilitar limite]**, e especifique o número ou as porcentagens da população a serem incluídas."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Classificação da atividade de divisão"
>abstract="Ao definir um limite de população para um subconjunto, é possível classificar os perfis selecionados com base em um atributo de perfil específico, em ordem crescente ou decrescente. Para fazer isso, ative a opção **Habilitar classificação**. Por exemplo, é possível restringir um subconjunto para incluir apenas os 50 perfis com o valor de compra mais alto."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Complemento de geração de divisão"
>abstract="Após configurar todos os subconjuntos, é possível selecionar a população restante que não correspondeu a nenhum dos subconjuntos e incluí-la em uma transição de saída adicional. Para fazer isso, ative a opção **Gerar complemento**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Gerar todos os subconjuntos na mesma tabela"
>abstract="Ative essa opção para agrupar todos os subconjuntos em uma única transição de saída."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Ignorar transição vazia"
>abstract="Ative a opção **[!UICONTROL Ignorar transição vazia]** para desabilitar a transição de saída para este subconjunto se a população de entrada estiver vazia."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="Habilitar sobreposição de populações de saída"
>abstract="A opção **[!UICONTROL Habilitar sobreposição de populações de saída]** permite gerenciar populações pertencentes a vários subconjuntos. Quando a caixa não está marcada, a atividade de divisão garante que um destinatário não possa estar presente em diversas transições de saída, mesmo que atenda aos critérios de vários subconjuntos. Eles estarão no público-alvo da primeira guia com critérios correspondentes. Quando a caixa for marcada, os destinatários poderão ser encontrados em vários subconjuntos se atenderem aos critérios de filtro. O Adobe Campaign recomenda usar critérios exclusivos."

Siga estas etapas para configurar a atividade de **Divisão**:

1. Adicione uma atividade de **Divisão** ao seu workflow.

1. O painel de configuração da atividade é aberto com um subconjunto padrão. Clique em **Adicionar segmento** para adicionar quantos subconjuntos desejar e segmentar a população recebida.

   ![Painel de configuração da atividade dividida mostrando subconjuntos](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Quando a Atividade de **divisão** é executada, a população é segmentada nos diferentes subconjuntos na ordem em que são adicionados à atividade. Por exemplo, se o primeiro subconjunto recuperar 70% da população inicial, o próximo subconjunto adicionado aplicará seus critérios de seleção somente aos 30% restantes e assim por diante.
   >
   >Antes de iniciar o fluxo de trabalho, verifique se você ordenou os subconjuntos na ordem que atende às suas necessidades. Use os botões de seta para alterar a posição de um subconjunto.

1. Após a adição dos subconjuntos, a atividade mostrará tantas transições de saída quanto houver subconjuntos. Altere o rótulo de cada subconjunto para identificá-los facilmente na tela do workflow.

1. Configure como cada subconjunto filtra a população recebida. Siga estas etapas:

   1. Abra o subconjunto para exibir suas propriedades.

   1. Para aplicar uma condição de filtragem ao subconjunto, clique em **[!UICONTROL Criar filtro]** e configure a regra de filtragem desejada usando o modelador de consultas. Por exemplo, inclua perfis da população recebida cujo endereço de email exista no banco de dados. [Saiba como trabalhar com o modelador de consultas](../../query/query-modeler-overview.md).

   1. Para limitar o número de perfis selecionados pelo subconjunto, ative a opção **[!UICONTROL Habilitar limite]**, e especifique o número ou as porcentagens da população a serem incluídas.

   1. Para desabilitar uma transição se a população recebida estiver vazia, alterne a opção **[!UICONTROL Ignorar transição vazia]** para. Se nenhum perfil corresponder ao subconjunto, o workflow não fará transição para a próxima atividade.

      ![Painel de configuração do subconjunto mostrando as opções de filtragem e classificação](../assets/workflow-split-subset.png)

      >[!NOTE]
      >
      >Ao definir um limite de população para um subconjunto, você pode classificar os perfis selecionados com base em um [atributo de perfil](../../get-started/attributes.md) específico, em ordem crescente ou decrescente. Para fazer isso, ative a opção **[!UICONTROL Habilitar classificação]**. Por exemplo, é possível restringir um subconjunto para incluir apenas os 50 perfis com o valor de compra mais alto.

1. Após configurar todos os subconjuntos, é possível selecionar a população restante que não correspondeu a nenhum dos subconjuntos e incluí-la em uma transição de saída adicional. Para fazer isso, ative a opção **[!UICONTROL Gerar complemento]**.

   ![Painel de configuração de transição de complemento](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >A opção **[!UICONTROL Generate all subsets in the same table]** permite agrupar todos os subconjuntos em uma única transição de saída.

1. A opção **[!UICONTROL Enable overlapping of output populations]** permite gerenciar populações pertencentes a vários subconjuntos:

   * Quando a caixa não está marcada, a atividade de divisão garante que um destinatário não possa estar presente em diversas transições de saída, mesmo que atenda aos critérios de vários subconjuntos. Eles estarão no target da primeira guia com critérios correspondentes.
   * Quando a caixa for marcada, os destinatários poderão ser encontrados em vários subconjuntos se atenderem aos critérios de filtro. O Adobe Campaign recomenda usar critérios exclusivos.

A atividade agora está configurada. Na execução do workflow, a população segmenta nos diferentes subconjuntos na ordem em que foram adicionados à atividade.

## Exemplo {#split-example}

No exemplo a seguir, a atividade **[!UICONTROL Split]** segmenta um público em subconjuntos distintos com base no canal de comunicação a ser usado:

* **Subconjunto 1 &quot;push&quot;**: esse subconjunto compreende todos os perfis que instalaram o aplicativo móvel.
* **Subconjunto 2 &quot;sms&quot;**: usuários de telefone celular: para a população restante que não se enquadra no Subconjunto 1, o Subconjunto 2 aplica uma regra de filtragem para selecionar perfis com telefones celulares no banco de dados.
* **Transição de complemento**: essa transição captura todos os perfis restantes que não corresponderam ao subconjunto 1 nem ao subconjunto 2. Especificamente, inclui perfis que não instalaram o aplicativo móvel nem possuem um telefone celular, como usuários que não instalaram o aplicativo ou que não têm um número de celular registrado.

![Exemplo de uma atividade Split com subconjuntos e transição de complemento](../assets/workflow-split-example.png)