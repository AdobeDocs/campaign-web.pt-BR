---
audience: end-user
title: Usar a atividade do workflow Carregar arquivo
description: Saiba como usar a atividade de workflow Carregar arquivo
badge: label="Disponibilidade limitada"
source-git-commit: f88c3cd200aa92f4db7a2ab36c85d778a07a4dc3
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 35%

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

Uma amostra de carregamento de arquivo externo usada com o **Reconciliação** a atividade está disponível em [nesta seção](reconciliation.md#example).