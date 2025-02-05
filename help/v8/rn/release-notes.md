---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 898a9d62a18de0ee27713b5f15b032103463fcef
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 85%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e as melhorias disponíveis nas versões anteriores estão listadas [nesta página](release-notes-24.md).

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
<p>Agora, é possível definir entregas externas e modelos de entrega externa na interface do Campaign Web. Nesse modo, as mensagens são compiladas em um arquivo de saída, que pode ser compartilhado com o provedor externo. Por padrão, o modo de entrega externa é usado no canal de correspondência direta.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Para obter mais informações, consulte a <a href="../msg/send-external-deliveries.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criar regras de negócios (regras de tipologia)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível criar tipologias e regras de tipologia na interface do Adobe Campaign Web. Uma tipologia é uma coleção de regras de tipologia que ajudam a controlar, filtrar e priorizar entregas. As tipologias garantem que as entregas sempre contenham os elementos necessários (como um link de cancelamento de inscrição ou uma linha de assunto) e aplicam regras de filtragem para excluir grupos específicos do público-alvo (como clientes que cancelaram sua assinatura, concorrentes ou clientes não fidelizados).</p>
<img src="assets/do-not-localize/typology.gif">
<p>Para obter mais informações, consulte a <a href="../administration/typologies.md">documentação detalhada</a>.</p>
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
<th><strong>Geração de página de aterrissagem com o Acelerador de conteúdo do assistente de IA</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O Acelerador de conteúdo do Assistente de IA agora está disponível com os deliveries da página de aterrissagem, permitindo gerar texto, imagens ou layouts de página completos.</p>
<p>Para obter mais informações sobre o Acelerador de Conteúdo do Assistente de IA, consulte a <a href="../email/generative-gs.md">documentação detalhada</a>.</p>
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

* Contas externas: o novo tipo **[!UICONTROL Roteamento]** está disponível para seleção ao criar uma nova conta externa. Ele permite configurar uma conta externa específica para usar em seus deliveries externos. [Saiba mais](../administration/external-account.md#routing)