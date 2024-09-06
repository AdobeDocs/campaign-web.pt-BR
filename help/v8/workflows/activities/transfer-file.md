---
audience: end-user
title: Usar a atividade Transferir arquivo
description: Saiba como usar a atividade de workflow Transferir arquivo
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 19%

---

# Transferir arquivo {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="Transferir arquivo"
>abstract="A atividade **Transferir arquivo** permite receber ou enviar arquivos, testar a presença de arquivos ou listar arquivos em um servidor. O protocolo usado pode ser o protocolo servidor para servidor ou o protocolo HTTP."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="Transferir opções do arquivo"
>abstract="Transferir opções do arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="Transferir atividade do arquivo"
>abstract="Transferir atividade do arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="Transferir servidor remoto do arquivo"
>abstract="Especifique o servidor ao qual deseja se conectar."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="Transferir origem do arquivo"
>abstract="Insira o nome do arquivo desejado."

A atividade **Transferir arquivo** é uma atividade de **Gerenciamento de Dados**. Ele permite receber ou enviar arquivos, testar a presença de arquivos ou listar arquivos em um servidor. O protocolo usado pode ser o protocolo servidor para servidor ou o protocolo HTTP.

>[!NOTE]
>
>Com a interface do usuário da Web do Campaign, consolidamos duas atividades em uma unindo os recursos de **transferência de arquivos** e **download da Web**. Essa consolidação não afeta a funcionalidade da atividade de forma alguma.

Siga as etapas detalhadas abaixo para configurar a atividade **Transferir arquivo**.

## Escolher o protocolo e a operação de transferência {#protocol}

1. Adicione uma atividade **Transferir arquivo** ao fluxo de trabalho e especifique o tipo de transferência a ser executado, dependendo do protocolo que deseja usar:

   * Para protocolo HTTP, selecione **[!UICONTROL Download da Web]**. Isso permite executar um download de GET ou POST em um URL explícito, uma conta externa ou uma instância do Adobe Campaign.
   * Para outros protocolos servidor a servidor e ações relacionadas, selecione **[!UICONTROL Transferência de arquivos]**.

1. Selecione a ação a ser executada com a atividade. As ações disponíveis dependem do tipo de transferência que você selecionou. Expanda as seções abaixo para obter mais informações.

   +++Ações disponíveis com **atividades do tipo transferência de arquivos**

   * **[!UICONTROL Download de arquivo]**: baixar um arquivo do servidor.
   * **[!UICONTROL Carregamento de arquivo]**: carregar um arquivo no servidor.
   * **[!UICONTROL Teste para ver se o arquivo existe]**: verifique se um determinado arquivo está presente no servidor. Gera duas transições de saída após a atividade: &quot;File exists&quot; e &quot;File does not exist&quot;.
   * **[!UICONTROL Lista de arquivos]**: lista todos os arquivos disponíveis no servidor.

+++

   +++Ações disponíveis com **atividades do tipo download da Web**

   * **[!UICONTROL Transferência simples (GET)]**: recuperar um arquivo.
   * **[!UICONTROL Transferir usando um formulário (POST)]**: Carregar um arquivo e parâmetros adicionais.

+++

   ![](../assets/workflow-transfer-file-action.png)

1. Por padrão, para ações de upload de arquivo, a atividade usa o arquivo especificado na atividade anterior. Para usar um arquivo diferente, desative a opção **[!UICONTROL Usar arquivo da atividade anterior]** e clique no botão **[!UICONTROL Adicionar arquivo]**.

   No campo **[!UICONTROL Source]**, insira o nome de arquivo desejado ou use o editor de expressão para calcular o nome de arquivo usando variáveis de evento. [Saiba como trabalhar com variáveis de evento e o editor de expressão](../event-variables.md). Repita a operação para adicionar quantos arquivos forem necessários.

## Definir o destino da transferência {#destination}

1. Na seção **[!UICONTROL Servidor remoto]**, especifique o servidor a ser conectado usando um destes métodos:

   * **[!UICONTROL Usar parâmetros de conexão definidos em uma conta externa]**: conecte-se a um servidor usando os parâmetros de conexão de uma conta externa. No campo **[!UICONTROL Pasta do servidor]**, especifique o caminho para o arquivo (ou para a pasta para ações de listagem de arquivos).
   * **[!UICONTROL Configuração rápida]**: insira a URL do arquivo (ou pasta para ações de listagem de arquivos).
   * **[!UICONTROL Instância do Adobe Campaign]** (atividades do tipo download da Web): baixe um arquivo de um servidor de instâncias do Adobe Campaign.

   ![](../assets/workflow-transfer-file-server.png)

1. Para ações POST de download da Web, você pode passar parâmetros adicionais com a operação. Para fazer isso, clique no botão **[!UICONTROL Adicionar parâmetro]** e especifique o nome e o valor dos parâmetros. Você pode adicionar quantos parâmetros forem necessários.

1. Por padrão, para o upload de arquivos, os arquivos carregados em um servidor são salvos automaticamente. Se você não quiser manter este histórico, desative a opção **[!UICONTROL Manter histórico de arquivos enviados]**.

## Configurações de histórico {#historization}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="Historização de arquivos"
>abstract="Toda vez que uma atividade **[!UICONTROL Transferir arquivo]** é executada, ela armazena os arquivos carregados ou baixados em uma pasta dedicada. Uma pasta é criada para cada atividade Transfer file de um workflow. Por padrão, os arquivos são salvos no diretório de armazenamento padrão da pasta de instalação do Adobe Campaign (`/vars`) antes de serem processados. Para usar uma pasta específica, desative a opção **[!UICONTROL Usar um diretório de armazenamento padrão]** e insira o caminho do diretório."

Toda vez que uma atividade **[!UICONTROL Transferir arquivo]** é executada, ela armazena os arquivos carregados ou baixados em uma pasta dedicada. Uma pasta é criada para cada atividade Transfer file de um workflow. Por padrão, os arquivos são salvos no diretório de armazenamento padrão da pasta de instalação do Adobe Campaign (`/vars`) antes de serem processados. Para usar uma pasta específica, desative a opção **[!UICONTROL Usar um diretório de armazenamento padrão]** e insira o caminho do diretório.

![](../assets/workflow-transfer-file-historization.png)

É importante poder limitar o tamanho dessa pasta para preservar o espaço físico no servidor. Para fazer isso, é possível definir um número máximo de arquivos ou o tamanho total da pasta da atividade. Por padrão, 100 arquivos e 50 MB são autorizados.

Toda vez que a atividade é executada, a pasta é verificada da seguinte maneira:

* Somente os arquivos criados mais de 24 horas antes da execução da atividade são considerados.
* Se o número de arquivos considerados for maior que o valor do campo **[!UICONTROL Número de arquivos]**, os arquivos mais antigos serão excluídos até que o número máximo de arquivos permitidos seja atingido.
* Se o tamanho total dos arquivos considerados for maior que o valor do parâmetro **[!UICONTROL Tamanho máximo (em MB)]**, os arquivos mais antigos serão excluídos até que o Tamanho máximo (em MB) permitido seja atingido.

>[!CAUTION]
>
>Se a atividade não for executada novamente, a pasta correspondente não será verificada nem eliminada. Por isso, tenha cuidado ao transferir arquivos grandes.

## Opções avançadas de gerenciamento de &amp; erros {#advanced}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="Excluir os arquivos de origem após a transferência"
>abstract="Apague os arquivos de origem após uma transferência bem-sucedida."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="Exibir os logs de sessão"
>abstract="Exibe as informações relacionadas à operação de transferência nos logs do fluxo de trabalho."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="Listar todos os arquivos"
>abstract="Essa opção indexa todos os arquivos presentes no servidor na variável de evento **vars.filenames**."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="Processar arquivos ausentes"
>abstract="Essa opção permite ativar uma transição de saída **Nenhum arquivo** após a atividade."

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="Processar erros"
>abstract="Essa opção permite ativar uma transição de saída **Erro** após a atividade."

1. Nas **[!UICONTROL Opções avançadas]**, opções adicionais estão disponíveis com base no tipo de atividade que você está configurando. Expanda as seções abaixo para obter mais informações.

   +++Opções adicionais para **[!UICONTROL atividades do tipo transferência de arquivos]**

   * **[!UICONTROL Excluir os arquivos de origem após a transferência]**: apague os arquivos de origem após uma transferência bem-sucedida.
   * **[!UICONTROL Exibir os logs de sessão]**: quando esta opção é ativada, as informações relacionadas à operação de transferência são exibidas nos logs de fluxo de trabalho após a execução do fluxo de trabalho.
   * **[!UICONTROL Listar todos os arquivos]** (Ações de listagem de arquivos): esta opção indexa todos os arquivos presentes no servidor na variável de evento `vars.filenames`, na qual os nomes dos arquivos são separados pelos caracteres `n`. [Saiba como trabalhar com variáveis de evento](../event-variables.md)

+++

   +++Opções adicionais para **[!UICONTROL atividades do tipo download da Web]**

   * **[!UICONTROL Seguir redirecionamentos]**: o redirecionamento de arquivo permite usar substituições para direcionar a entrada ou saída de dados para um dispositivo de tipo diferente.
   * **[!UICONTROL Adicionar os cabeçalhos HTTP ao arquivo]**: em alguns casos, talvez você queira adicionar outros cabeçalhos HTTP a um arquivo. Normalmente, esses cabeçalhos serão usados para fornecer informações adicionais para fins de solução de problemas, para [Compartilhamento de recursos entre origens (CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS) ou para definir diretivas específicas de armazenamento em cache.
   * **[!UICONTROL Ignorar o código de retorno HTTP]**: códigos de retorno HTTP, também conhecidos como códigos de status HTTP, indicam o resultado de uma solicitação HTTP.

1. A opção **[!UICONTROL Process errors]** permite ativar uma transição de saída &quot;Error&quot; após a atividade se ocorrer algum erro durante a transferência.

   Além disso, para atividades do tipo **Transferência de arquivos**, a opção **[!UICONTROL Arquivo ausente]** permite ativar uma transição de saída &quot;Nenhum arquivo&quot; após a atividade, se o arquivo não estiver disponível no caminho especificado.
