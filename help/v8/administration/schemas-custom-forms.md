---
title: Trabalhar com formulários personalizados
description: Saiba como criar, editar e gerenciar registros em esquemas personalizados usando formulários de entrada de dados.
source-git-commit: be4876090ecaac853aaa88948505c444bef27ec2
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Trabalhar com formulários personalizados {#custom-forms}

Formulários personalizados são interfaces de entrada de dados que permitem gerenciar registros em esquemas personalizados diretamente da Interface do Usuário da Web. Cada formulário personalizado corresponde a um esquema personalizado específico e fornece uma exibição de lista para procurar registros e uma exibição de detalhes para criar, editar e excluir registros.

Os formulários personalizados são baseados na definição de formulário do esquema (definição de tela), que configura quais campos são exibidos e como eles são organizados.

>[!NOTE]
>
>Os formulários personalizados só estão disponíveis para esquemas que tenham uma definição de formulário configurada.

## Criar e publicar os esquemas personalizados {#form-schema}

Primeiro, você deve criar e publicar seus esquemas personalizados. Para obter instruções detalhadas, consulte esta [seção](schemas-create-publish.md).

Este é o modelo de dados usado para este exemplo:

* Um recipient faz várias compras
* Uma compra está vinculada a um produto
* Um produto está vinculado a uma marca

Para este caso de uso, três schemas são criados: Compras, Produtos e Esquemas de marca. Aqui está um exemplo:

![Formulários personalizados](assets/schemas-forms.png)

## Configurar a definição da tela {#form-screen-schema}

Defina quais campos serão exibidos e como serão organizados. Para obter instruções detalhadas, consulte esta [seção](schemas-browse-access.md#screen-def).

Este é um exemplo do esquema de marca ao qual a lista personalizada de produtos é adicionada. O formulário exibe a lista de produtos vinculados à marca.

![Formulários personalizados](assets/schemas-forms2.png)

Para o schema Produtos, adicionamos a lista personalizada Compras. E, para o schema de compras, os campos Product e Recipient.

## Criar entradas de navegação {#form-screen-entries}

Crie pastas no Explorer para acessar seu formulário personalizado. Para obter instruções detalhadas, consulte esta [seção](schemas-create-publish.md#navigation).

![Formulários personalizados](assets/schemas-forms3.png)

A exibição de lista exibe todos os registros desse esquema. Se o esquema tiver uma definição de formulário configurada, a lista será editável e você poderá criar, editar e excluir registros.
![Formulários personalizados](assets/schemas-forms4.png)

Em seguida, é possível:

* **Exibir e editar registros**: clique em um registro na exibição de lista para abri-lo diretamente na exibição detalhada e editar os campos.
* **Criar novos registros**: clique no botão **[!UICONTROL Criar]** e preencha os campos obrigatórios. Para campos vinculados, use o ícone de pesquisa para selecionar entre os registros relacionados disponíveis.
* **Excluir registros**: selecione um registro e use a ação de exclusão disponível nos detalhes do registro ou na exibição de lista.
* **Exibir dados relacionados em guias**: acesse registros relacionados por meio de guias dedicadas na exibição detalhada (por exemplo, exibir todos os produtos vinculados a uma marca ou todas as compras vinculadas a um produto).
* **Aplicar filtros**: use o painel de filtros para refinar o modo de exibição de lista e localizar registros específicos com base em qualquer campo do esquema.
* **Personalizar colunas de lista**: configure quais colunas são exibidas por padrão nos modos de exibição de lista por meio da definição de tela.
