---
title: Gerenciar conta externa
description: Saiba como configurar contas externas
exl-id: 24e70106-3312-4138-bf2d-ffad74e2962d
source-git-commit: 155a7f3fb55a579dbf9a2ad81a1dc7e4ea3847df
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 2%

---

# Contas externas específicas de campanha {#external-account}

Siga as etapas abaixo para definir as configurações da conta com base no tipo de conta externa selecionada.

## Emails rejeitados (POP3) {#bounce}

A conta externa de Bounce mails especifica a conta POP3 externa usada para se conectar ao serviço de email. Todos os servidores configurados para acesso POP3 podem receber email de retorno.

![Captura de tela mostrando os campos de configuração da conta externa de emails devolvidos (POP3).](assets/external_account_bounce.png)

Para configurar a conta externa de **[!UICONTROL Emails rejeitados (POP3)]**, preencha os seguintes campos:

* **[!UICONTROL Servidor]** - URL do servidor POP3.

* **[!UICONTROL Porta]** - número da porta de conexão POP3 (a porta padrão é 110).

* **[!UICONTROL Conta]** - Nome do usuário.

* **[!UICONTROL Senha]** - Senha da conta de usuário.

* **[!UICONTROL Criptografia]** - Tipo de criptografia escolhida, incluindo:
   * Por padrão (POP3 se porta 110, POP3S se porta 995).
   * POP3 que alterna para SSL após enviar um STARTTLS.
   * POP3 não seguro (porta 110 por padrão).
   * POP3 seguro acima do SSL (porta 995 por padrão).

* **[!UICONTROL Função]** - Selecione **[!UICONTROL Email de entrada]** para configurar a conta para receber emails de entrada ou **[!UICONTROL Roteador SOAP]** para lidar com solicitações SOAP.

>[!IMPORTANT]
>
>Antes de configurar sua conta externa POP3 usando o Microsoft OAuth 2.0, primeiro é necessário registrar seu aplicativo no portal do Azure. Para obter mais informações, consulte [esta página](https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app){target=_blank}.

Para configurar um POP3 externo usando o Microsoft OAuth 2.0, marque a opção Microsoft OAuth 2.0 e preencha os seguintes campos:

* **[!UICONTROL Locatário do Azure]**

  A ID do Azure (ou a ID do diretório (locatário)) pode ser encontrada na lista suspensa Essentials da visão geral do seu aplicativo no portal do Azure.

* **[!UICONTROL ID do Azure Client]**

  A ID do cliente (ou a ID do aplicativo (cliente)) pode ser encontrada na lista suspensa do Essentials da visão geral do seu aplicativo no portal do Azure.

* **[!UICONTROL Segredo do Azure Client]**

  A ID do segredo do cliente pode ser encontrada na coluna Segredos do cliente do menu Certificados e segredos do aplicativo no portal do Azure.

* **[!UICONTROL URL de redirecionamento do Azure]**

  A URL de redirecionamento pode ser encontrada no menu Autenticação do seu aplicativo no portal do Azure. Ele deve terminar com a seguinte sintaxe nl/jsp/oauth.jsp, por exemplo: `https://redirect.adobe.net/nl/jsp/oauth.jsp`.

O acesso à Internet é necessário para a configuração e para usar o botão Testar conexão no console do cliente. Após a configuração, o processo do InMail pode se comunicar com os servidores da Microsoft sem Internet.

Depois de inserir suas credenciais diferentes, você pode clicar em Configurar a conexão para concluir a configuração da conta externa.

## Roteamento {#routing}

Para configurar uma conta externa específica para deliveries externos, siga as etapas abaixo.

1. Crie uma conta externa. [Saiba mais](create-external-account.md)

1. Selecione o tipo **[!UICONTROL Roteamento]**.

   ![Captura de tela mostrando a seleção do tipo de conta externa de Roteamento.](assets/external-account-routing.png){zoomable="yes"}

1. Selecione o canal desejado e clique em **[!UICONTROL Criar]**.

1. Na seção **[!UICONTROL Detalhes]** da conta externa, **[!UICONTROL Externo]** é selecionado por padrão como o **[!UICONTROL Modo de entrega]**.

   ![Captura de tela mostrando a configuração do modo de Entrega para contas externas de Roteamento.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Atualmente, **[!UICONTROL Externo]** é o único modo disponível.

1. Para lidar com o processo após a execução do delivery, externalize isso para um fluxo de trabalho de pós-processamento. Crie um fluxo de trabalho com uma atividade [Sinal externo](../workflows/activities/external-signal.md) e selecione-o no campo **[!UICONTROL Pós-processamento]**.

   ![Captura de tela mostrando a configuração do campo Pós-processamento para contas externas de Roteamento.](assets/external-account-post-processing.png){zoomable="yes"}

1. No campo **[!UICONTROL Atividade]**, edite o nome da atividade de fluxo de trabalho de pós-processamento exibida nos logs. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

## Instância de execução {#instance-exec}

Se você tiver uma arquitetura segmentada, identifique as instâncias de execução associadas à instância de controle e estabeleça conexões entre elas. Os templates de mensagem transacional são implantados na instância de execução.

![Captura de tela mostrando os campos de configuração da conta externa da instância de execução.](assets/external_account_exec.png)

Para configurar a conta externa **[!UICONTROL Instância de execução]**:

* **[!UICONTROL URL]** - URL do servidor onde a instância de execução está instalada.

* **[!UICONTROL Conta]** - Nome da conta, correspondente ao Agente do Centro de Mensagens conforme definido na pasta do operador.

* **[!UICONTROL Senha]** - Senha da conta conforme definido na pasta do operador.

* **[!UICONTROL Método]** - Escolha entre o serviço Web ou o FDA (Federated Data Access — Acesso a Dados Federados).

  Para FDA, selecione a conta FDA. Observe que a conexão do Campaign com sistemas externos é restrita a usuários avançados e está disponível somente no console do cliente. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Criar fluxo de trabalho de arquivamento]** - Para cada instância de execução registrada no Centro de Mensagens, independentemente de haver uma ou várias instâncias, crie um fluxo de trabalho de arquivamento separado para cada conta externa associada à instância de execução.
