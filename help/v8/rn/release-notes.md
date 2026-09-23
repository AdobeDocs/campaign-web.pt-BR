---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
    internal-label: Dynamic reporting
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
    internal-label: Integrations
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
source-git-commit: 73553f19c6e88256f0e9f38479bdfc292a3221f8
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 38%
---
# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de setembro de 2026 {#26-9-release}

_22 de setembro de 2026_

### Novos recursos {#26-9-features}

<table>
<thead>
<tr>
<th><strong>Canal LINE</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O Adobe Campaign agora oferece suporte ao canal <strong>LINE</strong>, um aplicativo popular de mensagens instantâneas. Crie e envie mensagens LINE usando conteúdo de texto, imagem ou vídeo, em deliveries independentes ou em workflows, junto com seus outros canais. <a href="../line/get-started-line.md">Leia mais</a></p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-9-improvements}

* **Acesso à navegação lateral**: os administradores agora podem ocultar entradas específicas de menu da navegação lateral. [Leia mais](../administration/schemas-browse-access.md#screen-def)
* **Tipos de aprovação adicionais**: agora você pode exigir aprovações de orçamento e de início de entrega para entregas do Campaign, além de aprovações de conteúdo e destino. [Leia mais](../campaigns/campaign-approvals.md#configure-approvals)
* **Direcionamento de SMS com base em visitante**: o mapeamento de destino de visitante agora está disponível para entregas de SMS. [Leia mais](../sms/create-sms.md)
* **Botão de cancelamento do fluxo de trabalho**: um novo botão **Cancelar** permite reverter alterações não salvas em um fluxo de trabalho. [Leia mais](../workflows/orchestrate-activities.md#save-cancel)
* **Desduplicação com vários valores**: a opção **Seguindo uma lista de valores** agora dá suporte a vários atributos. [Leia mais](../workflows/activities/deduplication.md#deduplication-configuration)
* **Mapeamento de destino móvel**: agora é possível criar mapeamentos de destino para destinos de aplicativos móveis. [Leia mais](../administration/target-mappings.md#create-mapping)
* **Enriquecimento do banco de dados externo**: agora você pode enriquecer dados de um banco de dados externo na atividade **Enriquecimento** ou **Compilar público**. [Leia mais](../workflows/activities/enrichment.md#external-data)
* **Reconciliação de público-alvo do arquivo**: agora você pode configurar se deseja importar destinatários para o banco de dados ao direcionar um público-alvo de um arquivo. [Leia mais](../audience/file-audience.md#upload)
* **Junções diretas em coleções**: ao selecionar um atributo diretamente de uma coleção, agora é possível escolher como a condição será criada: usando a opção padrão recomendada, uma função de agregação ou uma junção direta avançada. [Leia mais](../query/build-query.md#links)

