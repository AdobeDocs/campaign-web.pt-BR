---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '836'
ht-degree: 53%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário da Web do Adobe Campaign operam em um modelo de entrega contínua, que permite uma abordagem escalável e em fases para a implantação de recursos. Dessa forma, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e aprimoramentos disponíveis nas versões anteriores estão listadas [nesta página](release-notes-24.md).

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
<p>Agora é possível criar tipologias e regras de tipologia na interface do Adobe Campaign Web. As tipologias controlam, filtram e priorizam o envio de deliveries. As tipologias validam que os deliveries sempre contêm componentes obrigatórios (como um link de cancelamento de subscrição ou uma linha de assunto) ou regras de filtragem para excluir grupos do seu público-alvo (como clientes que não assinam, concorrentes ou clientes que não são do programa de fidelidade).</p>
<img src="assets/do-not-localize/typology.gif" alt="Ilustração da criação de regras de tipologia na interface do usuário da Web do Adobe Campaign">
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
<p>Agora é possível criar target mappings na interface do Campaign Web. Os target mappings definem como diferentes canais de entrega (email, SMS, notificações por push) se vinculam aos campos de dados de um esquema. O target mapping define o público-alvo direcionado: perfis, beneficiários de contrato, operadores, assinantes, prospetos e outros.</p>
<img src="assets/do-not-localize/target-mapping.gif" alt="Ilustração da criação de target mappings na interface do usuário da Web do Adobe Campaign">
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
<img src="assets/do-not-localize/schemas.gif" alt="Ilustração de detalhes do esquema e edição de campos personalizados na interface do usuário da Web do Adobe Campaign">
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
<p>Fragmentos visuais são blocos visuais predefinidos que podem ser reutilizados em vários deliveries de email ou em modelos de conteúdo. Esse recurso agora está disponível para todos os clientes que estão na build 8.6.4 do servidor e posteriores.</p>
<img src="assets/do-not-localize/visual-fragment.gif" alt="Ilustração da criação e do uso de fragmentos visuais na interface do usuário da Web do Adobe Campaign">
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
<img src="assets/do-not-localize/external-delivery.gif" alt="Ilustração da configuração de entrega externa na interface do usuário da Web do Adobe Campaign">
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
<p>Agora é possível criar enumerações diretamente por meio da interface do Adobe Campaign Web. Uma enumeração é uma lista de valores sugeridos pelo sistema para preencher campos. Use enumerações para padronizar os valores desses campos, auxiliar na entrada de dados ou usar em consultas.</p>
<img src="assets/do-not-localize/enumerations.gif" alt="Ilustração do gerenciamento de enumeração na interface do usuário da Web do Adobe Campaign">
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
<img src="assets/do-not-localize/options.gif" alt="Ilustração da criação de opções personalizadas na interface do usuário da Web do Adobe Campaign">
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
<img src="assets/do-not-localize/javascript.gif" alt="Ilustração da criação de código JavaScript na interface do usuário da Adobe Campaign Web">
<p>Para obter mais informações, consulte a <a href="../administration/javascript-codes.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Geração de página de aterrissagem com o Assistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O Assistente de IA agora está disponível com seus deliveries de página de aterrissagem, permitindo gerar texto, imagens ou layouts de página completos.</p>
<img src="assets/do-not-localize/ai-lp.gif" alt="Ilustração do uso do Assistente de IA para geração de páginas de aterrissagem na interface do usuário da Web do Adobe Campaign">
<p>Para obter mais informações sobre o Assistente de IA, consulte a <a href="../email/generative-lp.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Melhorias {#25-1-improvements}

* Personalize a exibição de campos personalizados na interface:
   * Selecione campos personalizados adicionais para exibir na interface.
   * Defina regras para exibir campos personalizados do tipo link, como restringir valores de lista com base em outra entrada de campo.
   * Organize os campos na interface de forma mais flexível: os campos podem se expandir por uma única coluna ou ser agrupados em subseções para uma melhor organização.
   * Definir campos específicos como somente leitura.

* Filtros Recentes e Favoritos: adicione os atributos usados com frequência aos favoritos para acesso rápido. Além dos favoritos, exiba e use os atributos selecionados mais recentemente.

* Contas externas: o novo tipo **[!UICONTROL Roteamento]** está disponível para seleção ao criar uma nova conta externa. Ele permite configurar uma conta externa específica para usar nas entregas externas. [Saiba mais](../administration/external-account.md#routing).