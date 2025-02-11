---
title: Gerenciar conta externa
description: Saiba como configurar contas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 14%

---

# Gerenciar contas externas {#external-accounts}

>[!AVAILABILITY]
>
>* Atualmente, contas externas estão disponíveis apenas para emails de devolução (POP3), Roteamento e a Instância de execução. Outros tipos de conta serão adicionados no futuro.
>
>* As contas externas não compatíveis criadas no console do Adobe Campaign estão visíveis na Interface do usuário da Web, mas não podem ser editadas nem acessadas.

O Adobe Campaign vem com um conjunto de contas externas pré-configuradas para fácil integração com vários sistemas. Se você precisar se conectar a plataformas adicionais ou personalizar as conexões para se adequar ao seu fluxo de trabalho, agora será possível criar facilmente novas contas externas usando a Interface do usuário da Web para atender às suas necessidades específicas e garantir transferências de dados perfeitas.

## Criar uma conta externa {#create-ext-account}

Para criar uma nova conta externa, siga as etapas abaixo. As configurações detalhadas dependem do tipo de conta externa. [Saiba mais](#campaign-specific)

1. No menu do painel esquerdo, selecione **[!UICONTROL Contas externas]** em **[!UICONTROL Administração]**.

1. Clique em **[!UICONTROL Criar conta externa]**.

   ![](assets/external_account_create_1.png)

1. Insira seu **[!UICONTROL Rótulo]** e selecione o **[!UICONTROL Tipo]** da conta externa.

   >[!NOTE]
   >
   >As configurações para tipos específicos de campanha estão detalhadas em [esta seção](#campaign-specific).

   ![](assets/external_account_create_2.png)

1. Clique em **[!UICONTROL Create]**.

1. No menu suspenso **[!UICONTROL Opções adicionais]**, você pode alterar o caminho **[!UICONTROL Nome interno]** ou **[!UICONTROL Pasta]**, se necessário.

   ![](assets/external_account_create_3.png)

1. Habilite a opção **[!UICONTROL Exportado automaticamente em pacotes]** se quiser que os dados gerenciados por esta conta externa sejam exportados automaticamente. <!--Exported where??-->

   ![](assets/external_account_create_exported.png)

1. Na seção **[!UICONTROL Detalhes]**, configure o acesso à conta especificando credenciais dependendo do tipo de conta externa escolhido. [Saiba mais](#bounce)

1. Clique em **[!UICONTROL Testar conexão]** para verificar se a configuração está correta.

1. No menu **[!UICONTROL Mais...]**, você pode duplicar ou excluir sua conta externa.

   ![](assets/external_account_create_4.png)

1. Quando a configuração estiver concluída, clique em **[!UICONTROL Salvar]**.

## Contas externas específicas de campanha {#campaign-specific}

Dependendo do tipo de conta externa selecionado, siga as etapas abaixo para definir as configurações da conta.

### Emails rejeitados (POP3) {#bounce}

>[!AVAILABILITY]
>
> No momento, o OAuth 2.0 não é compatível.

A conta externa de Bounce mails especifica a conta POP3 externa usada para se conectar ao serviço de email. Todos os servidores configurados para acesso POP3 podem receber email de retorno.

![](assets/external_account_bounce.png)

Para configurar a conta externa de **[!UICONTROL Emails rejeitados (POP3)]**, preencha os seguintes campos:

* **[!UICONTROL Servidor]** - URL do servidor POP3

* **[!UICONTROL Porta]** - Número da porta de conexão POP3 (a porta padrão é 110)

* **[!UICONTROL Conta]** - Nome do usuário

* **[!UICONTROL Senha]** - Senha da conta de usuário

* **[!UICONTROL Criptografia]** - Tipo de criptografia escolhida entre:

   * Por padrão (POP3 se usar a porta 110, POP3S se usar a porta 995)
   * POP3 que alterna para SSL após o envio de um STARTTLS
   * POP3 não seguro (porta 110 por padrão)
   * POP3 seguro acima de SSL (porta 995 por padrão)

* **[!UICONTROL Função]** - Email de entrada, quando a conta externa está configurada para receber emails de entrada, ou roteador SOAP, para lidar com solicitações SOAP.

### Roteamento {#routing}

Para configurar uma conta externa específica que será usada em seus deliveries externos, siga as etapas abaixo.

1. Crie uma conta externa. [Saiba mais](../administration/external-account.md#create-ext-account)

1. Selecione o tipo **[!UICONTROL Roteamento]**.

   ![](assets/external-account-routing.png){zoomable="yes"}

1. Selecione o canal desejado e clique em **[!UICONTROL Criar]**.

1. Na seção **[!UICONTROL Detalhes]** da conta externa, **[!UICONTROL Externo]** é selecionado por padrão como o **[!UICONTROL Modo de entrega]**.

   ![](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Atualmente, **[!UICONTROL Externo]** é o único modo disponível.

1. Para lidar com o processo após a execução do delivery, é possível externalizar isso para um fluxo de trabalho de pós-processamento. Para fazer isso, você deve criar um fluxo de trabalho com uma atividade [Sinal externo](../workflows/activities/external-signal.md) e selecioná-lo no campo **[!UICONTROL Pós-processamento]**.

   ![](assets/external-account-post-processing.png){zoomable="yes"}

1. No campo **[!UICONTROL Atividade]**, você pode editar o nome da atividade de fluxo de trabalho de pós-processamento que será exibida nos logs. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->


### Instância de execução {#instance-exec}

Se você tiver uma arquitetura segmentada, identifique as instâncias de execução associadas à instância de controle e estabeleça conexões entre elas. Os templates de mensagem transacional são implantados na instância de execução.

![](assets/external_account_exec.png)

Para configurar a conta externa **[!UICONTROL Instância de execução]**:

* **[!UICONTROL URL]**

  URL do servidor no qual a instância de execução está instalada.

* **[!UICONTROL Account]**

  O nome da conta deve corresponder ao Agente do Centro de Mensagens conforme definido na pasta do operador.

* **[!UICONTROL Password]**

  A senha da conta conforme definido na pasta do operador.

* **[!UICONTROL Método]**

  Escolha entre o serviço da Web ou o Federated Data Access (FDA).
No caso do método FDA, selecione a conta FDA. Observe que a conexão do Campaign com sistemas externos é restrita a usuários avançados e está disponível somente no console do cliente. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Criar fluxo de trabalho de arquivamento]**

  Para cada instância de execução registrada no Centro de Mensagens, independentemente de haver uma ou várias instâncias, é necessário criar um fluxo de trabalho de arquivamento separado para cada conta externa associada à instância de execução.
