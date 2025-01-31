---
title: Notas de versão antecipadas da interface do Campaign Web v8
description: Conheça os novos recursos incluídos na próxima versão da interface do Campaign Web
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 202796bbaa26afb0741a5eb3947795ceff7e5414
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 18%

---

# Notas de versão antecipadas {#e-release}

A interface do Adobe Campaign Web está sempre fornecendo novos recursos, melhorias de recursos existentes e correções de erros. As alterações são consolidadas no final de cada mês e incluídas nas [notas de versão](release-notes.md).

**As notas de versão antecipadas abaixo estão sujeitas a alterações sem aviso prévio até a data de disponibilidade do lançamento**. Links, telas e a documentação atualizada são publicados nas [notas de versão](release-notes.md) na data do lançamento.

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
<p>Fragmentos visuais são blocos visuais predefinidos que podem ser reutilizados em vários deliveries de email ou em modelos de conteúdo. Esse recurso agora está disponível para todos os clientes que estão executando no server build 8.6.4 e superior.</p>
<p>Para obter mais informações, consulte a <a href="../content/use-visual-fragments.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Usar um sistema de terceiros para enviar deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora você pode definir deliveries externos e templates de delivery externos na interface da Web do Campaign. Nesse modo, as mensagens são compiladas em um arquivo de entrada, que pode ser compartilhado com seu provedor externo. Por padrão, o modo de delivery externo é usado para o canal de mala direta.</p>
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
<p>Agora você pode criar tipologias e regras de tipologia na interface da Web do Adobe Campaign. Uma tipologia é uma coleção de regras de tipologia que ajudam a controlar, filtrar e priorizar os deliveries. As tipologias garantem que seus deliveries sempre contenham os elementos necessários (como um link de cancelamento de inscrição ou linha de assunto) e apliquem regras de filtragem para excluir grupos específicos do público-alvo (como clientes que não assinam, concorrentes ou clientes não fidelizados).</p>
<img src="assets/do-not-localize/typology.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gerenciar suas listas discriminadas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível criar enumerações diretamente por meio da interface da Web do Adobe Campaign. Uma enumeração é uma lista de valores sugeridos pelo sistema para preencher campos. Use enumerações para padronizar os valores desses campos, ajuda com a entrada de dados ou uso em queries.</p>
<img src="assets/do-not-localize/enumerations.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Agora você pode acessar opções técnicas na Interface do usuário da Web da Adobe Campaign e criar suas próprias opções personalizadas para atender às suas necessidades. Isso é particularmente útil ao trabalhar com atividades de workflow de código JavaScript para armazenar dados intermediários.</p>
<img src="assets/do-not-localize/options.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
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
<p>Agora é possível criar códigos JavaScript na Interface do usuário da Web do Adobe Campaign. Isso permite criar funções reutilizáveis que podem ser usadas em fluxos de trabalho, de modo semelhante a uma biblioteca.</p>
<img src="assets/do-not-localize/javascript.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

### Melhorias {#25-1-improvements}

* Personalizar a exibição de campos personalizados na interface:

   * Agora é possível selecionar campos personalizados adicionais para exibir na interface
   * Agora é possível definir regras para exibir campos personalizados do tipo link, como restringir valores da lista com base na entrada de outro campo
   * Agora é possível organizar os campos na interface com mais flexibilidade: os campos podem se estender por uma única coluna ou ser agrupados em subseções para melhorar a organização
   * Agora você pode definir campos específicos como somente leitura

* Filtros Recentes e Favoritos: para reutilizar rapidamente atributos usados com frequência, agora é possível adicioná-los aos favoritos. Isso garante que eles estejam prontamente acessíveis para tarefas futuras. Além dos favoritos, você também pode visualizar e usar os atributos selecionados mais recentemente.


