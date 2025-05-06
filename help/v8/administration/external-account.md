---
title: Gerenciar conta externa
description: Saiba como configurar contas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 21%

---

# Gerenciar contas externas {#external-accounts}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Criação de Conta Externa"
>abstract="Como administrador do Campaign, agora você pode configurar novas conexões com sistemas externos por meio da interface da Web do Campaign. Você também pode exibir, atualizar e gerenciar contas externas existentes."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

O Adobe Campaign inclui contas externas pré-configuradas para facilitar a integração com vários sistemas. Para se conectar a plataformas adicionais ou personalizar conexões para se adequar ao seu fluxo de trabalho, crie novas contas externas usando a Interface do usuário da Web. Isso garante transferências de dados perfeitas.

## Criar uma conta externa {#create-ext-account}

Para criar uma nova conta externa, siga as etapas abaixo. As configurações detalhadas dependem do tipo de conta externa. [Saiba mais](#campaign-specific)

1. No menu do painel esquerdo, selecione **[!UICONTROL Contas externas]** em **[!UICONTROL Administração]**.

1. Clique em **[!UICONTROL Criar conta externa]**.

   ![Captura de tela mostrando a opção de criar uma conta externa na Interface de Usuário da Web.](assets/external_account_create_1.png)

1. Insira seu **[!UICONTROL Rótulo]** e selecione o **[!UICONTROL Tipo]** da conta externa.

   >[!NOTE]
   >
   >As configurações para tipos específicos de campanha estão detalhadas em [esta seção](#campaign-specific).

   ![Captura de tela mostrando campos para inserir o rótulo e selecionar o tipo de conta externa.](assets/external_account_create_2.png)

1. Clique em **[!UICONTROL Create]**.

1. No menu suspenso **[!UICONTROL Opções adicionais]**, altere o caminho **[!UICONTROL Nome interno]** ou **[!UICONTROL Pasta]**, se necessário.

   ![Captura de tela mostrando opções adicionais para configuração de nome interno e caminho de pasta.](assets/external_account_create_3.png)

1. Habilite a opção **[!UICONTROL Exportado automaticamente em pacotes]** para exportar automaticamente dados gerenciados por esta conta externa. <!--Exported where??-->

   ![Captura de tela mostrando a opção para habilitar a exportação automática em pacotes.](assets/external_account_create_exported.png)

1. Na seção **[!UICONTROL Detalhes]**, configure o acesso à conta especificando credenciais com base no tipo de conta externa escolhido. [Saiba mais](#bounce)

1. Clique em **[!UICONTROL Testar conexão]** para verificar se sua configuração está correta.

1. No menu **[!UICONTROL Mais...]**, duplique ou exclua sua conta externa.

   ![Captura de tela mostrando o menu Mais com opções para duplicar ou excluir a conta externa.](assets/external_account_create_4.png)

1. Quando a configuração for concluída, clique em **[!UICONTROL Salvar]**.

## Contas externas específicas de campanha {#campaign-specific}

Dependendo do tipo de conta externa selecionado, siga as etapas abaixo para definir as configurações da conta.

### Emails rejeitados (POP3) {#bounce}

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

### Roteamento {#routing}

Para configurar uma conta externa específica para deliveries externos, siga as etapas abaixo.

1. Crie uma conta externa. [Saiba mais](../administration/external-account.md#create-ext-account)

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

### Instância de execução {#instance-exec}

Se você tiver uma arquitetura segmentada, identifique as instâncias de execução associadas à instância de controle e estabeleça conexões entre elas. Os templates de mensagem transacional são implantados na instância de execução.

![Captura de tela mostrando os campos de configuração da conta externa da instância de execução.](assets/external_account_exec.png)

Para configurar a conta externa **[!UICONTROL Instância de execução]**:

* **[!UICONTROL URL]** - URL do servidor onde a instância de execução está instalada.

* **[!UICONTROL Conta]** - Nome da conta, correspondente ao Agente do Centro de Mensagens conforme definido na pasta do operador.

* **[!UICONTROL Senha]** - Senha da conta conforme definido na pasta do operador.

* **[!UICONTROL Método]** - Escolha entre o serviço Web ou o FDA (Federated Data Access — Acesso a Dados Federados).

  Para FDA, selecione a conta FDA. Observe que a conexão do Campaign com sistemas externos é restrita a usuários avançados e está disponível somente no console do cliente. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Criar fluxo de trabalho de arquivamento]** - Para cada instância de execução registrada no Centro de Mensagens, independentemente de haver uma ou várias instâncias, crie um fluxo de trabalho de arquivamento separado para cada conta externa associada à instância de execução.

## Contas externas da Integração de soluções da Adobe

### Adobe Experience Cloud

Para se conectar ao console do Adobe Campaign usando uma Adobe ID, você deve configurar a conta externa do Adobe Experience Cloud (MAC).

![Captura de tela mostrando os campos de configuração da conta externa do Adobe Experience Cloud MAC.](assets/external-MAC.png)

* **[!UICONTROL IMS server]**

  URL do seu servidor IMS. Verifique se as instâncias de estágio e de produção apontam para o mesmo ponto final de produção IMS.

* **[!UICONTROL IMS scope]**

  Os escopos definidos aqui devem ser um subconjunto daqueles provisionados pelo IMS.

* **[!UICONTROL IMS client identifier]**

  ID do seu cliente IMS.

* **[!UICONTROL IMS client secret]**

  Credencial do segredo do cliente IMS.

* **[!UICONTROL Callback server]**

  URL de acesso da instância do Adobe Campaign.

* **[!UICONTROL IMS organization ID]**

  ID da sua organização. Para encontrar seu ID de organização, consulte [esta página](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=pt-BR){target=_blank}.

* **[!UICONTROL Association mask]**

  A sintaxe que permitirá que os nomes de configuração no Painel Enterprise sejam sincronizados com os grupos no Adobe Campaign.

* **[!UICONTROL Server]**

  URL da sua instância da Adobe Experience Cloud.

* **[!UICONTROL Tenant]**

  Nome do seu locatário do Adobe Experience Cloud.

## Contas externas de transferência de dados

### Serviço de armazenamento simples Amazon (S3) {#amazon-simple-storage-service--s3--external-account}

O conector do Serviço de Armazenamento Simples da Amazon (S3) pode ser usado para importar ou exportar dados para o Adobe Campaign. Ele pode ser configurado em uma atividade de workflow. Para obter mais informações, consulte [esta página](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![](assets/external-AWS.png)

Como você está configurando essa nova conta externa, é necessário fornecer os seguintes detalhes:

* **[!UICONTROL AWS S3 Account Server]**

  A URL do seu servidor deve ser preenchida da seguinte maneira:

  `  <S3bucket name>.s3.amazonaws.com/<s3object path>`


* **[!UICONTROL AWS access key ID]**

  Para saber onde encontrar a ID da chave de acesso AWS, consulte esta [página](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys).

* **[!UICONTROL Secret access key to AWS]**

  Para saber onde encontrar a chave de acesso secreta para o AWS, consulte esta [página](https://aws.amazon.com/fr/blogs/security/wheres-my-secret-access-key/).

* **[!UICONTROL AWS Region]**

  Para saber mais sobre a região do AWS, consulte esta [página](https://aws.amazon.com/about-aws/global-infrastructure/regions_az/).

* A caixa de seleção **[!UICONTROL Use server side encryption]** permite armazenar o arquivo no modo criptografado S3.

Para saber onde encontrar a ID da chave de acesso e a chave de acesso secreta, consulte a [documentação](https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys) dos serviços Web da Amazon.

### Armazenamento Azure Blob {#azure-blob-external-account}

A conta externa **[!UICONTROL Armazenamento Azure Blob]** pode ser usada para importar ou exportar dados para a Adobe Campaign usando uma atividade de fluxo de trabalho **[!UICONTROL Transferir arquivo]**. Para obter mais informações, consulte [esta seção](https://experienceleague.adobe.com/en/docs/campaign-web/v8/wf/design-workflows/transfer-file){target=_blank}.

![](assets/external-azure.png)

Para configurar a **[!UICONTROL conta externa do Azure]** para funcionar com a Adobe Campaign, você precisa fornecer os seguintes detalhes:

* **[!UICONTROL Server]**

  URL do seu servidor de armazenamento Azure Blob.

* **[!UICONTROL Encryption]**

  Tipo de criptografia escolhida entre **[!UICONTROL None]** ou **[!UICONTROL SSL]**.

* **[!UICONTROL Access key]**

  Para saber onde encontrar sua **[!UICONTROL Chave de acesso]**, consulte esta [página](https://docs.microsoft.com/en-us/azure/storage/common/storage-account-keys-manage?tabs=azure-portal).

## Hadoop

A conta externa do Hadoop permite conectar a instância do Campaign ao banco de dados externo do Hadoop. Você pode saber mais sobre o Hadoop na [documentação do console do Campaign V7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/accessing-external-database/configure-fda/config-databases/configure-fda-hadoop){target=_blank}.

![Captura de tela mostrando a configuração da conta externa do Hadoop.](assets/external-hadoop.png)

* **[!UICONTROL Server]**

  URL do servidor de armazenamento Hadoop.

* **[!UICONTROL Account]**

  Nome da conta do servidor do Hadoop.
