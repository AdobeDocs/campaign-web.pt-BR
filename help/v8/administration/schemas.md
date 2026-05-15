---
title: Sobre esquemas
description: Saiba como trabalhar com esquemas.
exl-id: 1433a441-1673-45a2-9fec-be9550fbba0d
TQID: https://experienceleague.adobe.com/D7gEyOdvyADCac9T3By3KKnx7kpN8LuE2-rnRBJDyMA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: b82389f8-9b5e-4083-8e3b-3cef299fb8b9
subfeature_v2:
  - id: cfc95e9b-b035-4403-a6a9-b27a8a053a37
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5a231f1dc49379d1be5d36e1732660111f851649
workflow-type: tm+mt
source-wordcount: 319
ht-degree: 32%

---

# Sobre esquemas {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Criação de esquema"
>abstract="Agora você pode criar e gerenciar esquemas diretamente da interface do Campaign Web. Você pode criar novas tabelas, estender esquemas existentes e criar formulários personalizados."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Esquemas"
>abstract="O Adobe Campaign usa esquemas baseados em XML para definir a estrutura física e lógica dos dados no aplicativo. Nesta tela, é possível exibir todos os esquemas, acessar detalhes do esquema, configurar formulários personalizados e criar ou estender esquemas diretamente da interface do usuário da Web."

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
