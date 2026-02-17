---
title: Criar e publicar esquemas
description: Saiba como criar, estender e publicar esquemas.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Criar e publicar esquemas {#create-publish}

## Criar e gerenciar esquemas {#create-schemas}

Você pode criar novos esquemas, estender esquemas existentes e acessar bancos de dados externos.

### Criar ou estender um esquema {#create-new}

Para criar ou estender um esquema:

1. Navegue até **[!UICONTROL Administração]** > **[!UICONTROL Esquemas]**.
1. Clique em **[!UICONTROL Criar esquema]**.

   ![Caixa de diálogo de criação do esquema](assets/schemas-create1.png)

1. Insira um namespace para o esquema (por exemplo, `cus` para esquemas personalizados).
1. Insira um nome e rótulo exclusivos e escolha se deseja criar um novo esquema ou estender um existente.

1. Clique em **[!UICONTROL Create]**.
   ![Caixa de diálogo de criação do esquema](assets/schemas-create2.png)

O schema é criado e a estrutura do schema gerada é exibida.

Por padrão, o schema está vazio. Agora é necessário adicionar os campos que deseja incluir no esquema usando o editor de esquemas:

1. Clique no ícone de lápis na seção **[!UICONTROL Conteúdo]** da tela de detalhes do esquema.
2. Adicione os elementos necessários e salve. Este é um exemplo de estrutura de esquema personalizada:

   ![Caixa de diálogo de criação do esquema](assets/schemas-create3.png)

O sistema valida automaticamente a estrutura XML e gera o schema.

### Definir a edição de tela {#define-attributes}

Depois de criar o schema, você precisa definir a edição da tela.

Para obter mais informações sobre a tela de definição de tela e como acessá-la, consulte a seção [Acessar a definição de tela](schemas-browse-access.md#screen-def).

No nosso exemplo, simplesmente adicionamos dois campos personalizados:

1. Clique no botão **[!UICONTROL Edição da tela]** na exibição de detalhes do esquema para acessar a definição da tela.

1. Clique no ícone de reticências acima da tabela **[!UICONTROL Lista de campos personalizados]** e escolha **[!UICONTROL Selecionar atributos]**.
1. Selecione os campos personalizados que deseja adicionar e confirme.

   ![Caixa de diálogo de criação do esquema](assets/schemas-create4.png)

## Publicar e sincronizar esquemas {#publish}

Depois de criar ou modificar um esquema, você precisa publicá-lo para sincronizar o esquema lógico com a estrutura do banco de dados físico.

### Publicar alterações no esquema {#publish-changes}

>[!CAUTION]
>
>A publicação de alterações de esquema modifica a estrutura do banco de dados. Entenda o impacto dessas alterações antes de confirmar a publicação.

Para publicar suas alterações de esquema:

1. Navegue até **[!UICONTROL Administração]** > **[!UICONTROL Esquemas]** para acessar a lista de esquemas.
1. Clique em **[!UICONTROL Publicação]** e confirme.

   ![Caixa de diálogo de publicação de esquema mostrando as alterações a serem aplicadas](assets/schemas-publish1.png)

1. Selecione, na lista, o schema que deseja sincronizar.

   ![Caixa de diálogo de publicação de esquema mostrando as alterações a serem aplicadas](assets/schemas-publish2.png)

1. Revise o script SQL que será executado para atualizar a estrutura do banco de dados.
1. Clique em **[!UICONTROL Publicar]** e confirme para continuar com a publicação.

>[!NOTE]
>
>O processo pode levar algum tempo, dependendo do tamanho do banco de dados e da complexidade das alterações.

### Criar uma entrada de navegação {#navigation}

Depois de publicar um esquema personalizado, você pode criar uma entrada de navegação no Explorer para acessar seus dados personalizados:

1. Navegue até o menu **[!UICONTROL Explorer]** e selecione uma pasta onde deseja colocar seu esquema personalizado.
1. Clique no ícone de reticências e em **[!UICONTROL Criar nova pasta]**.
   ![Criação de entrada de navegação para esquema personalizado](assets/schemas-publish3.png)
1. Adicione um rótulo e escolha o esquema no campo **[!UICONTROL Tipo de pasta]**.
   ![Criação de entrada de navegação para esquema personalizado](assets/schemas-publish5.png)
1. O esquema personalizado agora estará acessível no modo de exibição **[!UICONTROL Explorer]**.

Na nova pasta, é possível:

* Visualize a lista de registros no esquema personalizado.
* Criar novos registros.
* Editar e excluir registros existentes.
* Personalize quais colunas são exibidas por padrão na exibição de lista.
