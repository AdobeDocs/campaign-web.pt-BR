---
audience: end-user
title: Direcionar recipients de um arquivo
description: Saiba como usar recipients de um arquivo externo para criar seu público-alvo de email
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f60f0e34dc5d85808c208223d83d234e22a41c34
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 11%

---

# Carregar um público-alvo de email de um arquivo {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Seleção de arquivo"
>abstract="Selecione o arquivo a ser carregado. Os formatos compatíveis são TXT e CSV. Alinhe o formato de arquivo com o arquivo de amostra vinculado abaixo."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definição de colunas"
>abstract="Verifique o formato das colunas a serem inseridas do arquivo local."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parâmetros de formatação"
>abstract="Verifique os parâmetros de formatação do arquivo."

Você pode carregar contatos de um arquivo externo. Os perfis não são adicionados ao banco de dados, mas todos os campos no arquivo de entrada estão disponíveis para [personalização](../personalization/gs-personalization.md). Os formatos de arquivo compatíveis são: texto (TXT) e valor separado por vírgula (CSV).

>[!CAUTION]
>
>* Esse recurso só está disponível para **deliveries de email independentes**. Ele não pode ser usado em workflows nem com deliveries SMS ou Push.
>
>* Você não pode usar [grupos de controle](control-group.md) ao carregar a população do target de um arquivo externo.



Para direcionar perfis de um arquivo local diretamente da interface de email, siga estas etapas:

1. Abrir um delivery de email existente, ou [criar um novo delivery de email](../email/create-email.md).
1. Na janela de criação de delivery de email, no **Público** clique na guia **Selecionar público** e escolha o botão **Selecionar do arquivo** opção.

   ![](assets/select-from-file.png)

1. Selecione o arquivo a ser carregado. O formato deve estar alinhado com o [arquivo de amostra](#sample-file).
1. Visualize e verifique como os dados são mapeados na seção central da tela.
1. Escolha a coluna que contém o endereço de email da **Campo de endereço** menu suspenso. Você também pode selecionar a coluna incluir na lista de bloqueios se tiver essas informações no arquivo de entrada.
1. Ajuste as configurações de coluna e como formatar dados a partir das opções disponíveis.
1. Clique em **Confirmar** assim que as configurações estiverem corretas.

Ao criar e personalizar o conteúdo da mensagem, você pode selecionar campos do arquivo de entrada na [Editor de personalização](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## Arquivo de amostra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Arquivo de amostra"
>abstract="Formatos de arquivo compatíveis: txt, csv. Usar a primeira linha como cabeçalho da coluna."

Os formatos compatíveis são TXT e CSV. A primeira linha é o cabeçalho da coluna.

Alinhe o formato de arquivo com o arquivo de amostra abaixo:

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
