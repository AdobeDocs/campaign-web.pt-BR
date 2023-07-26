---
audience: end-user
title: Direcionar destinatários a partir de um arquivo
description: Saiba como usar destinatários de um arquivo externo para criar seu público-alvo de email
badge: label="Alfa"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 66%

---

# Carregar um público-alvo de email a partir de um arquivo {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Seleção de arquivo"
>abstract="Selecione o arquivo local a ser enviado. Os formatos compatíveis são TXT e CSV. Alinhe o formato de arquivo com o arquivo de amostra do link abaixo."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Definição de colunas"
>abstract="Verifique o formato das colunas a serem inseridas do seu arquivo local."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parâmetros de formatação"
>abstract="Verifique os parâmetros de formatação do arquivo."

É possível fazer upload de contatos de um arquivo externo. Os perfis não são adicionados ao banco de dados, mas todos os campos no arquivo de entrada estão disponíveis para [personalização](../personalization/gs-personalization.md). Os formatos de arquivo compatíveis são: texto (TXT) e valor separado por vírgula (CSV).

>[!CAUTION]
>
>* Esse recurso só está disponível para **deliveries de email independentes**. Ele não pode ser usado em workflows nem com deliveries SMS ou Push.
>
>* Não é possível usar [grupos de controle](control-group.md) ao carregar a população alvo a partir de um arquivo externo.


Para direcionar perfis de um arquivo local diretamente da interface de email, siga estas etapas:

1. Abrir um delivery de email existente, ou [criar um novo delivery de email](../email/create-email.md).
1. Na janela de criação da entrega de email, na seção **Público-alvo**, clique no botão **Selecionar público-alvo** e escolha a opção **Selecionar do arquivo**.

   ![](assets/select-from-file.png)

1. Selecione o arquivo local a ser enviado. O formato deve estar alinhado com o [arquivo de amostra](#sample-file).
1. Visualize e verifique como os dados estão mapeados na seção central da tela.
1. Escolha a coluna que contém o endereço de email do menu suspenso **Campo de endereço**. Também é possível selecionar a coluna lista de bloqueios se tiver essas informações no arquivo de entrada.
1. Ajuste as configurações da coluna e como formatar os dados a partir das opções disponíveis.
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
