---
audience: end-user
title: Configurar e gerenciar o processo de aprovação
description: Saiba como gerenciar aprovações de campanhas de marketing no Campaign Web
feature: Approvals, Campaigns
exl-id: 8140f904-ec0a-44e1-981f-0e050d3c9cdb
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 5%

---

# Gerenciar o processo de aprovação {#campaign-approvals}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn6"
>title="Gerenciamento de aprovação de campanha"
>abstract="Agora é possível coordenar a validação das partes interessadas antes de enviar os deliveries. Exigir aprovações de gerentes de marketing, analistas de dados ou outras equipes para controle de qualidade."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

>[!IMPORTANT]
>
>As aprovações só estão disponíveis para remessas criadas dentro de uma campanha. Isso não se aplica a deliveries autônomos ou deliveries criados em workflows fora de um contexto de campanha.

O processo de aprovação ajuda a coordenar vários participantes e garante o controle de qualidade antes que os deliveries sejam enviados. Use aprovações quando sua organização exigir a validação de equipes diferentes, como gerentes de marketing que revisam conteúdo ou analistas de dados que validam públicos-alvo.

Quando as aprovações estiverem habilitadas, você deverá enviar conteúdo ou público alvo para aprovação. Os revisores designados recebem notificações por email solicitando validação e podem aprovar ou rejeitar diretamente da interface da Web. Os deliveries não podem ser enviados até que todas as aprovações necessárias sejam concedidas. Você pode ativar:

* **Aprovação de conteúdo**: validar o conteúdo, o design e a personalização da mensagem
* **Aprovação do público-alvo**: validar o público-alvo e os critérios de direcionamento
* **Confirmação de entrega**: é necessária uma confirmação final antes de enviar

## Definir configurações de aprovação {#configure-approvals}

As configurações de aprovação são herdadas do template de campanha e podem ser modificadas para campanhas individuais. Siga estas etapas para definir configurações de aprovação:

1. Abra sua campanha ou modelo de campanha, ou crie um novo, no menu **[!UICONTROL Campanhas]**.

1. Clique no botão **[!UICONTROL Configurações]** na parte superior direita do painel de campanha.

1. Na seção **[!UICONTROL Aprovações]**, configure as seguintes opções:

   ![Captura de tela mostrando as configurações de aprovação da campanha](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Habilitar aprovação de conteúdo]**: quando habilitado, o conteúdo de entrega deve ser aprovado antes do envio. Clique no ícone de pasta no campo **[!UICONTROL Revisor]** para selecionar um operador ou grupo de operadores.

   * **[!UICONTROL Habilitar aprovação de público alvo]**: quando habilitado, o público alvo da entrega deve ser aprovado. Clique no ícone de pasta no campo **[!UICONTROL Revisor]** para selecionar um operador ou grupo de operadores.

   * **[!UICONTROL Confirmar a entrega antes de enviar]**: exige uma confirmação manual final antes de enviar, mesmo depois que todas as outras aprovações estiverem concluídas.

>[!NOTE]
>
>* Se nenhum revisor for especificado, o proprietário da campanha será atribuído como revisor.
>* Os revisores precisam de permissões apropriadas para aprovar deliveries. Somente os usuários identificados na lista de revisores podem aprovar.

## Enviar para aprovação {#submit-approval}

Depois de criar o delivery, siga estas etapas para enviar conteúdo e público-alvo para aprovação.

>[!NOTE]
>As aprovações estão disponíveis em deliveries de workflow de campanha e deliveries independentes de campanha.

1. No painel de entrega, clique no botão **[!UICONTROL Enviar conteúdo]**. Os revisores designados podem aprovar ou rejeitar. Consulte esta [seção](#approve-reject).

   ![Captura de tela mostrando o botão Enviar conteúdo](assets/approvals2.png){zoomable="yes"}

   O status de aprovação muda para pendente na seção **[!UICONTROL Properties]** do painel de entrega. Consulte esta [seção](#rack-approvals).

1. Depois que o conteúdo for aprovado, clique no botão **[!UICONTROL Preparar]** para preparar o destino de entrega. O sistema prepara o público-alvo e os critérios de direcionamento.

1. Clique no botão **[!UICONTROL Enviar destino]**. Os revisores designados podem aprovar ou rejeitar. Consulte esta [seção](#approve-reject).

   ![Captura de tela mostrando o botão Enviar destino](assets/approvals5.png){zoomable="yes"}

   O status de aprovação muda para pending. Consulte esta [seção](#rack-approvals).

1. Depois que o target for aprovado, a preparação será retomada e o delivery poderá ser enviado.

>[!NOTE]
>Se uma aprovação for rejeitada, o proprietário do delivery deverá fazer todas as alterações necessárias no conteúdo ou público alvo com base no feedback do revisor e reenviar para aprovação.

## Aprovar ou rejeitar {#approve-reject}

Os revisores designados podem aprovar ou rejeitar conteúdo e direcionar envios. Consulte esta [seção](#submit-approval).

>[!NOTE]
>Para que a notificação por email seja enviada, o endereço do revisor deve ser configurado na instância.

1. Ao receber o email de notificação, abra o delivery que requer aprovação diretamente da interface do usuário da Web.

1. Revise o conteúdo ou as informações de direcionamento.

1. Clique no botão **[!UICONTROL Aprovar conteúdo]** ou **[!UICONTROL Aprovar destino]**.

   ![Captura de tela mostrando o botão Aprovar conteúdo no painel de entrega](assets/approvals3.png){zoomable="yes"}

1. Clique em **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]**.

1. Opcionalmente, adicione um **[!UICONTROL Comentário]** para explicar sua decisão.

   ![Captura de tela mostrando a caixa de diálogo de aprovação com os botões Aprovar, Rejeitar e o campo Comentário](assets/approvals4.png){zoomable="yes"}

1. Confirme sua decisão. O status de aprovação é atualizado imediatamente no painel do delivery. Consulte esta [seção](#rack-approvals).

## Rastrear status de aprovação {#track-approvals}

O status de aprovação é visível na seção **[!UICONTROL Properties]** do painel de entrega. O status exibe quais aprovações estão aguardando e seu estado atual:

![Captura de tela mostrando o status de aprovação](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL Sendo editado]**: o conteúdo ou destino ainda não foi enviado para aprovação
* **[!UICONTROL Aprovação pendente]**: o conteúdo ou destino está aguardando revisão
* **[!UICONTROL Aprovado]**: o conteúdo ou destino foi aprovado pelo revisor
* **[!UICONTROL Rejected]**: o conteúdo ou destino foi rejeitado pelo revisor

A seção de aprovação mostra todas as aprovações e atualizações ativadas em tempo real, conforme os revisores validam ou rejeitam cada etapa.

## Tópicos relacionados {#related}

* [Criar campanhas](create-campaigns.md)
* [Gerenciar campanhas](manage-campaigns.md)
