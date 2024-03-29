---
audience: end-user
title: Usar a atividade do workflow Carregar arquivo
description: Saiba como usar a atividade de workflow Carregar arquivo
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 44%

---

# Carregar arquivo {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Atividade Carregar arquivo"
>abstract="A atividade **Carregar arquivo** é uma atividade de **gerenciamento de dados**. Use esta atividade para trabalhar com dados armazenados em um arquivo externo."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Arquivo de amostra"
>abstract="Arquivo de amostra"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Nome do arquivo"
>abstract="Nome do arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Banco de dados de públicos-alvo"
>abstract="Banco de dados de públicos-alvo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Gerenciamento de rejeições da atividade Carregar arquivo"
>abstract="Gerenciamento de rejeições da atividade Carregar arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Transição de saída do gerenciamento de rejeições"
>abstract="Transição de saída do gerenciamento de rejeições"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Transição de saída do gerenciamento de rejeições para recusas"
>abstract="Transição de saída do gerenciamento de rejeições para recusas"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Formatação da atividade Carregar arquivo"
>abstract="Formatação da atividade Carregar arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Arquivo de destino da atividade Carregar arquivo"
>abstract="Arquivo de destino da atividade Carregar arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Remapeamento de valor da atividade Carregar arquivo"
>abstract="Remapeamento de valor da atividade Carregar arquivo"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Comando Carregar arquivo"
>abstract="Permitir comandos arbitrários para pré-processamento é uma vulnerabilidade de segurança. Desabilite a opção de segurança XtkSecurity_Disable_Preproc para forçar o uso de uma lista predefinida de comandos."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Excluir arquivo após importação"
>abstract="A confirmar"

A atividade **Carregar arquivo** é uma atividade de **gerenciamento de dados**. Use esta atividade para trabalhar com perfis e dados armazenados em um arquivo externo. Perfis e dados não são adicionados ao banco de dados, mas todos os campos no arquivo de entrada estão disponíveis para [personalização](../../personalization/gs-personalization.md), ou para atualizar perfis ou qualquer outra tabela.

>[!NOTE]
>Os formatos de arquivo compatíveis são: texto (TXT) e valor separado por vírgula (CSV).

Esta atividade pode ser usada com um [Reconciliação](reconciliation.md) atividade para vincular dados não identificados aos recursos existentes. Por exemplo, a variável **Carregar arquivo** A atividade pode ser colocada antes de um **Reconciliação** atividade se você importar dados não padrão para o banco de dados.

## Configurar a atividade de carregamento de arquivo {#load-configuration}

Siga estas etapas para configurar o **Carregar arquivo** atividade:

1. Arraste e solte uma **Carregar arquivo** atividade no seu workflow. Clique em **Selecionar do arquivo** botão.

1. Selecione o arquivo local a ser usado. O formato deve estar alinhado com este [arquivo de amostra](../../audience/file-audience.md#sample-file).

1. Visualize e verifique como os dados estão mapeados na seção central da tela.

   ![](../assets/load-file.png)

1. Use o **Colunas** no painel esquerdo para ajustar o tipo de dados e a largura de cada coluna.

1. No **Formatação** seção localizada na configuração de colunas, especifique como o arquivo externo é formatado para garantir que os dados sejam importados corretamente.

1. Clique em **Confirmar** assim que as configurações estiverem corretas.

## Exemplo{#load-example}

Uma amostra de carregamento de arquivo externo usada com o **Reconciliação** a atividade está disponível em [nesta seção](reconciliation.md#reconciliation-example).
