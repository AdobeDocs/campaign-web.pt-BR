---
title: Conta externa
description: Saiba como configurar contas externas
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 21%

---

# Configurar contas externas {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Contas externas"
>abstract="Agora você pode se conectar a plataformas adicionais ou personalizar as conexões para se adequar ao seu fluxo de trabalho e criar facilmente novas contas externas para atender às suas necessidades específicas e garantir transferências de dados perfeitas."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"


>[!AVAILABILITY]
>
> Observe que as contas externas estão disponíveis no momento apenas para emails de Devolução (POP3) e a instância de Execução, com tipos de conta adicionais a serem adicionados no futuro.
> As contas externas não compatíveis criadas no console do Adobe Campaign estão visíveis na Interface do usuário da Web, mas não podem ser editadas ou acessadas.

O Adobe Campaign vem com um conjunto de contas externas pré-configuradas para fácil integração com vários sistemas. Se você precisar se conectar a plataformas adicionais ou personalizar as conexões para se adequar ao seu fluxo de trabalho, agora será possível criar facilmente novas contas externas usando a Interface do usuário da Web para atender às suas necessidades específicas e garantir transferências de dados perfeitas.

## Criar uma conta externa {#create-ext-account}

Para criar uma nova conta externa, siga as etapas abaixo. As configurações detalhadas dependem do tipo de conta externa.

1. No menu do painel esquerdo, selecione **[!UICONTROL Contas externas]** em **[!UICONTROL Administração]**.

1. Clique em **[!UICONTROL Criar conta externa]**.

   ![](assets/external_account_create_1.png)

1. Insira seu **[!UICONTROL Rótulo]** e selecione sua Conta externa **[!UICONTROL Tipo]**.

   ![](assets/external_account_create_2.png)

1. Clique em **[!UICONTROL Create]**.

1. No menu suspenso **[!UICONTROL Opções avançadas]**, você pode alterar o caminho **[!UICONTROL Nome interno]** ou **[!UICONTROL Pasta]**, se necessário.

   ![](assets/external_account_create_3.png)

1. Habilite a opção **[!UICONTROL Exportado automaticamente]** se quiser que os dados gerenciados por esta conta externa sejam exportados automaticamente.

1. Configure o acesso à conta especificando credenciais dependendo do tipo escolhido da conta externa.

1. Clique em **[!UICONTROL Testar a conexão]** para verificar se sua configuração está correta

1. No menu **[!UICONTROL Mais...]**, duplique ou exclua sua conta externa.

   ![](assets/external_account_create_4.png)

1. Quando a configuração estiver concluída, clique em **[!UICONTROL Salvar]**.

## Contas externas específicas de campanha {#campaign-specific}

### Emails rejeitados (POP3) {#bounce}

>[!AVAILABILITY]
>
> No momento, o OAuth 2.0 não é compatível.

A conta externa de email de devolução especifica a conta POP3 externa usada para se conectar ao serviço de email. Todos os servidores configurados para acesso POP3 podem receber email de retorno.

![](assets/external_account_bounce.png)

Para configurar a conta externa de **[!UICONTROL Emails rejeitados (POP3)]**:

* **[!UICONTROL Server]**

  URL do servidor POP3

* **[!UICONTROL Port]**

  Número da porta de conexão POP3 (a porta padrão é 110)

* **[!UICONTROL Account]**

  Nome do usuário

* **[!UICONTROL Password]**

  Senha da conta do usuário

* **[!UICONTROL Criptografia]**

  Tipo de criptografia escolhida entre:

   * Por padrão (POP3 se usar a porta 110, POP3S se usar a porta 995)
   * POP3 que alterna para SSL após o envio de um STARTTLS
   * POP3 não seguro (porta 110 por padrão)
   * POP3 seguro acima de SSL (porta 995 por padrão)

* **[!UICONTROL Função]**

  Email de entrada, quando a conta externa é configurada para receber emails de entrada, ou roteador SOAP, para lidar com solicitações SOAP.

### Instância de execução{#instance-exec}

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
