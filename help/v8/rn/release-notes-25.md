---
title: Notas de versão anteriores da interface do Campaign v8 Web
description: Versões de 2025 da interface do Campaign Web
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 8ec342d565bc8418c202cdba834d74a99cff3a47
workflow-type: tm+mt
source-wordcount: '1281'
ht-degree: 98%

---

# Notas de versão de 2025 {#2025-release}

Esta página lista todas as alterações e melhorias disponíveis com as **versões de 2025**. As notas de versão mais recentes estão disponíveis [nesta página](release-notes.md).

## Versão de abril de 2025 {#25-4-release}

**Data de lançamento**: 29 de abril de 2025

### Novos recursos {#25-4-features}

Os seguintes recursos estão disponíveis para todos os usuários a partir da versão de abril.

<table>
<thead>
<tr>
<th><strong>Canal da central de atendimento</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O canal da central de atendimento já está disponível na interface do usuário da web do Campaign. Este canal se refere a um método de comunicação usado para gerenciar e rastrear comunicações ou interações realizadas por meio de uma central de atendimento, normalmente, chamadas telefônicas feitas por agentes para clientes ou clientes potenciais.</p>
<p>Observação: os relatórios não estão disponíveis na interface do usuário da Web para o canal da central de atendimento. Você deve navegar até o Console do cliente para acessar os relatórios.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Para obter mais informações, consulte a <a href="../call-center/gs-call-center.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Novo construtor de regras</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Um novo construtor de regras agora está disponível para ajudar você a definir condições complexas em uma interface aprimorada. Você pode alternar do construtor de regras antigo para o novo, conforme necessário.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Para obter mais informações, consulte a <a href="../query/query-modeler-overview.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criação de conta externa</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Como administrador do Campaign, agora você pode configurar novas conexões com sistemas externos por meio da interface do Campaign Web.
Você também pode exibir, atualizar e gerenciar contas externas existentes.</p>
<p>Para obter mais informações, consulte a <a href="../administration/external-account.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Melhorias {#25-4-improvements}

**Melhorias gerais na interface**

* A descrição do Campo, as opções “Adicionar aos favoritos” e “Distribuição de valores” para atributos de esquema agora estão mais visíveis na interface. Para obter mais informações, consulte a [documentação detalhada](../get-started/attributes.md).
* Na interface, a data e a hora agora são exibidas de acordo com o idioma principal definido nas preferências da Experience League. Esta melhoria está disponível apenas para alguns idiomas. Para ver a lista completa dos idiomas compatíveis, consulte a [documentação detalhada](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Editor de email**: para aprimorar a acessibilidade na interface do Campaign Web, dois novos campos agora estão disponíveis no Designer de email: eles correspondem ao elemento `title` e ao atributo lang no elemento `html` do seu conteúdo de email. É possível definir essas configurações além do campo Pré-cabeçalho, na seção Corpo do email. Para obter mais informações, consulte a [documentação detalhada](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Esquemas**

* Agora é possível editar o esquema temporário de uma lista na interface do Campaign Web. Para obter mais informações, consulte a [documentação detalhada](../audience/manage-audience.md).
* Agora você pode visualizar os campos personalizados de um esquema em uma tela de amostra. Para obter mais informações, consulte a [documentação detalhada](../administration/custom-fields.md#add).
* Agora é possível mover campos personalizados na lista usando a função arrastar e soltar. Para obter mais informações, consulte a [documentação detalhada](../administration/custom-fields.md#add).


### Novos recursos em Disponibilidade limitada {#25-4-features-la}

>[!AVAILABILITY]
>
>Os seguintes recursos estão em Disponibilidade limitada (LA). Eles são restritos a clientes que migram **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente. Eles exigem uma atualização do servidor do Campaign para a v8.7.4.
>
>Consulte as seguintes páginas de documentação: [Transição do Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários do Campaign Standard](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/campaign-standard-migration-home).

* **Criação de entrega multilíngue**: agora você pode enviar várias entregas de email em diferentes idiomas na Interface do Adobe Campaign Web. O recurso de entrega multilíngue permite escolher o idioma padrão da entrega, bem como os diferentes idiomas nos quais a entrega pode ser enviada. Você também pode visualizar essas entregas nos idiomas escolhidos. Para obter mais informações, consulte a [documentação detalhada](../email/edit-content.md).

* **Relatórios dinâmicos para multilíngue**: os relatórios dinâmicos agora estão disponíveis para entregas de email multilíngues. Para obter mais informações, consulte a [documentação detalhada](../reporting/global-reports.md).

* **Suporte à API REST de SMS (Disponibilidade limitada)**: a API REST de Mensagens transacionais agora está disponível para o canal de SMS. Quando email e mobilePhone estão presentes no conteúdo, você pode usar o campo “wishedChannel” para especificar o canal. Se não for fornecido, o email será usado por padrão, a menos que wishedChannel solicite explicitamente SMS. Para obter mais informações, consulte a [documentação detalhada](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

## Versão de fevereiro de 2025 {#25-2-release}

**Data de lançamento**: 18 de fevereiro de 2025

Os seguintes recursos e melhorias estão disponíveis a partir da versão de fevereiro.

### Recursos {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Criar regras de negócios (regras de tipologia)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível criar tipologias e regras de tipologia na interface do Adobe Campaign Web. Elas permitem controlar, filtrar e priorizar o envio de entregas. Tipologias são usadas para validar que as entregas sempre contenham componentes obrigatórios (como um link de cancelamento de assinatura ou uma linha de assunto) ou regras de filtragem para excluir grupos do seu público-alvo (como pessoas que cancelaram a assinatura, concorrentes ou clientes sem fidelização).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Para obter mais informações, consulte a <a href="../administration/typologies.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Target mappings</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível criar target mappings na interface do Campaign Web. Os target mappings definem como diferentes canais de entrega (email, SMS, notificações por push) se vinculam aos campos de dados de um esquema. O target mapping permite definir o público-alvo: perfis, beneficiários de contrato, operadores, assinantes, clientes potenciais etc.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>Para obter mais informações, consulte a <a href="../administration/target-mappings.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Detalhes do esquema</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível acessar os detalhes de um esquema selecionando seu nome na lista. A edição de campos personalizados agora pode ser acessada pelo botão <b>Editar campos personalizados</b>, disponível nos detalhes do esquema.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>Para obter mais informações, consulte a <a href="../administration/schemas.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

## Versão de janeiro de 2025 {#25-1-release}

**Data de lançamento**: 5 de fevereiro de 2025

Os seguintes recursos e melhorias estão disponíveis a partir da versão de janeiro.

### Recursos {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Criar e usar fragmentos visuais</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Fragmentos visuais são blocos visuais predefinidos que podem ser reutilizados em várias entregas de email ou em modelos de conteúdo. Esse recurso agora está disponível para todos os clientes que estão na build 8.6.4 do servidor e posteriores.</p>
<img src="assets/do-not-localize/visual-fragment.gif">
<p>Para obter mais informações, consulte a <a href="../content/use-visual-fragments.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Usar um sistema de terceiros para entregas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora, é possível definir entregas externas e modelos de entrega externa na interface do Campaign Web. Nesse modo, as mensagens são compiladas em um arquivo de saída que pode ser compartilhado com o provedor externo. Por padrão, o modo de entrega externa é usado no canal de correspondência direta.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Para obter mais informações, consulte a <a href="../msg/send-external-deliveries.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gerenciar enumerações</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível criar enumerações diretamente por meio da interface do Adobe Campaign Web. Uma enumeração é uma lista de valores sugeridos pelo sistema para preencher campos. Enumerações permitem padronizar os valores desses campos, ajudam na entrada de dados ou podem ser usadas em consultas.</p>
<img src="assets/do-not-localize/enumerations.gif">
<p>Para obter mais informações, consulte a <a href="../administration/enumerations.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criar opções personalizadas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível acessar as opções técnicas na interface do Adobe Campaign Web e criar suas próprias opções personalizadas para atender às suas necessidades. Isso é particularmente útil ao trabalhar com atividades de fluxo de trabalho de código JavaScript para armazenar dados intermediários.</p>
<img src="assets/do-not-localize/options.gif">
<p>Para obter mais informações, consulte a <a href="../administration/options.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Definir e chamar códigos JavaScript</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível criar códigos JavaScript na interface do Adobe Campaign Web. Isso permite criar funções reutilizáveis que podem ser usadas em fluxos de trabalho, de modo semelhante a uma biblioteca.</p>
<img src="assets/do-not-localize/javascript.gif">
<p>Para obter mais informações, consulte a <a href="../administration/javascript-codes.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Geração de páginas de destino com o Assistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O Assistente de IA agora está disponível para entregas de página de destino, permitindo gerar texto, imagens ou layouts de página completos.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Para obter mais informações sobre o Assistente de IA, consulte a <a href="../email/generative-lp.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>


### Melhorias {#25-1-improvements}

* Personalize a exibição de campos personalizados na interface:

   * Agora é possível selecionar campos personalizados adicionais para exibição na interface
   * Agora é possível definir regras para exibir campos personalizados do tipo link, como restringir valores de lista com base na entrada de outro campo
   * Agora é possível organizar os campos na interface com mais flexibilidade: os campos podem se estender por uma única coluna ou ser agrupados em subseções para melhorar a organização
   * Agora você pode definir campos específicos como somente leitura

* Filtros Recentes e Favoritos: para reutilizar rapidamente atributos usados com frequência, agora é possível adicioná-los aos favoritos. Isso garante que eles estejam prontamente acessíveis para tarefas futuras. Além dos favoritos, é possível também visualizar e usar os atributos selecionados mais recentemente.

* Contas externas: o novo tipo **[!UICONTROL Roteamento]** está disponível para seleção ao criar uma nova conta externa. Ele permite configurar uma conta externa específica para usar nas entregas externas. [Saiba mais](../administration/external-account.md#routing)
