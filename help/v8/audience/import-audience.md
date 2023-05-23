---
audience: end-user
title: Direcionar recipients de um arquivo
description: Saiba como usar recipients de um arquivo externo para criar seu público-alvo de email
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 34%

---

# Direcionar recipients de um arquivo {#audience-from-file}

Você pode carregar contatos de um arquivo externo. Esse recurso só está disponível para deliveries de email. Os formatos compatíveis são: arquivo de texto (TXT) ou arquivo de valores separados por vírgula (CSV). Eles serão adicionados ao banco de dados.

>[!NOTE]
>
>Você pode criar um workflow de importação para adicionar ou atualizar vários perfis.  Saiba mais


Para direcionar perfis de um arquivo local diretamente da interface do, siga estas etapas:

1. Na janela de criação de delivery de email, clique no link **Selecionar público** e selecione o botão **Selecionar do arquivo** opção.

   ![](assets/select-from-file.png)

1. Selecione o arquivo a ser carregado.
1. Visualize como os dados são mapeados na seção central da tela.
1. Escolha a coluna que contém o endereço de email da **Campo de endereço** menu suspenso.
1. Ajuste as configurações de coluna e como formatar dados a partir das opções disponíveis.
1. Clique em **Confirmar** assim que as configurações estiverem corretas.

Ao criar e personalizar o conteúdo da mensagem, você pode selecionar campos do arquivo de entrada no Editor de personalização.

![](assets/select-external-perso.png)

## Arquivo de amostra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Arquivo de amostra"
>abstract="Formatos de arquivo compatíveis: txt, csv. Usar a primeira linha como cabeçalho da coluna."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
