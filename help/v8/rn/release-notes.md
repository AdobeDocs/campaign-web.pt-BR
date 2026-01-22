---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ca1a437f8a8a25c0a15b9148e9c73271795f16c7
workflow-type: ht
source-wordcount: '506'
ht-degree: 100%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e melhorias disponíveis em versões anteriores estão listadas nas páginas de [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Versão de outubro de 2025 {#25-10-updates}

_3 de novembro de 2025_

<table>
<thead>
<tr>
<th><strong>Recursos multilíngues para mensagens transacionais, notificações por push e SMS (DL)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora você pode enviar várias mensagens transacionais, notificações por push e mensagens SMS em diferentes idiomas na Interface do Adobe Campaign Web. O recurso de entrega multilíngue permite escolher o idioma padrão da entrega, bem como os diferentes idiomas nos quais a entrega pode ser enviada. Você também pode visualizar essas entregas nos idiomas escolhidos. </p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura.</p>
<p>Para obter mais informações, consulte a <a href="../msg/multilingual.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>Enriquecimento de perfil em mensagens transacionais (DL)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Esse recurso permite personalizar mensagens transacionais vinculando campos do banco de dados do Adobe Campaign ao conteúdo da mensagem. Você pode selecionar target mappings, colunas de enriquecimento e uma chave de reconciliação para garantir uma personalização em tempo real e precisa, mantendo os limites de desempenho.</p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura. No momento, este recurso só está disponível para emails.</p>
<p>Para obter mais informações, consulte a <a href="../transactional-messaging/profile-enrichment.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integração com o Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Para aprimorar a eficiência do marketing e manter a consistência da marca, agora é possível integrar facilmente as experiências do GenStudio for Performance Marketing com o Campaign. Isso permite aproveitar a criação de conteúdo viabilizada por IA do GenStudio com os recursos de orquestração avançada do Campaign.<p>
<p>Para obter mais informações, consulte a <a href="../integrations/genstudio.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Suporte ao modo escuro no Designer de email</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O Designer de email agora oferece a capacidade de alternar para a exibição no modo escuro, onde é possível definir configurações personalizadas específicas. Observe que a renderização final depende do cliente de email do destinatário e que nem todos os clientes de email são compatíveis com o modo escuro.</p>
<p>Para obter mais informações, consulte a <a href="../email/dark-mode.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Aprimoramentos {#25-10-improvements}

* Nas entregas criadas no Console do cliente, a seção **Público-alvo** agora indica se uma condição dinâmica foi definida para destinos de prova. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* Agora é possível alternar entre o construtor de regras novo e o legado ao configurar uma condição com o recurso de conteúdo condicional do Designer de email. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* Agora é possível selecionar links de coleção, como compras, na definição da tela do esquema do destinatário. Isso exibe os dados relacionados nas telas de perfil por meio de uma guia dedicada. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Como admin do Campaign, agora é possível configurar conexões com o Salesforce CRM e o Microsoft Dynamics.
  [Saiba mais](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

