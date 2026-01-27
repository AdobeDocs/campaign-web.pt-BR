---
audience: end-user
title: Gerenciar marca
description: Saiba como criar e gerenciar as diretrizes da sua marca
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 3%

---

# Criar e gerenciar suas marcas {#brands}

As diretrizes da marca são um conjunto abrangente de regras e padrões que definem a identidade visual e verbal de uma marca. Eles servem como referência para garantir uma representação de marca consistente em todos os canais de marketing e comunicação.

No [!DNL Adobe Campaign Web], os usuários podem inserir e organizar manualmente informações da marca ou carregar documentos de diretrizes da marca para extração automática de dados.

## Acessar marcas {#generative-access}

Para acessar o menu **[!UICONTROL Marcas]** no [!DNL Adobe Campaign Web], os usuários devem receber os perfis de produto **[!UICONTROL Administrador (administrador)]** e **[!UICONTROL Kit de marcas]** para criar e gerenciar marcas. Para acesso somente leitura, os usuários precisam do perfil de produto [!UICONTROL Assistente de IA]. [Saiba mais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Saiba como atribuir permissões relacionadas à marca

1. Na página inicial do [Admin Console](https://adminconsole.adobe.com/enterprise), acesse seu produto do Campaign.

   ![Página inicial do Admin Console mostrando o acesso ao produto do Campaign](assets/brands_admin_1.png)

1. Selecione o **[!DNL Product profile]** com base no nível de permissões que você deseja conceder ao usuário.

   ![Seleção do perfil de produto no Admin Console](assets/brands_admin_2.png)

1. Clique em **[!DNL Add users]** para atribuir o perfil de produto selecionado.

   ![Opção Adicionar usuários no Admin Console](assets/brands_admin_3.png)

1. Digite seu nome de usuário, grupo de usuários ou endereço de email.

1. Clique em **Salvar** para aplicar as alterações.

Os usuários já atribuídos a esta função têm suas permissões automaticamente atualizadas.

+++

## Crie sua marca {#create-brand-kit}

Para criar e gerenciar as diretrizes da sua marca, siga as etapas abaixo.

Os usuários podem inserir os detalhes manualmente ou fazer upload de um documento de diretrizes de marca para extrair as informações automaticamente:

1. No menu **[!UICONTROL Marcas]**, clique em **[!UICONTROL Criar marca]**.

   ![Menu Marcas com a opção Criar marca](assets/brands-1.png)

1. Digite um **[!UICONTROL Nome]** para sua marca.

1. Arraste e solte ou selecione seu arquivo para fazer upload das diretrizes da marca e extrair automaticamente informações relevantes sobre a marca. Clique em **[!UICONTROL Criar marca]**.

   O processo de extração de informações agora começa. Observe que pode levar vários minutos para ser concluído.

   ![Carregamento de arquivo para extração de diretrizes de marca](assets/brands-2.png)

1. Seus padrões de criação de conteúdo e visual agora são preenchidos automaticamente. Navegue pelas diferentes guias para adaptar as informações conforme necessário. [Saiba mais](#personalize)

1. No menu avançado de cada seção ou categoria, você pode adicionar referências para extrair automaticamente informações relevantes sobre a marca.

   Para remover conteúdo existente, use as opções **[!UICONTROL Limpar seção]** ou **[!UICONTROL Limpar categoria]**.

   ![](assets/brands-15.png)

1. Após a configuração, clique em **[!UICONTROL Salvar]** e em **[!UICONTROL Publicar]** para disponibilizar a diretriz de marca no Assistente de IA.

1. Para fazer modificações na sua marca publicada, clique em **[!UICONTROL Editar marca]**.

   >[!NOTE]
   >
   >Isso cria uma cópia temporária no modo de edição, substituindo a versão online depois de publicada.

   ![Opção Editar marca no menu Marcas](assets/brands-8.png)

1. No painel **[!UICONTROL Marcas]**, abra o menu avançado clicando no ícone ![](assets/do-not-localize/Smock_More_18_N.svg) para:

   * Exibir marca
   * Editar
   * Marcar como marca padrão
   * Duplicar
   * Publicação
   * Cancelar publicação
   * Excluir

   ![Opções de menu avançadas no painel Marcas](assets/brands-6.png)

As diretrizes de marca agora podem ser acessadas no menu suspenso **[!UICONTROL Marca]** do Assistente de IA. Isso permite que o Assistente de IA gere conteúdo e ativos alinhados às suas especificações. [Saiba mais sobre o Assistente de IA](../content/generative-gs.md)

Você também pode usar as diretrizes da marca para avaliar a qualidade do conteúdo e o alinhamento da marca. [Saiba mais sobre a validação de qualidade do conteúdo](brands-score.md#validate-quality)

![Menu do assistente de IA com o menu suspenso Marca](assets/brands_6.png)

### Definir uma marca padrão {#default-brand}

Você pode designar uma marca padrão a ser aplicada automaticamente ao gerar conteúdo e calcular pontuações de alinhamento durante a criação da campanha.

Para definir uma marca padrão, vá para o painel **[!UICONTROL Marcas]**. Abra o menu avançado clicando no ícone ![](assets/do-not-localize/Smock_More_18_N.svg) e selecione **[!UICONTROL Marcar como marca padrão]**.

![Opções de menu avançadas no painel Marcas](assets/brands-6.png)

