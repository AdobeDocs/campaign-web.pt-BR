---
audience: end-user
title: Criar um delivery de correspondência direta
description: Saiba como projetar seu delivery de correspondência direta com o Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: 60484d08a68a5caaf91074c9ce543d8a44d44ab7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 21%

---

# Criar o arquivo de extração {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Conteúdo do arquivo de extração"
>abstract="Clique no botão **Editar conteúdo** para iniciar a criação do arquivo de extração exigido pelo seu provedor de correspondência direta. Isso permite definir as propriedades do arquivo, como rótulo e formato, e especificar as colunas que deseja incluir no arquivo."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Propriedades do arquivo"
>abstract="Configure as propriedades do arquivo de extração, como nome e formato. É possível personalizar o nome do arquivo usando atributos do banco de dados com o editor de expressão."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Conteúdo"
>abstract="Nesta seção, especifique as colunas a serem exibidas no arquivo de extração. Depois de concluído, é possível obter uma visualização do arquivo de extração usando o botão **Simular conteúdo**."

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

   ![](assets/dm-content-details.png){zoomable="yes"}

## Configurar as colunas do arquivo de extração {#content}

No **[!UICONTROL Conteúdo]** especifique as colunas a serem exibidas no arquivo de extração. Para fazer isso, siga estes passos:

1. Clique em **[!UICONTROL Adicionar atributo]** botão para criar uma nova coluna.
1. Escolha o atributo a ser exibido na coluna e confirme. Observe que você pode aproveitar o editor de expressão para selecionar o atributo a ser usado clicando no botão **[!UICONTROL Editar expressão]** botão.

   ![](assets/dm-add-attribute.png)

1. Depois que a coluna é adicionada, você pode alterar seu rótulo e modificar o atributo associado usando o ícone de edição.
1. Repita essas etapas para adicionar quantas colunas forem necessárias para o arquivo de extração.
1. Para classificar o arquivo de extração usando uma das colunas, clique no ícone na **[!UICONTROL Classificação]** e selecione o método de classificação desejado.
1. Para alterar a posição de uma coluna, use as setas para cima e para baixo.

![](assets/dm-content-attributes.png)

Agora você pode visualizar o arquivo de extração e enviar o delivery para gerar o arquivo de extração. [Saiba como testar e enviar mensagens de correspondência direta](send-direct-mail.md)
