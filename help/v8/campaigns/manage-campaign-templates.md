---
audience: end-user
title: Gerenciar modelos de campanha com o Adobe Campaign Web
description: Saiba como gerenciar modelos de campanha com o Adobe Campaign Web
badge: label="Beta"
source-git-commit: d9273f383e2301ea761ac67eeb47f6d9fd769d44
workflow-type: tm+mt
source-wordcount: '971'
ht-degree: 47%

---


# Gerenciar modelos de campanha{#manage-campaign-templates}

Todas as campanhas de marketing são baseadas em um modelo, que armazena as principais características e recursos. O Campaign vem com um conjunto de modelos integrados para ajudar você a começar. Você pode criar e configurar seus modelos de campanha e, em seguida, criar campanhas com base nesses modelos.

## Criar um template de campanha

Para criar um template de campanha, siga as etapas abaixo:

Abra o explorador do Campaign e navegue até Recursos > Modelos > Modelos de campanha.
Clique em New na barra de ferramentas acima da lista de modelos.


Você também pode duplicar o modelo incorporado para reutilizar e adaptar sua configuração. Para fazer isso, clique com o botão direito do mouse no template e selecione Duplicate.

Insira o rótulo do seu novo template de campanha.

Clique em Save e abra seu template novamente.

Na guia Edit, defina as propriedades do template.

Selecione Advanced campaign parameters... para adicionar um workflow ao seu template de campanha.



Altere o valor de Targeting and workflows para Yes e confirme. Saiba como adicionar funcionalidades nesta seção.

A guia Targeting and workflows é adicionada ao template. Clique em Add a workflow..., digite um Label e clique em Ok.

Crie o fluxo de trabalho de acordo com suas necessidades.



Clique em Salvar. Seu template está pronto para ser usado para criar uma nova campanha.

As várias guias e subguias do template de campanha permitem que você acesse as configurações, descritas em Configuração geral.

Selecionar módulos O link Advanced campaign parameters... permite habilitar e desabilitar tarefas para as campanhas com base neste template. Selecione os recursos que deseja habilitar nas campanhas criadas com base neste modelo.



Se uma funcionalidade não estiver selecionada, os elementos relativos ao processo (menus, ícones, opções, guias, subguias etc.) não aparecem na interface do template ou em campanhas baseadas nesse template. As guias à esquerda dos detalhes da campanha e as guias disponíveis coincidem com as funcionalidades selecionadas no template. Por exemplo, a funcionalidade Expenses and objetives não está habilitada, a guia correspondente a Budget não é exibida em campanhas baseadas no template.

Além disso, os atalhos para as janelas de configuração são adicionados ao painel de campanha. Quando uma funcionalidade é habilitada, um link direto dá acesso a ela a partir do painel de campanha.

Exemplos de configuração Por exemplo, com as seguintes configurações:



O painel de campanha mostra:



Observe que a guia Targeting and workflows está ausente.

As seguintes funcionalidades estão disponíveis:



Observe que a guia Budget está ausente.

As configurações avançadas do Campaign também refletem essa configuração.



Observe que a guia Aprovações não está disponível.

Com esta configuração:


O painel de campanha mostra:



Observe que a guia Targeting and workflows está disponível, mas o link Add a document está ausente.

As seguintes funcionalidades estão disponíveis:



Observe que a guia Orçamento está disponível.

As configurações avançadas do Campaign também refletem essa configuração.



Observe que a guia Approvals está disponível, mas as guias Control population e Seed addresses não estão habilitadas.

Tipologia dos módulos Grupo de controle

Quando este módulo está selecionado, uma guia adicional é adicionada às configurações avançadas do template e às campanhas baseadas nesse template. A configuração pode ser definida por meio do modelo ou individualmente para cada campanha. Saiba mais sobre grupos de controle nesta seção.



Seed addresses

Quando este módulo está selecionado, uma guia adicional é adicionada às configurações avançadas do template e às campanhas baseadas nesse template. A configuração pode ser definida por meio do template ou individualmente para cada campanha.



Documentos

Quando este módulo é selecionado, uma guia adicional é adicionada à guia Edit do template e às campanhas baseadas nesse template. Os documentos anexados podem ser adicionados do modelo ou individualmente para cada campanha. Saiba mais sobre documentos nesta seção.



Outline de entrega

Quando esse módulo é selecionado, uma subguia Delivery outlines é adicionada à guia Documents para definir delivery outlines para a campanha. Saiba mais sobre delivery outlines nesta seção.



Direcionamento e workflows

Quando você seleciona o módulo Targeting and workflows, uma guia é adicionada para permitir que você crie um ou mais workflows para campanhas com base nesse template. Os workflows também podem ser configurados individualmente para cada campanha com base neste modelo. Saiba mais sobre workflows da campanha nesta seção.



Quando esse módulo é habilitado, uma guia Jobs é adicionada às configurações avançadas da campanha para definir a sequência de execução do processo.

Aprovações

Se você ativar as Aprovações, será possível selecionar os processos que serão aprovados e os operadores de aprovação. Saiba mais sobre aprovações nesta seção.



Você pode optar por habilitar ou não a aprovação do processo por meio da guia Approvals da seção de configurações avançadas dos templates.

Despesas e objetivos

Quando esse módulo é selecionado, uma guia Budget é adicionada aos detalhes do template e às campanhas com base nesse template para que o orçamento associado possa ser selecionado.



Propriedades do template


Ao criar um template de campanha, você precisa inserir as seguintes informações:

Insira o rótulo do template: o rótulo é obrigatório e é o rótulo padrão para todas as campanhas com base neste template.
Selecione a natureza da campanha na lista suspensa. Os valores disponíveis nesta lista são os que foram salvos na lista discriminada natureOp.
Saiba como acessar e configurar suas listas discriminadas nesta página.

Selecione o tipo de campanha: exclusiva, recorrente ou periódica. Por padrão, os templates de campanha se aplicam a campanhas exclusivas. As campanhas recorrentes e periódicas são detalhadas nesta seção.

Especifique a duração da campanha, ou seja, o número de dias em que a campanha ocorrerá. Ao criar uma campanha com base nesse template, as datas de início e término da campanha serão preenchidas automaticamente.

Se a campanha for recorrente, você deverá especificar as datas de início e término da campanha diretamente no template.

Especifique o programa relacionado do template: campanhas baseadas neste template são vinculadas ao programa selecionado.

