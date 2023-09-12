---
audience: end-user
title: Direcionar destinatários a partir de um arquivo
description: Saiba como usar destinatários de um arquivo externo para criar seu público-alvo de email
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ed9d67c5d84826035785e9543f4ed7655aa094f1
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 50%

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

## Fazer upload do arquivo {#upload}

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

## Pré-visualizar e testar seu email {#test}

O Campaign Web permite visualizar e enviar emails de teste ao usar um público-alvo carregado de um arquivo. Para fazer isso, siga estes passos:

1. Simular conteúdo
1. Abre a visualização. Clique em selecionar perfil(is): selecione os perfis no arquivo a ser usado
1. para enviar email de teste, clique em testar
1. modo de teste: definir o target das provas
1. Fazer upload do target do email de teste de um segundo arquivo (ou usar o mesmo). a formatação do arquivo segue a mesma do arquivo carregado
1. Verificações realizadas no formato de arquivo
1. clique em enviar

+ link para visualizar e testar a seção

**perguntas:**
* nenhuma substituição do arquivo disponível?

## Arquivo de amostra {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Carregar um público-alvo de um arquivo"
>abstract="Os formatos de arquivo compatíveis são TXT e CSV. Usar a primeira linha como cabeçalho da coluna. Alinhe seu formato de arquivo com o arquivo de amostra fornecido no link abaixo."

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
