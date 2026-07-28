---
title: 'Configurar opções do  [!DNL Campaign] '
description: Saiba como configurar as opções do Campaign e criar suas próprias opções personalizadas.
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
TQID: https://experienceleague.adobe.com/a3MU21qEI7ggDv-gUT4--glIkWdU05mz14v3U9Q2wnM
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0638cc11f533521f7c8f3df3a80361b040a05b0c
workflow-type: tm+mt
source-wordcount: 592
ht-degree: 4%

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

>[!IMPORTANT]
>As opções integradas são pré-configuradas e só devem ser modificadas por usuários avançados. Em caso de dúvidas ou solicitações, entre em contato com o representante da Adobe.

## Acessar opções do Campaign {#access}

Opções disponíveis no menu **[!UICONTROL Administração]** / **[!UICONTROL Opções]**. Use o painel de filtros para restringir a lista e localizar rapidamente a opção necessária.

![](assets/options-list.png)\
[Lista de opções exibida no menu Administração/Opções]

>[!NOTE]
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

## Restringir o endereço de email do remetente para entregas {#restrict-sender-address}

Por padrão, os profissionais de marketing podem digitar qualquer endereço no campo **[!UICONTROL Do email]** de uma entrega de email. Para restringir esse campo a uma lista predefinida de endereços, crie ou edite a opção `NmsDelivery_senderAddressMask` interna e defina seu valor como uma lista separada por vírgulas dos endereços de remetente permitidos, por exemplo `abc@adobe.com,bcd@adobe.com`.

![Opção para restringir valores no menu De](assets/option-restrict-from.png)

Depois que esta opção tiver um valor, o campo **[!UICONTROL Do email]** se tornará uma lista suspensa contendo apenas esses endereços, em vez de um campo de texto livre. Se a opção não existir ou seu valor estiver vazio, o campo permanecerá como texto livre, como antes.

![Valores disponíveis em um email](assets/option-restrict-from2.png)

Essa restrição é global. Ela se aplica a todas as marcas e modelos de entrega e não aceita campos de personalização, somente endereços estáticos.

Para obter mais informações sobre o campo **[!UICONTROL Do email]**, consulte [Configurar o conteúdo do email](../email/edit-content.md#edit-content).
