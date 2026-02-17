---
title: Sobre schemas
description: Saiba como trabalhar com esquemas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 6%

---

# Sobre schemas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Esquemas"
>abstract="O Adobe Campaign usa esquemas baseados em XML para definir a estrutura física e lógica dos dados no aplicativo. Nesta tela, você pode exibir todos os esquemas existentes, acessar detalhes do esquema, configurar formulários personalizados e criar ou estender esquemas diretamente da Interface do Usuário da Web."

O **[!DNL Adobe Campaign]** usa esquemas baseados em XML para definir a estrutura física e lógica dos dados no aplicativo. Um esquema é um documento XML vinculado a uma tabela de banco de dados que define:

* A estrutura da tabela SQL, incluindo nome da tabela, campos e relacionamentos.
* A estrutura de dados XML, incluindo elementos, atributos, hierarquia, tipos, valores padrão e rótulos.

Os esquemas desempenham um papel fundamental em:

* Mapeamento de dados do aplicativo para tabelas do banco de dados.
* Definição de relações entre objetos de dados.
* Especificação da estrutura e das propriedades de cada campo.

Cada entidade no Adobe Campaign tem um esquema dedicado, garantindo a consistência e a organização dos dados.

A interface de schemas permite:

* [Acessar e personalizar esquemas](schemas-browse-access.md) - Exibir esquemas disponíveis, explorar seus detalhes e personalizar a exibição da tela
* [Configurar colunas de lista](schemas-list-columns.md) - Configure quais colunas são exibidas por padrão nos modos de exibição de lista.
* [Editar campos personalizados](schemas-custom-fields.md) - Configure quais campos personalizados serão exibidos em telas de detalhes e organize-os em seções.
* [Adicionar listas de coleções](schemas-collection-lists.md) - Adicione listas de coleções para mostrar dados relacionados em telas de perfil.
* [Criar e gerenciar esquemas](schemas-create-publish.md#create-schemas) - Criar novos esquemas e estender os existentes
* [Publicar e sincronizar esquemas](schemas-create-publish.md#publish) - Sincronize as alterações de esquema com a estrutura do banco de dados.
* [Trabalhar com formulários personalizados](schemas-custom-forms.md) - Criar, editar e gerenciar registros em esquemas personalizados usando formulários de entrada de dados.

>[!NOTE]
>
>Você precisa ter direitos de administrador para gerenciar esquemas.

Informações detalhadas sobre esquemas estão disponíveis na [documentação do console do Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.
