---
title: Gerenciar conta externa
description: Saiba como configurar contas externas do CRM
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 3%

---

# Conta externa do CRM {#external-crm}

Use uma conta externa do tipo CRM para conectar o Adobe Campaign a um banco de dados de terceiros.

As definições de configuração dessa conta externa dependem do mecanismo de banco de dados específico ao qual você está se conectando. As instruções de configuração detalhadas para cada banco de dados compatível são fornecidas nas seções abaixo.

## Microsoft Dynamics CRM

A conta externa do Microsoft Dynamics CRM permite conectar a instância do Campaign ao banco de dados externo do Microsoft Dynamics CRM.

Na Interface do Usuário da Web do Adobe Campaign, configure a conta externa do Microsoft Dynamics CRM.

1. [Crie sua conta externa](external-account.md) e selecione **[!UICONTROL Banco de dados externo]** como **[!UICONTROL Tipo]** da sua conta externa e Microsoft Dynamics CRM como **[!UICONTROL Tipo de provedor]**.

1. Clique em **[!UICONTROL Create]**.

1. Para configurar a conta externa do **[!UICONTROL Microsoft Dynamics CRM]**, preencha os seguintes campos:

   ![Captura de tela mostrando os campos de configuração da conta externa do Microsoft Dynamics CRM.](assets/crm-microsoft-1.png)

   +++ Para o tipo OAuth do CRM: Credenciais de senha

   * **[!UICONTROL Servidor]**: insira a URL do servidor do Microsoft CRM.

     Para localizar a URL do Servidor do Microsoft CRM, entre na sua conta do Microsoft Dynamics CRM, selecione Dynamics 365 e abra o aplicativo. A URL do servidor é exibida na barra de endereços do seu navegador, por exemplo:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Conta]**: especifique a conta usada para entrar no Microsoft CRM.

   * **[!UICONTROL Senha]**: digite a senha associada à conta especificada.

   * **[!UICONTROL Identificador do cliente]**: insira a ID do cliente encontrada no Portal de Gerenciamento do Microsoft Azure.

   * **[!UICONTROL Versão do CRM]**: escolha a versão do Dynamics CRM 365 CRM.

   +++

   </br>

   +++ Para o tipo de OAuth do CRM: Certificado

   * **[!UICONTROL Servidor]**: insira a URL do servidor do Microsoft CRM.

     Para localizar a URL do Servidor do Microsoft CRM, entre na sua conta do Microsoft Dynamics CRM, selecione Dynamics 365 e abra o aplicativo. A URL do servidor é exibida na barra de endereços do seu navegador, por exemplo:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Chave privada (codificada em Base64)]**: forneça a chave privada codificada no formato Base64.

     Para fazer isso, você pode usar a ajuda de um codificador Base64 ou usar a linha de comando `base64 -w0 private.key` para Linux.

   * **[!UICONTROL Identificador de chave personalizado]**: insira o identificador de chave personalizado usado para seu certificado.

   * **[!UICONTROL ID da Chave]**: Insira a ID da chave associada ao seu certificado.

   * **[!UICONTROL Identificador do cliente]**: insira a ID do cliente encontrada no Gerenciamento do Microsoft Azure

   * **[!UICONTROL Versão do CRM]**: escolha a versão do Dynamics CRM 365 CRM.

   +++

1. Depois de configurar a conexão, acesse o **[!UICONTROL assistente de configuração do Microsoft CRM]** para gerar sua lista de tabelas do Microsoft CRM.

   Clique em **[!UICONTROL Avançar]** para selecionar as tabelas necessárias.

   ![Captura de tela mostrando os campos de configuração da conta externa do Microsoft Dynamics CRM.](assets/crm-microsoft-2.png)

1. Selecione as tabelas do Microsoft CRM a serem recuperadas ou adicione uma tabela remota especificando o **[!UICONTROL Rótulo da tabela]** e o **[!UICONTROL Nome interno da tabela]**. Em seguida, habilite a opção **[!UICONTROL Selecionado]**.

   Clique em **[!UICONTROL Next]**.

1. Clique em **[!UICONTROL Iniciar]** para começar a criar o esquema do Microsoft CRM com base nas tabelas selecionadas.

1. Siga as instruções na tela para inserir páginas do Histórico de marketing e do Gerenciamento de assinaturas do Adobe Campaign diretamente no Microsoft Dynamics CRM.

1. Clique em **[!UICONTROL Exibir URLs do histórico de marketing]** para exibir as URLs para integração de páginas de Histórico de Marketing ou **[!UICONTROL Exibir URLs para assinaturas de clientes potenciais]** para exibir as URLs para integração de páginas de Gerenciamento de Assinaturas.

   ![Captura de tela mostrando os campos de configuração da conta externa do Microsoft Dynamics CRM.](assets/crm-microsoft-3.png)

1. Clique em **[!UICONTROL Salvar]** depois que a conta externa do Microsoft CRM estiver configurada.

1. Depois que a conta externa for criada, você poderá clicar em **[!UICONTROL Sincronizando enumerações...]** para sincronizar enumerações automaticamente do Microsoft CRM para a Interface do Usuário da Web do Adobe Campaign.

   ![Captura de tela mostrando os campos de configuração da conta externa do Microsoft CRM.](assets/crm-microsoft-4.png)

1. Selecione a enumeração do Adobe Campaign que corresponde à enumeração do Microsoft CRM.

   Para substituir valores do Adobe Campaign por valores do Microsoft CRM, habilite a opção **[!UICONTROL Substituir]**.

## Salesforce {#salesforce}

Para configurar a conta externa do Salesforce para funcionar com o Adobe Campaign, é necessário fornecer os seguintes detalhes:

1. [Crie sua conta externa](external-account.md) e selecione **[!UICONTROL Banco de dados externo]** como o **[!UICONTROL Tipo]** da sua conta externa e Salesforce.com como **[!UICONTROL Tipo de provedor]**.

   ![Captura de tela mostrando os campos de configuração da conta externa do Salesforce.](assets/crm-salesforce-1.png)

1. Clique em **[!UICONTROL Create]**.

1. Para configurar a conta externa do **[!UICONTROL Salesforce]**, preencha os seguintes campos:

   * **[!UICONTROL Tipo de OAuth do CRM]**: **[!UICONTROL Credenciais da senha]** ou **[!UICONTROL Credenciais]**

   * **[!UICONTROL Conta]**: conta usada para entrar no Salesforce CRM.

   * **[!UICONTROL Senha]**: digite a senha associada à conta especificada.

   * **[!UICONTROL Token de segurança]**: insira o token de segurança do Salesforce associado à conta.

   * **[!UICONTROL Versão da API]**: escolha a Versão 49.

   ![Captura de tela mostrando os campos de configuração da conta externa do Salesforce.](assets/crm-salesforce-2.png)

1. Abra o **[!UICONTROL assistente de configuração do Salesforce CRM]** para gerar sua lista de tabelas do Salesforce CRM e clique em **[!UICONTROL Avançar]**.

   ![Captura de tela mostrando os campos de configuração da conta externa do Salesforce CRM.](assets/crm-salesforce-3.png)

1. Selecione as tabelas do Salesforce a serem recuperadas ou adicione uma tabela remota inserindo o **[!UICONTROL Rótulo da tabela]** e o **[!UICONTROL Nome interno da tabela]**. Em seguida, habilite a opção **[!UICONTROL Selecionado]**.

   Clique em **[!UICONTROL Next]**.

1. Clique em **[!UICONTROL Iniciar]** para começar a criar o esquema do Salesforce CRM com base nas tabelas selecionadas.

1. Clique em **[!UICONTROL Assistente de criação de links do Salesforce...]** para gerar os links da Web no Salesforce.

   Em seguida, clique em **[!UICONTROL Avançar]** para recuperar os links da Web para **Clientes potenciais** e **Contatos** da Salesforce.

1. Selecione os links a serem exportados para a lista de links da Web do Salesforce.

1. Siga as instruções na tela para inserir as páginas **Histórico de Marketing** e **Gerenciamento de Assinaturas** da Interface Web do Adobe Campaign no Salesforce CRM.

1. Clique em **[!UICONTROL Salvar]** depois que a conta externa do Salesforce CRM estiver configurada.

1. Depois que a conta externa for criada, você poderá clicar em **[!UICONTROL Sincronizando enumerações...]** para sincronizar enumerações automaticamente do Salesforce para a Interface do Usuário da Adobe Campaign Web.

   ![Captura de tela mostrando os campos de configuração da conta externa do Salesforce CRM.](assets/crm-salesforce-4.png)

1. Selecione a lista discriminada do Adobe Campaign que corresponde à lista discriminada do Salesforce.

   Para substituir valores Adobe Campaign por valores Salesforce, habilite a opção **[!UICONTROL Substituir]**.

   ![Captura de tela mostrando os campos de configuração da conta externa do Salesforce CRM.](assets/crm-salesforce-5.png)

