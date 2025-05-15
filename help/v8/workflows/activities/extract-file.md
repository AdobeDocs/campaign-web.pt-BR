---
audience: end-user
title: Usar a atividade de workflow Extrair arquivo
description: Saiba como usar a atividade de workflow Extrair arquivo
exl-id: fa50ab5b-2539-4517-9d7b-93315f1e505c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 16%

---

# Extrair arquivo {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Extrair arquivo"
>abstract="A atividade **Extrair arquivo** permite exportar dados do Adobe Campaign como um arquivo externo. Os dados podem então ser exportados para um local de servidor, como SFTP, armazenamento na nuvem ou servidor de campanha, usando uma atividade Transferir arquivo."

A atividade **Extrair arquivo** é uma atividade de **Gerenciamento de dados**. Use esta atividade para exportar dados do Adobe Campaign na forma de um arquivo externo. Os dados podem então ser exportados para um local de servidor, como SFTP, armazenamento na nuvem ou servidor de campanha, usando uma atividade Transferir arquivo.

Para configurar a atividade **Extrair arquivo**, adicione uma atividade **Extrair arquivo** no seu fluxo de trabalho e, em seguida, siga as etapas abaixo.

## Configurar o arquivo a ser extraído {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Arquivo a ser extraído"
>abstract="Selecione o arquivo a ser extraído."

A seção **[!UICONTROL Arquivo a ser extraído]** permite configurar as propriedades do arquivo e os dados a serem incluídos.

![Captura de tela mostrando as opções de configuração do arquivo a ser extraído.](../assets/extract-file-file.png)

1. No campo **[!UICONTROL Nome do arquivo]**, digite o nome desejado para o arquivo a ser extraído.

   Você pode personalizar o nome do arquivo usando variáveis de evento, condições e funções de data/hora. Para fazer isso, clique no ícone **[!UICONTROL Abrir caixa de diálogo de personalização]** para abrir o editor de expressão. [Saiba como trabalhar com variáveis de evento e o editor de expressão](../event-variables.md).

1. Especifique as colunas a serem apresentadas no arquivo extraído. Para fazer isso, siga estes passos:

   1. Clique na **[!UICONTROL Adicionar coluna de saída]**.
   1. Escolha o atributo a ser exibido na coluna e confirme. Os atributos disponíveis dependem do targeting dimension do fluxo de trabalho. [Saiba como selecionar atributos e adicioná-los aos favoritos](../../get-started/attributes.md).
   1. Após adicionar a coluna, você poderá alterar seu **[!UICONTROL Rótulo]** e modificar o **[!UICONTROL Atributo]** associado.
   1. Para aplicar uma transformação aos valores da coluna, selecione-a na lista suspensa. Por exemplo, você pode colocar todos os valores na coluna selecionada em maiúsculas.

1. Repita essas etapas para adicionar quantas colunas forem necessárias no arquivo de extração. Para alterar a posição de uma coluna, use as setas para cima e para baixo.

1. Para remover todas as linhas duplicadas do arquivo extraído, alterne a opção **[!UICONTROL Remover linhas duplicadas (Listagem)]**.

1. Para classificar o arquivo extraído com base em um atributo, alterne na opção **[!UICONTROL Habilitar Classificação]** e escolha o atributo pelo qual deseja classificar o arquivo, juntamente com o método de classificação desejado (crescente ou decrescente). Você pode classificar qualquer atributo da dimensão de direcionamento atual, independentemente de ele ter sido adicionado às colunas do arquivo ou não.

## Configurar o formato de arquivo extraído {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Formato de destino"
>abstract="Selecione as diferentes opções para configurar a formatação do arquivo extraído."

A seção de formato **[!UICONTROL Destino]** permite configurar como o arquivo extraído será formatado.

1. Escolha o **[!UICONTROL Formato de saída]** para o arquivo extraído: **Texto**, **Texto usando colunas de largura fixa**, **CSV (Excel)** ou **XML**.

1. Clique no botão **[!UICONTROL Formato de extração]** para acessar opções específicas relacionadas ao formato selecionado. Expanda a seção abaixo para obter mais informações.

+++ Opções de formato de extração disponíveis

   * **[!UICONTROL Usar a primeira linha como cabeçalho da coluna]** (Formato de texto/CSV (Excel)): ative esta opção para usar a primeira coluna como cabeçalho.
   * **[!UICONTROL Separador de coluna]** (formato de texto): especifique o caractere a ser usado como separador de coluna no arquivo de saída.
   * **[!UICONTROL Delimitador de cadeia de caracteres]** (Formato de texto): especifique como delimitar cadeias de caracteres no arquivo de saída.
   * **[!UICONTROL Fim da linha]** (Formato de texto): especifique como delimitar o fim das linhas no arquivo de saída.
   * **[!UICONTROL Codificação]**: escolha a codificação do arquivo de saída.
   * **[!UICONTROL Formato de data e separadores]**: especifique como as datas devem ser formatadas no arquivo de saída.
   * **[!UICONTROL Formato de número]**: especifique como os números devem ser formatados no arquivo de saída.
   * **[!UICONTROL Exportar rótulos em vez de valores internos de enumerações]**: ative esta opção se exportar valores de enumeração e quiser recuperar rótulos de coluna, que são mais fáceis de entender, em vez de IDs internas.

+++

   ![Captura de tela mostrando as opções de configuração do arquivo a ser extraído.](../assets/extract-file-format.png)

## Adicionar um estágio de pré-processamento {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Pós-processamento"
>abstract="Defina uma etapa de pós-processamento a ser aplicada, como compactação ou criptografia."

O **[!UICONTROL script de modificação de exportação]** permite aplicar um estágio de processamento para ser executado durante a extração de dados, como compactação ou criptografia. Para fazer isso, clique no botão **[!UICONTROL Editar script]**.

O editor de expressão é aberto, permitindo inserir o comando a ser aplicado ao arquivo. O painel do lado esquerdo fornece sintaxes predefinidas que você pode utilizar para criar seu script. [Saiba como trabalhar com variáveis de evento e o editor de expressão](../event-variables.md).

![Captura de tela mostrando o editor de scripts para pós-processamento.](../assets/extract-file-script.png)

## Opções adicionais {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Transição de saída"
>abstract="Ative a opção **Gerar uma transição de saída** para adicionar uma transição de saída após a atividade atual."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Processar erros"
>abstract="Ative a opção **Processar erros** para adicionar uma transição de saída que contém erros."

Depois que a extração do arquivo de saída tiver sido configurada, opções adicionais relacionadas às transições e ao gerenciamento de erros estarão disponíveis:

* **[!UICONTROL Gerar transição de saída]**: ative essa opção para adicionar uma transição de saída e configurar seu rótulo.
* **[!UICONTROL Não gerar um arquivo se a transição de entrada estiver vazia]**: ative esta opção para ignorar a extração de arquivos se a transição de entrada não contiver dados.
* **[!UICONTROL Erro de processo]**: ative essa opção para adicionar uma transição de saída se algum erro for encontrado durante a extração do arquivo.

## Exemplo {#example}

No exemplo a seguir, uma atividade **Build audience** é seguida por uma atividade **Extract file** para extrair todos os perfis direcionados em um arquivo CSV.

![Captura de tela mostrando um fluxo de trabalho de exemplo com uma atividade Criar público-alvo seguida por uma atividade Extrair arquivo.](../assets/extract-file-example.png)

* O campo **[!UICONTROL Nome do arquivo]** está configurado para incluir a data da extração.

  ![Captura de tela mostrando a configuração do nome do arquivo com a data incluída.](../assets/extract-file-example-name.png)

* As colunas são adicionadas para exibir o nome e o sobrenome dos perfis, as IDs do cliente e as datas de criação no banco de dados.

  ![Captura de tela mostrando a configuração das colunas no arquivo extraído.](../assets/extract-file-example-columns.png)