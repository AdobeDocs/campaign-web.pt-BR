---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: ht
source-wordcount: '418'
ht-degree: 100%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e as melhorias disponíveis nas versões anteriores estão listadas [nesta página](release-notes-24.md).

## Versão de outubro de 2024 {#24-10-release}

**Data de lançamento**: 29 de outubro de 2024

Os seguintes recursos e melhorias estão disponíveis a partir da versão de outubro.

### Recursos

<table>
<thead>
<tr>
<th><strong>Contas externas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível configurar e gerenciar contas externas diretamente na interface do Adobe Campaign Web. Esse novo recurso facilita a configuração de diferentes tipos de contas externas, como emails de rejeição (POP3) ou instâncias de execução.</p>
<p>Para obter mais informações, consulte a <a href="../administration/external-account.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Mensagens transacionais</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>As mensagens transacionais (Centro de mensagens) agora estão disponíveis na interface do Campaign Web. Este complemento foi desenvolvido para Acionar mensagens geradas de eventos disparados por sistemas de informação, podendo ser: fatura, confirmação de pedido, confirmação de envio, alteração de senha, notificação de indisponibilidade de produto, extrato de conta, criação de conta em site etc.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/transactional.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Melhorias

* **Atividades do fluxo de trabalho**: agora é possível mover uma atividade e todos os seus nós secundários de uma transição para outra dentro de um fluxo de trabalho. Um botão **Mover** dedicado está disponível no painel de propriedades da atividade para realizar isso. [Saiba mais](../workflows/orchestrate-activities.md#move)

* **Atividade de enriquecimento de fluxo de trabalho**

   * Agora é possível definir um alias e um rótulo ao criar um novo campo na atividade **Enriquecimento**. [Saiba mais](../workflows/activities/enrichment.md#collection-settings)
   * Agora você pode adicionar ofertas para cada perfil na atividade **Enriquecimento**. [Saiba mais](../workflows/activities/enrichment.md##add-offers)

* **Distribuição de valores**: ao acessar a lista de campos para personalização, agora é possível verificar como os valores estão distribuídos para cada campo. Uma janela pop-up exclusiva mostra o número e a porcentagem para cada valor. [Saiba mais](../query/build-query.md#distribution-values-query)

* **Informações de versão e sistema**: agora você pode acessar detalhes das versões da sua instância, tanto para o console do cliente quanto para a Interface da Web. Esta nova seção também lista todos os pacotes integrados instalados no seu ambiente. [Saiba mais](../get-started/user-interface.md#user-interface-about)

* **Listas**: agora é possível reordenar facilmente os valores de uma lista. [Saiba mais](../get-started/work-with-folders.md)

* **Entrega**: a variável Entrega agora pode ser acessada em campos de personalização. [Saiba mais](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)