---
audience: end-user
title: Criar públicos-alvo
description: Saiba como criar públicos-alvo no Adobe Campaign Web
badge: label="Beta"
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 523a43bef4f179740a96039ac2fc5f4f858aa1dc
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 29%

---

# Criar públicos-alvo {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Composição de público-alvo"
>abstract="Crie novos públicos-alvo em uma tela de fluxo de trabalho intuitiva. Além de criar um público-alvo simples do zero, você também pode aproveitar as atividades do fluxo de trabalho para refinar seu público-alvo. Combine vários públicos-alvo em um único público-alvo, enriqueça-o com atributos externos ou divida-o em vários públicos-alvo com base em regras de sua escolha."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=pt-BR" text="Consulte as notas de versão"

<!--TO REMOVE BELOW-->

>[!CONTEXTUALHELP]
>id="acw_homepage_rn1"
>title="Composição do público-alvo"
>abstract="Crie novos públicos-alvo em uma tela de fluxo de trabalho intuitiva. Além de criar um público-alvo simples do zero, você também pode aproveitar as atividades do fluxo de trabalho para refinar seu público-alvo. Combine vários públicos-alvo em um único público-alvo, enriqueça-o com atributos externos ou divida-o em vários públicos-alvo com base em regras de sua escolha."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html?lang=pt-BR" text="Consulte as notas de versão"

<!--TO REMOVE ABOVE-->

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="Nessa tela, é possível acessar a lista de todos os públicos-alvo que podem ser direcionados em suas entregas. Clique em **Criar** para criar novos públicos-alvo em uma tela visual usando várias atividades de fluxo de trabalho, como **Dividir** ou **Excluir**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Configurações de público-alvo"
>abstract="Insira o nome do público-alvo e as opções adicionais, e clique no botão **Criar público-alvo**."

O Campaign Web permite criar novos públicos-alvo em uma tela de fluxo de trabalho visual. Além de criar um público-alvo simples do zero, você também pode aproveitar as atividades do fluxo de trabalho para refinar seu público-alvo. Por exemplo, você pode combinar vários públicos-alvo em um único, enriquecer o público-alvo com atributos externos ou dividi-lo em vários públicos-alvo com base em regras de sua escolha.

Depois de criar o fluxo de trabalho, os públicos resultantes são automaticamente armazenados no banco de dados do Campaign junto com os existentes. Esses públicos-alvo podem ser direcionados em workflows ou deliveries independentes.

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

1. Abra o **[!UICONTROL Criar público-alvo]** atividade e usar o modelador de consultas para definir a população a ser incluída no público-alvo filtrando os dados contidos no banco de dados. [Saiba como configurar uma atividade Criar público-alvo](../workflows/activities/build-audience.md)

1. Se você quiser executar operações adicionais no público direcionado para o workflow, adicione quantas atividades forem necessárias e conecte-as. Para obter mais informações sobre como configurar atividades de workflow, consulte [documentação de workflows](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >As atividades de canal não estão disponíveis para uso em fluxos de trabalho de público.

   ![](assets/audience-creation-canvas.png)

1. Configure o **[!UICONTROL Salvar público-alvo]** atividade para especificar como você deseja salvar a população computada upstream no workflow. [Saiba como configurar uma atividade Salvar público](../workflows/activities/save-audience.md)

1. Quando o workflow estiver pronto, clique em **[!UICONTROL Início]** para executá-lo.

O workflow é salvo na variável **[!UICONTROL Fluxos de trabalho]** lista, enquanto os públicos resultantes estão acessíveis na **[!UICONTROL Públicos-alvo]** lista. Saiba como monitorar e gerenciar públicos-alvo no [nesta seção](manage-audience.md)

Agora você pode usar esse público-alvo como o principal alvo de uma entrega. [Saiba mais](add-audience.md)

## Exemplo de fluxo de trabalho de público {#example}

O exemplo abaixo mostra um fluxo de trabalho de público-alvo configurado para direcionar clientes do sexo feminino que moram em Nova York e criar dois novos públicos-alvo, dependendo de sua compra mais recente (Yoga ou Running gear).

![](assets/audiences-example.png)

1. A variável **[!UICONTROL Criar público-alvo]** A atividade segmenta todas as perfis femininas que vivem em Nova York.
1. A variável **[!UICONTROL Enriquecimento]** A atividade de enriquece o público-alvo com informações da tabela Purchases para identificar o tipo de produto que os clientes compraram.
1. A variável **[!UICONTROL Split]** A atividade divide o fluxo de trabalho em dois caminhos com base na compra mais recente dos clientes.
1. A variável **[!UICONTROL Salvar público-alvo]** as atividades no final de cada caminho criam dois novos públicos-alvo no banco de dados, incluindo a população calculada em cada caminho.
