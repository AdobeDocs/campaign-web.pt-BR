---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
TQID: https://experienceleague.adobe.com/HkI2JUqLNM805hPfVsXl-8nwR70TzxRP31V9EI4yKGA
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
  - id: c309ee4e-82e4-4f7e-b608-ef345678c34e
  - id: d5ef99fa-df0c-4153-bf94-105ad0724167
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: d9d1733854bceac52d54e02125dac92b74872c77
workflow-type: tm+mt
source-wordcount: 716
ht-degree: 23%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de julho de 26 {#26-7-release}

_28 de julho de 2026_

### Novos recursos {#26-7-features}

<table>
<thead>
<tr>
<th><strong>Gerenciamento de ofertas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora é possível gerenciar ofertas de ponta a ponta diretamente na interface do usuário da Web do Campaign. Configure ambientes de oferta e espaços de oferta, crie seu catálogo de ofertas e categorias, crie ofertas com regras de elegibilidade e pesos de prioridade, e aprove-os e implante-os para uso em seus deliveries. As configurações avançadas permanecem disponíveis no Console do cliente.</p>
<p>Para obter mais informações, consulte a <a href="../offers/gs-offer-management.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Configuração da marca</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Agora, os administradores técnicos podem criar e configurar marcas diretamente na interface do usuário da Web do Campaign, sem usar o console do cliente. Todas as configurações da marca, incluindo identidade, subdomínio e protocolos, parâmetros de cabeçalho de email e parâmetros de rastreamento de URL, agora estão disponíveis na interface do usuário da Web.</p>
<p>Para obter mais informações, consulte a <a href="../administration/branding/branding-configure.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Recursos públicos no Designer de email</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Ao adicionar imagens a seus emails, agora você pode selecionar <strong>recursos públicos</strong>. Isso permite escolher uma imagem já disponível em sua instância do Adobe Campaign, como um arquivo importado anteriormente no Designer de email ou um recurso público carregado do console do cliente.</p>
<p>Para obter mais informações, consulte a <a href="../email/content-components.md#image">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Atividade de workflow do carregamento de dados (RDBMS)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A atividade <strong>Data loading (RDBMS)</strong> agora está disponível na interface do usuário da Web do Campaign. Use esta atividade para carregar dados diretamente de um banco de dados relacional externo em seu fluxo de trabalho. Os dados extraídos estão disponíveis em todo o fluxo de trabalho e podem ser usados para direcionamento, enriquecimento ou processamento adicional de dados.</p>
<p>Para obter mais informações, consulte a <a href="../workflows/activities/data-loading-rdbms.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Páginas JavaScript dinâmicas</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>As páginas dinâmicas do JavaScript (JSSP) permitem construir páginas do lado do servidor que geram conteúdo dinâmico quando acessados por meio de um URL, como APIs personalizadas, exportações ou lógica de aplicativo da Web. Agora você pode criar, modificar, duplicar e excluir essas páginas diretamente da interface do usuário da Web do Campaign.</p>
<p>Para obter mais informações, consulte a <a href="../administration/dynamic-javascript-pages.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-7-improvements}

* As seguintes melhorias foram realizadas na **configuração de esquema personalizada**:
  * A nova seção **Dados de ação** permite restringir as ações disponíveis nos registros de um esquema personalizado, independentemente das regras de segurança configuradas em pastas individuais. [Leia mais](../administration/schemas-action-data.md)
  * **Filtros personalizados** foram adicionados à seção **Configuração da lista de inventário**. Eles permitem escolher quais atributos são exibidos como campos de acesso rápido no painel Filtros da exibição de lista. [Leia mais](../administration/schemas-custom-filters.md)

* As seguintes melhorias foram realizadas nos **fluxos de trabalho**:
  * A exclusão de uma atividade de workflow agora é mais flexível: quando a atividade tem atividades subsequentes, você pode optar por excluir todas elas, excluir apenas a atividade selecionada ou excluí-la enquanto mantém suas atividades subsequentes em uma nova ramificação. [Leia mais](../workflows/orchestrate-activities.md#delete-activity)
  * Agora é possível desconectar uma transição entre duas atividades de workflow sem excluir nenhuma delas. Isso permite reorganizar um diagrama de workflow, por exemplo, para separar temporariamente um grupo de atividades que você deseja manter, sem precisar excluí-las e recriá-las. [Leia mais](../workflows/orchestrate-activities.md#disconnect-transition)
  * Agora, barras de rolagem horizontais e verticais são exibidas ao redor da tela do fluxo de trabalho, permitindo navegar em fluxos de trabalho grandes arrastando-os diretamente para a área que deseja visualizar. [Leia mais](../workflows/orchestrate-activities.md)
  * Ao salvar ou iniciar/reiniciar um fluxo de trabalho, um aviso será exibido se outro usuário tiver modificado o fluxo de trabalho na interface do usuário da Web ou no console do cliente desde que você o abriu. Você pode optar por substituir as outras alterações pela sua, recarregar o fluxo de trabalho para obter a versão mais recente ou cancelar.

* **Endereço de email do remetente**: agora é possível restringir o campo **De email** de suas entregas a uma lista predefinida de endereços, usando a opção **NmsDelivery_senderAddressMask**. [Leia mais](../administration/options.md#restrict-sender-address)
* **Mensagens de erro de logon** foram aprimoradas: quando uma tentativa de logon falha, a interface do usuário da Web agora exibe uma mensagem de erro mais específica para vários cenários (por exemplo, quando o usuário não tem uma zona de segurança atribuída ou seu endereço IP é restrito).
