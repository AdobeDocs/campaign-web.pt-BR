---
audience: end-user
title: Criar públicos
description: Saiba como criar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 1%

---


# Criar públicos {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="Nessa tela, você pode criar e combinar públicos-alvo em uma tela visual. Adicione várias atividades de workflow, como **Split** ou **Excluir** para gerar públicos novos e refinados."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configurações do público-alvo"
>abstract="Insira o nome do público-alvo e as opções adicionais e clique no link **Criar público-alvo** botão."

O Campaign Web permite criar novos públicos-alvo em uma tela de fluxo de trabalho visual. Além de começar do zero para criar um público-alvo simples, você também pode aproveitar as atividades do fluxo de trabalho para refinar seus públicos-alvo. Por exemplo, você pode dividir vários públicos-alvo em um único, enriquecer públicos-alvo com atributos externos ou dividir um determinado público-alvo em vários.

Depois de criar o fluxo de trabalho, os públicos resultantes são automaticamente armazenados no banco de dados do Campaign junto com os existentes. Esses públicos-alvo podem ser direcionados em campanhas ou deliveries independentes.

As principais etapas para criar um público-alvo são as seguintes:

1. Criar um fluxo de trabalho de público-alvo.
1. Configure uma atividade Build audience para consultar o banco de dados com base em suas necessidades.
1. Adicione atividades de workflow para refinar seu público-alvo (opcional).
1. Configure uma atividade Save audience.
1. Execute o fluxo de trabalho para salvar o(s) público(s) resultante(s) no banco de dados.


## Criar seu primeiro público-alvo {#create}

Para criar um público-alvo, siga estas etapas:

1. Navegue até a **[!UICONTROL Públicos-alvo]** e clique no botão **[!UICONTROL Criar público-alvo]** localizado no canto superior direito.
1. Forneça um rótulo para o público.
1. Expanda a **[!UICONTROL Opções adicionais]** seção para configurar parâmetros avançados de público-alvo.

   Por padrão, os públicos-alvo são criados na **[!UICONTROL Perfis e públicos alvo]** / **[!UICONTROL Listas]** menu do explorador. É possível alterar o local de armazenamento padrão usando o **[!UICONTROL Pasta]** campo.

   ![](assets/audiences-settings.png)

1. Depois de definir as configurações de público-alvo, clique no **[!UICONTROL Criar público-alvo]** botão.

1. Uma tela de workflow é exibida, apresentando duas atividades padrão:

   * **[!UICONTROL Criar público-alvo]**: este é o ponto de partida do fluxo de trabalho, permitindo criar um público-alvo e usá-lo como base para ele. [Saiba como configurar uma atividade Criar público-alvo](../workflows/activities/build-audience.md)

   * **[!UICONTROL Salvar público-alvo]**: representa a etapa final do fluxo de trabalho, permitindo salvar os resultados como um novo público-alvo. [Saiba como configurar uma atividade Salvar público](../workflows/activities/save-audience.md)

1. Se desejar executar uma operação adicional após a **[!UICONTROL Criar público-alvo]** adicionar quantas atividades forem necessárias ao fluxo de trabalho. Para obter mais informações sobre como configurar atividades de workflow, consulte [documentação de workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >As atividades de canal não estão disponíveis para uso em fluxos de trabalho de público.

   ![](assets/audience-creation-canvas.png)

1. Quando o workflow estiver pronto, clique em **[!UICONTROL Início]** para executá-lo.

1. O workflow é salvo na variável **[!UICONTROL Fluxos de trabalho]** lista, enquanto os públicos resultantes estão acessíveis na **[!UICONTROL Públicos-alvo]** lista. [Saiba como monitorar e gerenciar públicos](access-audiences.md)

## Exemplo de fluxo de trabalho de público {#example}

O exemplo abaixo mostra um fluxo de trabalho de público-alvo configurado para direcionar clientes do sexo feminino que moram em Nova York e criar dois novos públicos-alvo, dependendo do centro de interesse no Yoga ou na Running Gear. Os dois públicos-alvo são enriquecidos com informações adicionais relacionadas às compras dos clientes.

ADICIONAR CAPTURA DE TELA

1. A atividade Build audience segmenta todos os perfis femininos que vivem em Nova York.
1. A atividade Enrichment enriquece o público-alvo com atributos da tabela Purchases.
1. A atividade Split divide o workflow em dois caminhos com base nos centros de interesse dos clientes.
1. As atividades Save audience no final de cada caminho para salvar cada público no banco de dados.
