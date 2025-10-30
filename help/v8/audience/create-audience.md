---
audience: end-user
title: Criar públicos-alvo
description: Saiba como criar públicos-alvo no Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 15%

---

# Criar públicos-alvo {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Públicos-alvo"
>abstract="Nesta tela, é possível acessar a lista de todos os públicos-alvo que podem ser direcionados nos fluxos de trabalhos ou nas entregas independentes. Clique em **Criar** para criar um novo público-alvo em uma tela visual.<br/><br/>Além de criar um público-alvo simples do zero, você também pode aproveitar as atividades de fluxo de trabalho para refinar o seu público-alvo. Por exemplo, é possível combinar vários públicos-alvo em um, enriquecer o público-alvo com atributos externos ou dividi-lo em vários públicos-alvo com base em regras de sua escolha."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

O Campaign Web permite criar novos públicos-alvo em uma tela de fluxo de trabalho visual. Além de criar um público-alvo simples do zero, você também pode aproveitar as atividades do fluxo de trabalho para refinar seu público-alvo. Por exemplo, é possível combinar vários públicos-alvo em um, enriquecer o público-alvo com atributos externos ou dividi-lo em vários públicos-alvo com base em regras de sua escolha.

Depois de criar o fluxo de trabalho, os públicos resultantes são automaticamente armazenados no banco de dados do Campaign junto com os existentes. Esses públicos-alvo podem ser direcionados em workflows ou deliveries independentes.

A coluna **[!UICONTROL Origem]** indica as origens dos públicos-alvo: os públicos-alvo do **[!UICONTROL Adobe Campaign]** são criados no console do Adobe Campaign v8 ou na Interface do Usuário da Web, enquanto os públicos-alvo do **[!UICONTROL Adobe Experience Platform:]** são criados no Adobe Experience Platform e integrados ao Campaign usando a integração de Fontes e Destinos do Adobe.

➡️ [Conheça este recurso no vídeo](#video)

## Criar seu primeiro público-alvo {#create}

Para criar um público-alvo, siga estas etapas:

1. Navegue até o menu **[!UICONTROL Públicos-alvo]** e clique no botão **[!UICONTROL Criar público-alvo]**, localizado no canto superior direito.

1. Um novo fluxo de trabalho é criado automaticamente, permitindo combinar atividades para gerar seu público. Por padrão, a tela contém duas atividades principais:

   * A atividade &quot;Query&quot; **[!UICONTROL Build audience]** é o ponto de partida do seu fluxo de trabalho. Ele permite criar um público-alvo e usá-lo como base para o seu fluxo de trabalho.

   * A atividade &quot;Novo público-alvo&quot; **[!UICONTROL Salvar público-alvo]** representa a etapa final do fluxo de trabalho. Ela permite salvar os resultados como um novo público-alvo.

   ![Uma tela de criação de público-alvo em branco com duas atividades padrão: Criar público-alvo e Salvar público-alvo.](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >Os fluxos de trabalho do público-alvo são armazenados no menu **Fluxos de trabalho**, juntamente com os outros fluxos de trabalho do Campaign. Eles são especificamente projetados para construir públicos e são identificáveis por sua tela vertical.

1. Para melhorar a compreensão, altere o nome do fluxo de trabalho no campo **Rótulo** das configurações do fluxo de trabalho. [Saiba como definir configurações de fluxo de trabalho](../workflows/workflow-settings.md)

1. Abra a atividade **[!UICONTROL Criar público-alvo]** e use o modelador de consultas para definir a população a ser incluída no público-alvo filtrando os dados contidos no banco de dados. [Saiba como configurar uma atividade Criar público-alvo](../workflows/activities/build-audience.md)

1. Se você quiser executar operações adicionais no público-alvo do fluxo de trabalho, adicione quantas atividades forem necessárias e conecte-as. Para obter mais informações sobre como configurar atividades de fluxo de trabalho, consulte a [documentação sobre fluxos de trabalho](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >As atividades de canal não estão disponíveis para uso em fluxos de trabalho de público.

   ![Uma tela de criação de público-alvo com várias atividades conectadas para refinar o público-alvo.](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configure a atividade **[!UICONTROL Save audience]** para especificar como você deseja salvar a população computada upstream no fluxo de trabalho. [Saiba como configurar uma atividade Save audience](../workflows/activities/save-audience.md)

1. Quando o fluxo de trabalho estiver pronto, clique em **[!UICONTROL Iniciar]** para executá-lo.

O fluxo de trabalho é salvo na lista **[!UICONTROL Fluxos de trabalho]**, enquanto os públicos resultantes ficam acessíveis na lista **[!UICONTROL Públicos-alvo]** com o rótulo definido na atividade **Salvar público**. Saiba como monitorar e gerenciar públicos [nesta seção](manage-audience.md)

Agora você pode usar esse público-alvo como o principal alvo de uma entrega. [Saiba mais](add-audience.md)

## Exemplo de fluxo de trabalho de público {#example}

O exemplo abaixo mostra um fluxo de trabalho de público-alvo configurado para direcionar clientes do sexo feminino que moram em Nova York e criar dois novos públicos-alvo, dependendo de sua compra mais recente (Yoga ou Running gear).

![Um exemplo de fluxo de trabalho de público-alvo direcionado a clientes do sexo feminino em Nova York e dividindo-os com base em suas compras mais recentes.](assets/audiences-example.png){zoomable="yes"}

1. A atividade **[!UICONTROL Criar público]** segmenta todos os perfis femininos que vivem em Nova York.
1. A atividade **[!UICONTROL Enrichment]** enriquece o público com informações da tabela Purchases para identificar o tipo de produto que os clientes compraram.
1. A atividade **[!UICONTROL Split]** divide o fluxo de trabalho em dois caminhos com base na compra mais recente dos clientes.
1. As atividades **[!UICONTROL Salvar público-alvo]** no final de cada caminho criam dois novos públicos-alvo no banco de dados, incluindo a população calculada em cada caminho.

## Editar um público {#edit}

Você pode modificar um público-alvo gerado por um fluxo de trabalho sempre que necessário, executando novamente o fluxo de trabalho correspondente. Isso permite atualizar os dados do público ou refiná-lo ajustando o query de acordo com suas necessidades.

1. Navegue até o menu **Públicos-alvo** e abra o público-alvo que deseja editar.
1. Na guia **Visão geral**, a seção **Último fluxo de trabalho** fornece um link para o fluxo de trabalho usado para gerar o público-alvo. Clique nele para acessar o workflow.
1. Faça as alterações desejadas e clique no botão **Iniciar** para executar o fluxo de trabalho novamente. Após a conclusão, o público-alvo resultante do fluxo de trabalho é atualizado automaticamente com os resultados mais recentes do fluxo de trabalho.

Por padrão, a nova execução de um fluxo de trabalho de público-alvo substitui todo o conteúdo do público-alvo por novos dados, causando a perda de dados anteriores.

Se preferir não substituir os resultados do público existente, configure as atividades **Salvar público-alvo** para alinharem-se aos seus requisitos. Por exemplo, você pode alterar o campo **Rótulo do público-alvo** para armazenar os novos resultados em um novo público-alvo ou adicionar os novos resultados ao conteúdo do público-alvo existente sem apagar os dados anteriores. [Saiba como configurar uma atividade Save audience](../workflows/activities/save-audience.md)

![A tela de configuração Salvar atividade do público-alvo com opções para ajustar o comportamento de salvamento do público-alvo.](assets/edit-audience-save.png){zoomable="yes"}

## Vídeo tutorial {#video}

Saiba como criar e gerenciar públicos-alvo, selecionar públicos-alvo para uma entrega e definir grupos de controle.

>[!VIDEO](https://video.tv.adobe.com/v/3453207?captions=por_br&quality=12)