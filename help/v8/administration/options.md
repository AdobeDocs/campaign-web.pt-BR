---
title: 'Configurar opções do  [!DNL Campaign] '
description: Saiba como configurar as opções do Campaign e criar suas próprias opções personalizadas.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 5%

---

# Configurar opções do [!DNL Campaign] {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="Opções"
>abstract="Opções"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="Criar opção"
>abstract="Criar opção"

O Adobe Campaign Web inclui opções técnicas que permitem configurar o aplicativo mais especificamente. Algumas dessas opções são incorporadas, enquanto outras podem ser adicionadas manualmente, conforme necessário.

>[!IMPORTANT]\
>As opções integradas são pré-configuradas e só devem ser modificadas por usuários avançados. Em caso de dúvidas ou solicitações, entre em contato com o representante da Adobe.

## Acessar opções do Campaign {#access}

Opções disponíveis no menu **[!UICONTROL Administração]** / **[!UICONTROL Opções]**. Use o painel de filtros para restringir a lista e localizar rapidamente a opção necessária.

![](assets/options-list.png)\
[Lista de opções exibida no menu Administração/Opções]

>[!NOTE]\
>Embora o local do menu de opções seja diferente entre o console do Adobe Campaign e a interface do usuário da Web, a lista é idêntica e funciona como um espelho. Para obter mais detalhes sobre as opções disponíveis, consulte a lista de opções na [documentação do Campaign v7](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}.

Na lista de opções, é possível:

* **Duplique ou exclua uma opção**: clique no botão de reticências e selecione a ação desejada.
* **Modificar uma opção**: clique no nome da opção para abrir suas propriedades. Faça as alterações e salve.
* **Criar uma opção personalizada**: clique no botão **[!UICONTROL Criar opção]**.

## Criar uma opção {#create}

A interface da Web do Adobe Campaign permite criar opções personalizadas para atender aos seus requisitos. Isso é particularmente útil ao trabalhar com atividades de fluxo de trabalho de **[!UICONTROL código JavaScript]** para armazenar dados intermediários.

Para criar uma opção:

1. Acesse a lista de opções e clique em **[!UICONTROL Criar opção]**.
1. Insira um nome para a opção, selecione seu tipo e defina o valor desejado.
1. Clique em **[!UICONTROL Criar]** para criar a opção.

![Criar interface de opção mostrando campos para nome, tipo e valor](assets/options-create.png)

As opções podem atuar como armazenamento temporário para dados, oferecendo os seguintes benefícios:

* Valores digitados: as opções são compatíveis com tipos de dados específicos, como datas, números inteiros, cadeias de caracteres etc.
* Flexibilidade: as opções permitem que os usuários armazenem e recuperem dados com eficiência sem a sobrecarga do gerenciamento de tabelas de banco de dados.

No exemplo abaixo, uma opção personalizada chamada `sampleOption` é criada com o valor inicial &quot;a&quot;. Uma atividade **[!UICONTROL JavaScript code]** em um fluxo de trabalho modifica o valor desta opção e o armazena em uma variável. O valor atualizado é exibido nos logs de fluxo de trabalho e refletido no menu **[!UICONTROL Opções]**.

1. Crie a opção.

   ![Interface de criação de opção personalizada mostrando o nome `sampleOption` e o valor inicial &quot;a&quot;](assets/options-sample-create.png)

1. Configure uma atividade **[!UICONTROL JavaScript code]** e inicie o fluxo de trabalho.

   ![Interface de configuração da atividade do código JavaScript](assets/options-sample-javascript.png)

1. Execute o workflow para ver o valor atualizado nos logs de workflow.

   ![Logs de fluxo de trabalho mostrando o valor atualizado da opção personalizada](assets/options-sample-logs.png)

1. O valor atualizado agora está visível no menu **[!UICONTROL Opções]**.

   ![Menu Opções exibindo o valor atualizado da opção personalizada](assets/options-sample-updated.png)