---
audience: end-user
title: Trabalhar com tipologias
description: Saiba como trabalhar com tipologias e regras de tipologia para controlar, filtrar e monitorar o envio de deliveries.
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: c759dd72e2ca3d11b4dad0cd38410d699b651cad
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 8%

---

# Trabalhar com tipologias {#typologies}

>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="Tipologias e regras de tipologia"
>abstract="As tipologias permitem padronizar as práticas comerciais em todos os deliveries. Uma tipologia é uma coleção de regras de tipologia que permitem controlar, filtrar e priorizar o envio de entregas. Os perfis que correspondem aos critérios em uma regra de tipologia são excluídos dos públicos-alvo da entrega na fase de preparação."

## Sobre tipologias

As tipologias permitem padronizar as práticas comerciais em todos os deliveries. Uma **tipologia** é uma coleção de **regras de tipologia** que permitem controlar, filtrar e priorizar o envio de entregas. Os perfis que correspondem aos critérios em uma regra de tipologia são excluídos dos públicos-alvo da entrega na fase de preparação.

As tipologias garantem que seus deliveries sempre contenham determinados elementos (como um link de cancelamento de subscrição ou uma linha de assunto) ou regras de filtragem para excluir grupos do target pretendido (como clientes que não assinam, concorrentes ou clientes não fidelizados).

As tipologias podem ser acessadas pelo menu **[!UICONTROL Administração]** > **[!UICONTROL Regras de negócio]**. Nessa tela, você pode acessar todas as tipologias e regras de tipologia existentes ou criar novas com base nas suas necessidades.

![](assets/business-rules-list.png)

>[!NOTE]
>
>A lista de **[!UICONTROL Regras de tipologia]** exibe todas as regras existentes criadas até o momento na Interface do Usuário da Web ou no Console do Cliente. Entretanto, somente as regras **Controle** e **Filtragem** podem ser criadas na Interface do Usuário da Web. Para criar outros tipos de regras de tipologia, como regras de Pressão ou Capacidade, use o console do cliente do Campaign v8. [Saiba como criar regras de tipologia no console do cliente](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

As principais etapas para aplicar tipologias às suas mensagens são as seguintes:

1. [Criar uma tipologia](#typology).
1. [Criar regras de tipologia](#typology-rules).
1. [Regras de tipologia de referência na tipologia](#add-rules).
1. [Aplicar a tipologia a uma mensagem](#message).

## Criar uma tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="Propriedades de tipologia"
>abstract="Defina as propriedades da tipologia e expanda a seção **[!UICONTROL Opções adicionais]** para acessar as configurações avançadas. Use o campo **[!UICONTROL Afinidade de IP]** para associar afinidades de IP a tipologias. Isso permite controlar melhor o tráfego SMTP de saída, definindo quais endereços IP específicos podem ser usados para cada afinidade."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="Afinidade de IP"
>abstract="O gerenciamento de afinidades com endereços IP permite melhor controle do tráfego SMTP de saída, associando diferentes endereços IP a cada tipo de tráfego, dependendo da tipologia de sua ação de delivery."

Para criar uma tipologia, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Regras de negócio]** e selecione a guia **[!UICONTROL Tipologia]**.

1. Clique no botão **[!UICONTROL Criar tipologia]** e digite um **[!UICONTROL Rótulo]** para a tipologia.

1. Expanda a seção **[!UICONTROL Opções adicionais]** para definir configurações avançadas, como o nome interno da tipologia, a pasta de armazenamento e a descrição.

   ![](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >O campo **[!UICONTROL Afinidade de IP]** permite associar afinidades de IP a tipologias. Isso permite controlar melhor o tráfego SMTP de saída, definindo quais endereços IP específicos podem ser usados para cada afinidade.  Você pode, por exemplo, usar uma afinidade por país ou subdomínio. Em seguida, é possível criar uma tipologia por país e vincular cada afinidade à tipologia correspondente.

1. Clique em **[!UICONTROL Criar]** para confirmar a criação da tipologia.

A tipologia abre detalhes. Nessa tela, você pode fazer referência diretamente às regras de tipologia existentes. Você também pode criar novas regras de tipologia e referenciá-las na tipologia posteriormente:
* [Saiba como criar uma regra de tipologia](#add-rules)
* [Saiba como fazer referência a regras em uma tipologia](#add-rules)

## Criar uma regra de tipologia {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="Propriedades da regra de tipologia"
>abstract="Defina as propriedades da regra de tipologia. As regras de **Controle** verificam a qualidade e a validade da mensagem antes do envio, enquanto as regras de **Filtragem** excluem segmentos do público-alvo com base em critérios específicos.<br/><br/>Você também pode alterar a ordem de execução da regra para gerenciar a sequência em que as regras de tipologia serão executadas quando várias regras do mesmo tipo forem executadas durante a mesma fase de processamento de mensagens."

Para criar uma regra de tipologia, navegue até o menu **[!UICONTROL Regras de negócio]** e selecione a guia **[!UICONTROL Regras de tipologia]**.

Clique no botão **[!UICONTROL Criar regra de tipologia]** e siga as etapas detalhadas abaixo.

### Definir as propriedades da regra de tipologia {#properties}

Defina as propriedades da regra de tipologia:

1. Insira um **[!UICONTROL Rótulo]** para a regra.

   ![](assets/business-rules-control-rule.png)

1. Selecione o **[!UICONTROL Tipo]** da regra de tipologia:

   * **Controle**: garante a qualidade e a validade da mensagem pré-envio (por exemplo, exibição de caracteres, comprimento do SMS, formato de endereço, redução de URL). Eles são criados usando uma interface de script para definir uma lógica complexa para verificações e modificações de conteúdo.

   * As regras de **Filtragem** excluem segmentos do público-alvo com base em critérios específicos (por exemplo, idade, local, país, números de telefone). Essas regras estão vinculadas a uma targeting dimension.

   >[!NOTE]
   >
   >Por enquanto, somente as regras de tipologia **Controle** e **Filtragem** podem ser criadas a partir da Interface do Usuário da Web. Para criar outros tipos de regras, use o console do Cliente. [Saiba como criar regras de tipologia no console do cliente](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. Selecione um **[!UICONTROL Canal]** para associar à regra.

1. Desative a opção **[!UICONTROL Ativo]** se não quiser que a regra fique ativa logo após sua criação.

1. Defina a regra **[!UICONTROL Ordem de execução]**.

   Por padrão, a ordem das regras de tipologia é definida como 50. É possível adaptar esse valor para gerenciar a sequência em que as regras de tipologia serão executadas quando várias regras do mesmo tipo forem executadas durante a mesma fase de processamento de mensagens. Por exemplo, uma regra de filtragem com uma ordem de execução de 20 é executada antes de uma regra de filtragem com uma ordem de execução de 30.

1. Expanda a seção **[!UICONTROL Opções adicionais]** para acessar configurações avançadas, como o nome interno da regra, o armazenamento da pasta e a descrição.

1. Para regras de controle, duas regras adicionais estão disponíveis nas opções adicionais. Eles permitem especificar quando a regra deve ser aplicada e seu nível de alerta:

   * **[!UICONTROL Fase]**: este campo permite que você especifique em qual ponto do ciclo de vida da entrega a regra será aplicada. Selecione o valor a ser aplicado na lista suspensa **[!UICONTROL Fase]**. Expanda a seção abaixo para obter mais detalhes sobre os valores possíveis.

   +++Fases das regras de controle:

   **[!UICONTROL No início do direcionamento]**: para evitar que a etapa de personalização seja executada em caso de erros, é possível aplicar a regra de controle aqui.

   **[!UICONTROL Após o direcionamento]**: se você precisar saber o volume do destino para aplicar a regra de controle, selecione esta fase. Por exemplo, a regra de controle Check proof size se aplica após cada estágio do targeting: essa regra impede a personalização da mensagem se houver muitos recipients de prova.

   **[!UICONTROL No início da personalização]**: esta fase deve ser selecionada se o controle envolver a aprovação da personalização da mensagem. A personalização da mensagem é realizada durante a fase de análise.

   **[!UICONTROL No final da análise]**:Quando uma verificação exige a personalização da mensagem para ser concluída, selecione esta fase.

+++

   * **[!UICONTROL Nível]**: essas opções permitem especificar o nível de alerta para a regra. Expanda a seção abaixo para obter mais informações.

   +++Níveis de regras de controle:

   **[!UICONTROL Erro]**: parar a preparação da mensagem.

   **[!UICONTROL Aviso]**: exibir um aviso nos logs de preparação.

   **[!UICONTROL Informações]**: exibir informações nos logs de preparação.

   <!--**[!UICONTROL Status]**:-->

   **[!UICONTROL Detalhado]**: exibir informações nos logs do servidor.

+++

### Criar o conteúdo da regra {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="Filtragem"
>abstract="As regras de **Filtragem** excluem segmentos do público-alvo com base em critérios específicos (por exemplo, idade, local, país, números de telefone). Selecione a dimensão de direcionamento da regra de tipologia e clique no botão **[!UICONTROL Adicionar regras]** para acessar o modelador de consultas e criar a regra."

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="Código"
>abstract="As regras de **Controle** verificam a qualidade e a validade da mensagem pré-enviada (por exemplo, exibição de caracteres, comprimento do SMS, formato de endereço, redução de URL). Eles são criados usando o código JavaScript."

Após definir as propriedades da regra de tipologia, é possível criar o conteúdo da regra.

* Para **Regras de controle**, clique no botão **Editar código** e insira a lógica da regra usando o JavaScript. No exemplo abaixo, estamos criando uma regra para exibir um aviso nos logs se o target estiver vazio.

  ![](assets/business-rules-code.png)

* Para **Regras de filtragem**, selecione a targeting dimension e clique no botão **[!UICONTROL Adicionar regras]** para definir os critérios de filtragem usando o [modelador de consultas](../query/query-modeler-overview.md).

  ![](assets/business-rules-query.png)

Quando a regra estiver pronta, clique no botão **[!UICONTROL Criar]** para criar a regra de tipologia. Agora você pode fazer referência à regra em uma tipologia para aplicá-la a mensagens.

## Regras de tipologia de referência em uma tipologia {#add-rules}

Para referenciar uma ou várias regras em uma tipologia, siga estas etapas:

1. Navegue até a guia **[!UICONTROL Tipologia]** e abra a tipologia onde deseja fazer referência à(s) regra(s).

1. Selecione a guia **[!UICONTROL Regras de tipologia]** e clique no botão **[!UICONTROL Adicionar regra de tipologia]**.

   ![](assets/business-rules-reference.png)

1. Selecione uma ou várias regras de tipologia para associar à tipologia e confirmar.

   ![](assets/business-rules-typology-save.png)

1. Clique em **[!UICONTROL Salvar]**.

Agora você pode aplicar a tipologia a mensagens. Depois de concluído, todas as regras de tipologia selecionadas serão executadas para executar as verificações definidas.

## Aplicar tipologias a mensagens {#message}

Para aplicar uma tipologia a uma mensagem ou a um template de mensagem, é necessário selecionar a tipologia nas configurações da mensagem. [Saiba como definir as configurações de entrega](../advanced-settings/delivery-settings.md#typology)

![](assets/business-rules-apply.png)

Depois de concluído, as regras de tipologia incluídas na tipologia são executadas para verificar a validade do delivery durante a preparação da mensagem. Os perfis que correspondem aos critérios em uma regra de tipologia são excluídos dos públicos-alvo do delivery.
