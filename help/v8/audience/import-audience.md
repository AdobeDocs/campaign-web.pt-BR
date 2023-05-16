---
audience: end-user
title: Importar recipients de um arquivo
description: Saiba como importar recipients de um arquivo externo
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 97%

---

# Importar recipients de um arquivo {#audience-from-file}

Você pode adicionar ou atualizar contatos da interface de entrega, carregando um arquivo de texto (TXT) ou um arquivo de valores separados por vírgulas (CSV). Eles serão adicionados ao banco de dados.

>[!NOTE]
>
>Você também pode criar um fluxo de trabalho de importação para adicionar ou atualizar vários perfis.


Para adicionar perfis de um arquivo local diretamente da interface, siga estas etapas:

1. Na janela de criação da entrega, clique no botão **Selecionar público** e escolha a opção **Selecionar do arquivo**.
1. Selecione o arquivo a ser carregado.
1. Defina as configurações da coluna e como formatar dados. É possível ignorar uma coluna usando o botão de alternância **Ignorar coluna**.
1. Visualize como os dados são mapeados na seção central da tela.
1. Clique em **Confirmar** assim que as configurações estiverem corretas.

Ao criar e personalizar o conteúdo da mensagem, você pode selecionar campos do arquivo de entrada no Editor de personalização.

## Arquivo de amostra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Arquivo de amostra"
>abstract="Formatos de arquivo compatíveis: txt, csv. Usar a primeira linha como cabeçalho da coluna."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
