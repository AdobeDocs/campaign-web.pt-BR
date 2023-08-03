---
audience: end-user
title: Utilização da atividade de workflow Divisão
description: Saiba como usar a atividade de workflow Divisão
badge: label="Alfa"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 100%

---


# Divisão {#split}

A atividade de **Divisão** é uma atividade de **Direcionamento** que permite segmentar as populações recebidas em vários subconjuntos com base em diferentes critérios de seleção, como regras de filtragem ou tamanho da população.

## Configuração {#general}

Siga estas etapas para configurar a atividade de **Divisão**:

1. Adicione uma atividade de **Divisão** ao seu workflow.

1. O painel de configuração da atividade é aberto com um subconjunto padrão. Clique em **Adicionar segmento** para adicionar quantos subconjuntos desejar e segmentar a população recebida.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Quando a atividade de Divisão é executada, a população é segmentada nos diferentes subconjuntos na ordem em que são adicionados à atividade. Por exemplo, se o primeiro subconjunto recuperar 70% da população inicial, o próximo subconjunto adicionado aplicará seus critérios de seleção somente aos 30% restantes e assim por diante.
   >
   > Antes de configurar os subconjuntos, verifique se eles foram adicionados na ordem correta, pois sua posição não pode ser alterada.

1. Após a adição dos subconjuntos, a atividade mostrará tantas transições de saída quanto houver subconjuntos. Recomendamos alterar o rótulo de cada subconjunto para identificá-los facilmente na tela de workflow.

1. Configure como cada subconjunto deve filtrar a população recebida. Para fazer isso, siga estes passos:

   1. Abra o subconjunto para exibir suas propriedades.

   1. Para aplicar uma condição de filtragem ao subconjunto, clique em **[!UICONTROL Criar filtro]** e configure a regra de filtragem desejada. Por exemplo, inclua perfis da população recebida cujo endereço de email já exista no banco de dados.

   1. Para limitar o número de perfis selecionados pelo subconjunto, ative a opção **[!UICONTROL Habilitar limite]**, e especifique o número ou as porcentagens da população a serem incluídas.

      >[!NOTE]
      >
      >Ao definir um limite de população para um subconjunto, é possível classificar os perfis selecionados com base em um atributo de perfil específico, em ordem crescente ou decrescente. Para fazer isso, ative a opção **[!UICONTROL Habilitar classificação]**. Por exemplo, é possível restringir um subconjunto para incluir apenas os 50 perfis com o valor de compra mais alto.

   ![](../assets/workflow-split-subset.png)

1. Após configurar todos os subconjuntos, é possível selecionar a população restante que não correspondeu a nenhum dos subconjuntos e incluí-la em uma transição de saída adicional. Para fazer isso, ative a opção **[!UICONTROL Gerar complemento]**.

   ![](../assets/workflow-split-complement.png)

A atividade agora está configurada. Na execução do workflow, a população será segmentada nos diferentes subconjuntos, na ordem em que foram adicionados à atividade.

## Exemplo

No exemplo a seguir, a atividade de **[!UICONTROL Divisão]** é usada para segmentar um público-alvo em subconjuntos distintos com base no canal de comunicação que queremos usar:

* **Subconjunto 1 “push”**: esse subconjunto inclui todos os perfis que instalaram nosso aplicativo móvel.
* **Subconjunto 2 “sms”**: usuários de celular: para a população restante que não se enquadrou no subconjunto 1, o subconjunto 2 aplica uma regra de filtragem para selecionar perfis com telefones celulares no banco de dados.
* **Transição de complemento**: essa transição captura todos os perfis restantes que não corresponderam ao subconjunto 1 nem ao subconjunto 2. Especificamente, inclui perfis que não instalaram o aplicativo móvel nem possuem um telefone celular, como usuários que não instalaram o aplicativo ou que não têm um número de celular registrado.

![](../assets/workflow-split-example.png)
