---
audience: end-user
title: Carregar um público-alvo de email a partir de um arquivo
description: Saiba como carregar perfis de um arquivo externo para criar seu público-alvo de email
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 28%

---

# Carregar um público-alvo de email a partir de um arquivo {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Seleção de arquivo"
>abstract="Selecione o arquivo local a ser enviado. Os formatos compatíveis são TXT e CSV. Alinhe o formato de arquivo com o arquivo de amostra do link abaixo."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definição de colunas"
>abstract="Verifique o formato das colunas no arquivo externo."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parâmetros de formatação"
>abstract="Especifique como o arquivo externo está formatado para garantir que os dados sejam importados corretamente."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Visualizar seu arquivo"
>abstract="Verifique a visualização das colunas do arquivo externo. Essa tela mostra um máximo de 30 registros."

A interface da Web do Adobe Campaign permite direcionar perfis armazenados em um arquivo externo. Após carregar os perfis, todos os campos do arquivo de entrada estarão disponíveis para uso na personalização da entrega [Saiba como personalizar o conteúdo](../personalization/personalize.md).

Perfis do arquivo de entrada não são adicionados ao banco de dados. Eles são carregados e disponibilizados somente para esse delivery de email independente específico.

>[!NOTE]
>
>Esta página descreve como carregar perfis externos de um arquivo ao criar um delivery de email independente. Para carregar dados de um arquivo no contexto de um workflow, consulte [esta página](../workflows/activities/load-file.md).

## Leitura obrigatória {#must-read}

* Este recurso está disponível somente para **entregas de email**.
* Os formatos de arquivo compatíveis são: texto (TXT) e valor separado por vírgula (CSV).
* Não é possível usar [grupos de controle](control-group.md) ao carregar a população alvo a partir de um arquivo externo.

## Selecionar e configurar o arquivo de entrada {#upload}

Para direcionar perfis de um arquivo em seus emails, siga estas etapas:

1. Abra uma entrega de email existente ou [crie uma nova entrega de email](../email/create-email.md).
1. Na seção **Público**, clique no botão **Selecionar público-alvo** e escolha **Selecionar do arquivo**.

   ![](assets/select-from-file.png){zoomable="yes"}

1. Selecione o arquivo local a ser carregado. O formato de arquivo deve estar alinhado com o [arquivo de exemplo](#sample-file).
1. Visualize e verifique como os dados estão mapeados na seção central da tela.

   ![](assets/select-from-file-map.png)

1. Especifique a coluna que contém o endereço de email da lista suspensa **Campo de Endereço**. Também é possível selecionar a coluna lista de bloqueios se tiver essas informações no arquivo de entrada.
1. Ajuste as configurações de coluna e como formatar os dados a partir das opções disponíveis.
1. Clique em **Confirmar** assim que as configurações estiverem corretas.

Ao criar o conteúdo da mensagem, você pode adicionar personalização aproveitando os campos do arquivo de entrada. [Saiba como personalizar conteúdo](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable="yes"}

## Arquivo de amostra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Carregar um público-alvo de um arquivo"
>abstract="Os formatos de arquivo compatíveis são TXT e CSV. Usar a primeira linha como cabeçalho da coluna. Alinhe seu formato de arquivo com o arquivo de amostra fornecido no link abaixo."

Ao carregar um arquivo externo para direcionar perfis em seus deliveries, verifique se o arquivo de entrada corresponde às recomendações abaixo:

* Os formatos compatíveis são TXT e CSV.
* A primeira linha do arquivo é o cabeçalho da coluna.
* Alinhe o formato de arquivo com o arquivo de amostra abaixo:

  ```javascript
  {
  lastname,firstname,city,birthdate,email,denylist
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
  }
  ```

## Pré-visualizar e testar o email {#test}

O Campaign Web permite visualizar e enviar provas ao usar um público-alvo carregado de um arquivo. Para fazer isso, siga estes passos:

1. Clique no botão **[!UICONTROL Simular conteúdo]** da tela de edição de conteúdo da entrega e clique no botão **[!UICONTROL Adicionar perfil(s) de teste]**.

1. Os perfis contidos no arquivo carregado são exibidos. Selecione o(s) perfil(is) que deseja usar para visualizar seu conteúdo e clique em **[!UICONTROL Selecionar]**.

1. Uma pré-visualização do conteúdo do delivery é exibida no painel direito da tela. Os elementos personalizados são substituídos pelos dados do perfil selecionado no painel esquerdo. [Saiba mais sobre a visualização do conteúdo da entrega](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable="yes"}

1. Para enviar provas, clique no botão **[!UICONTROL Enviar prova]**.

1. Clique no botão **[!UICONTROL Carregar perfis de prova]** e selecione o arquivo .txt ou .csv que contém os destinatários de prova.

   >[!CAUTION]
   >
   >Verifique se o formato do arquivo corresponde ao usado para fazer upload do seu público-alvo. Quaisquer erros de formato exibirão um alerta.

1. Quando os perfis de prova forem adicionados e você estiver pronto para enviar as provas, clique no botão **[!UICONTROL Enviar prova]** e confirme o envio.

   ![](assets/file-upload-test.png){zoomable="yes"}

1. Você pode monitorar o envio da prova usando o botão **[!UICONTROL Exibir provas]** a qualquer momento. [Saiba mais sobre o monitoramento de provas](../preview-test/test-deliveries.md#access-test-deliveries)
