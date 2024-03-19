---
audience: end-user
title: Criar um delivery de correspondência direta
description: Saiba como projetar seu delivery de correspondência direta com o Adobe Campaign Web
source-git-commit: 717f6f2fb5e07213fb6a16f7ed701f450d1e257e
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 3%

---


# Criar o arquivo de extração {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Conteúdo do arquivo de extração"
>abstract="Clique em **Editar conteúdo** botão para começar a projetar o arquivo de extração exigido pelo seu provedor de correspondência direta. Isso permite definir as propriedades do arquivo, como rótulo e formato, e especificar as colunas que deseja incluir no arquivo."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propriedades do arquivo"
>abstract="Configure as propriedades do arquivo de extração, como nome e formato. Você pode personalizar o nome do arquivo usando atributos do banco de dados usando o editor de expressão."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Conteúdo"
>abstract="Nesta seção, especifique as colunas a serem exibidas no arquivo de extração. Depois de concluído, você pode obter uma pré-visualização do arquivo de extração usando o **Simular conteúdo** botão."

Para projetar o conteúdo do arquivo de extração gerado pelo delivery de correspondência direta, clique no link **[!UICONTROL Editar conteúdo]** na página de entrega e, em seguida, configure as propriedades e o conteúdo do arquivo.

## Configurar as propriedades do arquivo de extração {#properties}

1. No **[!UICONTROL Nome do arquivo]** especifique o nome desejado para o arquivo de extração. Você pode personalizar o nome do arquivo usando atributos do banco de dados. Para fazer isso, clique no link **[!UICONTROL Abrir caixa de diálogo de personalização]** ícone para abrir o editor de expressão. [Saiba como personalizar o conteúdo](../personalization/personalize.md)

1. No **[!UICONTROL Formato de arquivo]** escolha o formato desejado para o arquivo de extração; **Texto**, **Texto usando fixo com colunas**, **CSV (Excel)** ou **XML**.

1. Expanda a **[!UICONTROL Formato de extração]** para acessar opções específicas relacionadas ao formato do arquivo de extração. Os valores disponíveis dependem do formato selecionado.

+++ Opções de formato de extração disponíveis

   * **[!UICONTROL Usar a primeira linha como cabeçalho da coluna]** (Formato de texto / CSV (Excel)): ative essa opção para usar a primeira coluna como cabeçalho.
   * **[!UICONTROL Separador de colunas]** (Formato de texto): especifique o caractere a ser usado como separador de colunas no arquivo de extração.
   * **[!UICONTROL Delimitador de cadeia de caracteres]** (Formato de texto): especifique como delimitar strings no arquivo de extração.
   * **[!UICONTROL Fim da linha]** (Formato de texto): especifique como delimitar o final das linhas no arquivo de extração.
   * **[!UICONTROL Codificação]**: escolha a codificação do arquivo de extração.
   * **[!UICONTROL Formato de data e separadores]**: especifique como as datas devem ser formatadas no arquivo de extração.
   * **[!UICONTROL Formato de número]**: especifique como os números devem ser formatados no arquivo de extração.
   * **[!UICONTROL Exportar rótulos em vez de valores internos de enumerações]**: ative essa opção caso exporte valores de uma lista discriminada e deseje recuperar rótulos de colunas, que são mais fáceis de entender, em vez de IDs internas.

+++

1. Ative a **[!UICONTROL Quantidade solicitada]** opção para restringir o número de recipients do seu delivery.

   ![](assets/dm-content-details.png){zoomable=&quot;yes&quot;}

## Configurar as colunas do arquivo de extração {#content}

No **[!UICONTROL Conteúdo]** especifique as colunas a serem exibidas no arquivo de extração. Para fazer isso, siga estes passos:

1. Clique em **[!UICONTROL Adicionar atributo]** botão para criar uma nova coluna.
1. Escolha o atributo a ser exibido na coluna e confirme. Depois que a coluna é adicionada, você pode alterar seu rótulo e modificar o atributo associado usando o ícone de edição.
1. Repita essas etapas para adicionar quantas colunas forem necessárias para o arquivo de extração.
1. Para classificar o arquivo de extração usando uma das colunas, clique no ícone na **[!UICONTROL Classificação]** e selecione o método de classificação desejado.
1. Para alterar a posição de uma coluna, use as setas para cima e para baixo.

![](assets/dm-content-attributes.png)

Agora você pode visualizar o arquivo de extração e enviar o delivery para gerar o arquivo de extração. [Saiba como testar e enviar mensagens de correspondência direta](send-direct-mail.md)
