---
audience: end-user
title: Criar um delivery de correspondência direta
description: Saiba como projetar seu delivery de correspondência direta com o Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 8%

---

# Criar o arquivo de extração {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Conteúdo do arquivo de extração"
>abstract="Clique no botão **Editar conteúdo** para iniciar a criação do arquivo de extração exigido pelo seu provedor de correspondência direta. Isso permite definir as propriedades do arquivo, como rótulo e formato, e especificar as colunas que deseja incluir no arquivo."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propriedades do arquivo"
>abstract="Configure as propriedades do arquivo de extração, como nome e formato. Você pode personalizar o nome do arquivo usando atributos do banco de dados usando o editor de expressão."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Conteúdo"
>abstract="Nesta seção, especifique as colunas a serem exibidas no arquivo de extração. Depois de concluído, você pode visualizar o arquivo de extração usando o botão **Simular conteúdo**."

Para criar o conteúdo do arquivo de extração gerado pela entrega de correspondência direta, clique no botão **[!UICONTROL Editar conteúdo]** na página de entrega e configure as propriedades e o conteúdo do arquivo.

## Configurar as propriedades do arquivo de extração {#properties}

1. No campo **[!UICONTROL Nome do arquivo]**, especifique o nome desejado para o arquivo de extração. Você pode personalizar o nome do arquivo usando atributos do banco de dados. Para fazer isso, clique no ícone **[!UICONTROL Abrir caixa de diálogo de personalização]** para abrir o editor de expressão. [Saiba como personalizar o conteúdo](../personalization/personalize.md)

1. No campo **[!UICONTROL Formato de arquivo]**, escolha o formato desejado para o arquivo de extração: **Texto**, **Texto usando colunas de largura fixa**, **CSV (Excel)** ou **XML**.

1. Expanda a seção **[!UICONTROL Formato de extração]** para acessar opções específicas relacionadas ao formato do arquivo de extração. Os valores disponíveis dependem do formato selecionado.

+++ Opções de formato de extração disponíveis

   * **[!UICONTROL Usar a primeira linha como cabeçalho da coluna]** (Formato de texto/CSV (Excel)): ative esta opção para usar a primeira coluna como cabeçalho.
   * **[!UICONTROL Separador de coluna]** (formato de texto): especifique o caractere a ser usado como separador de coluna no arquivo de extração.
   * **[!UICONTROL Delimitador de cadeia de caracteres]** (Formato de texto): especifique como delimitar cadeias de caracteres no arquivo de extração.
   * **[!UICONTROL Fim da linha]** (Formato de texto): especifique como delimitar o fim das linhas no arquivo de extração.
   * **[!UICONTROL Codificação]**: escolha a codificação do arquivo de extração.
   * **[!UICONTROL Formato de data e separadores]**: especifique como as datas devem ser formatadas no arquivo de extração.
   * **[!UICONTROL Formato de número]**: especifique como os números devem ser formatados no arquivo de extração.
   * **[!UICONTROL Exportar rótulos em vez de valores internos de enumerações]**: ative esta opção se exportar valores de enumeração e quiser recuperar rótulos de coluna, que são mais fáceis de entender, em vez de IDs internas.

+++

1. Ative a opção **[!UICONTROL Quantidade solicitada]** para restringir o número de destinatários da sua entrega.

   ![Captura de tela mostrando as opções de configuração de detalhes de conteúdo para o arquivo de extração.](assets/dm-content-details.png){zoomable="yes"}

## Configurar as colunas do arquivo de extração {#content}

Na seção **[!UICONTROL Conteúdo]**, especifique as colunas a serem exibidas no arquivo de extração. Para fazer isso, siga estes passos:

1. Clique no botão **[!UICONTROL Adicionar atributo]** para criar uma nova coluna.
1. Escolha o atributo a ser exibido na coluna e confirme. Observe que você pode usar o editor de expressão para selecionar o atributo clicando no botão **[!UICONTROL Editar expressão]**. [Saiba como selecionar atributos e adicioná-los aos favoritos](../get-started/attributes.md)

   ![Captura de tela mostrando o botão Adicionar Atributo e as opções para adicionar atributos ao arquivo de extração.](assets/dm-add-attribute.png)

1. Depois que a coluna for adicionada, você poderá alterar seu rótulo e modificar o atributo associado usando o ícone de edição.
1. Repita essas etapas para adicionar quantas colunas forem necessárias para o arquivo de extração.
1. Para classificar o arquivo de extração usando uma das colunas, clique no ícone na coluna **[!UICONTROL Sorting]** e selecione o método de classificação desejado.
1. Para alterar a posição de uma coluna, use as setas para cima e para baixo.

![Captura de tela mostrando as opções de configuração de atributos para o arquivo de extração.](assets/dm-content-attributes.png)

Agora você pode visualizar o arquivo de extração e enviar o delivery para gerar o arquivo de extração. [Saiba como testar e enviar mensagens de correspondência direta](send-direct-mail.md)