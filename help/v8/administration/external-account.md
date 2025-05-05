---
title: Gerenciar conta externa
description: Saiba como configurar contas externas
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 3%

---

# Gerenciar contas externas {#external-accounts}

>[!AVAILABILITY]
>
>* Contas externas estão disponíveis no momento apenas para emails de devolução (POP3), Roteamento e a Instância de execução. Outros tipos de conta serão adicionados posteriormente.
>
>* As contas externas não compatíveis criadas no console do Adobe Campaign estão visíveis na Interface do usuário da Web, mas não podem ser editadas ou acessadas.

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

>[!AVAILABILITY]
>
> No momento, o OAuth 2.0 não é compatível.

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

  Para FDA, selecione a conta FDA. Observe que a conexão do Campaign com sistemas externos é restrita a usuários avançados e está disponível somente no console do cliente. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Criar fluxo de trabalho de arquivamento]** - Para cada instância de execução registrada no Centro de Mensagens, independentemente de haver uma ou várias instâncias, crie um fluxo de trabalho de arquivamento separado para cada conta externa associada à instância de execução.