---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2: id: a075b2c1-7748-4328-b7f6-343aa314616aid: c309ee4e-82e4-4f7e-b608-ef345678c34eid: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 404a5a4f1d793404a326feb07cd6869aa97af664
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 78%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de agosto de 2026 {#26-8-release}

_18 de agosto de 2026_

### Novos recursos {#26-8-features}

<table>
<thead>
<tr>
<th><strong>Atividade de fluxo de trabalho de aprovação</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A atividade de fluxo de trabalho <strong>Aprovação</strong>, anteriormente disponível apenas no Console do cliente, agora está disponível na interface do usuário do Campaign Web. Atribua a tarefa a um grupo ou operador individual, personalize o título da notificação e a mensagem e defina as respostas possíveis (por exemplo, Sim/Não) como ramificações de saída.</p>
<p>Para obter mais informações, consulte a <a href="../workflows/activities/approval.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-8-improvements}

* **Abre o rastreamento**: agora você pode habilitar ou desabilitar a abertura de rastreamento diretamente na interface do usuário do Campaign Web. Isso ajuda você a cumprir os regulamentos de proteção dos dados. [Leia mais](../advanced-settings/delivery-settings.md#tracking-tab)
* **Exibição da lista de programas**: os programas agora estão listados em uma exibição dedicada, semelhante a campanhas, entregas e fluxos de trabalho. Você pode procurar programas existentes e criar novos diretamente nessa exibição. [Leia mais](../administration/plans-programs.md#create-program)
* **Configuração de esquema personalizado**: na seção **Dados da ação**, agora é possível desativar a ação **Duplicar** nos registros de um esquema personalizado. [Leia mais](../administration/schemas-action-data.md#action-data)
* **Filtros personalizados**: no editor de esquemas, agora é possível restringir os valores disponíveis no seletor para um filtro personalizado do tipo link, usando a nova caixa de diálogo **Configurações de link**. [Leia mais](../administration/schemas-custom-filters.md#settings)
* **Validação de esquema**: agora é possível validar a estrutura de um esquema diretamente do editor de esquema, usando o novo botão **Verificar**. [Leia mais](../administration/schemas-create-publish.md#create-new)
* **Segurança da pasta**: as ações disponíveis em uma pasta agora são consistentemente controladas pelos direitos do operador, correspondendo ao comportamento do Console do Cliente. [Saiba mais](../get-started/work-with-folders.md#about-folders).
  <!--* **Enrichment activity**: You can now enrich data from an external database directly from the **Enrichment** workflow activity. This matches the capability already available in the Client Console.-->
  <!--* **Workflow and delivery templates (only msf???)**: When creating a new workflow or delivery, you must now explicitly select a template. A default template is no longer applied automatically.-->

