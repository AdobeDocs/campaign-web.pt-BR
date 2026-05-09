---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 65031741dc7c667ef74469d75b8ea60a5fc20aaf
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 91%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de abril de 2026 {#26-4-release}

_29 de abril de 2026_

### Melhoria {#26-4-improvement}

A seção **Enrichment data** agora está disponível na atividade de fluxo de trabalho **Build audience** (tipo de consulta). Você pode exibir, adicionar, editar e remover **dados adicionais** diretamente da interface do usuário da Web do Campaign. Como na atividade **Enrichment**, você pode adicionar atributos de enriquecimento único, links de coleção e expressões.

[Saiba mais](../workflows/activities/build-audience.md)

## Versão de março de 2026 {#26-3-release}

_24 de março_ de 2026_

### Novos recursos {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Criação de esquema (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O recurso de criação de esquema agora está disponível para todos os clientes (GA). Esse recurso permite criar e gerenciar esquemas diretamente na interface do Campaign Web. Você pode criar novas tabelas, estender esquemas existentes e criar formulários personalizados. Você pode definir estruturas de dados personalizadas para atender às suas necessidades comerciais específicas sem precisar acessar o Console do cliente.</p>
<p>Para obter mais informações, consulte a <a href="../administration/schemas.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Temas no Designer de email (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Os temas proporcionam uma experiência de criação de emails aprimorada, permitindo que você defina estilos de tema reutilizáveis que se adéquem às diretrizes da sua marca. Agora você pode usar variáveis de tema nos fragmentos, garantindo um estilo consistente em todos os seus modelos de email. Esse recurso permite que você crie emails mais rapidamente com módulos predefinidos que agrupam elementos de conteúdo, como títulos, descrições, imagens e links, mantendo a consistência da marca.</p>
<p>Observação: esse recurso só está disponível para um conjunto de organizações (disponibilidade limitada) e será implantado globalmente em uma versão futura.</p>
<p>Para obter mais informações, consulte a <a href="../email/apply-email-themes.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integração de modelos personalizados do Firefly e modelos de geração de imagens de terceiros</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Permita a integração perfeita de modelos padrão e personalizados do Firefly, bem como de modelos de imagem de terceiros aprovados, para oferecer maior flexibilidade, controle e alinhamento com a marca na geração de imagens.</p>
<p>Escolha o modelo certo para suas necessidades:</p>
<ul><li> <strong>Modelo da Adobe</strong> (desenvolvido pelo Firefly Image Model 4) para geração imediata de imagens sem configuração adicional</li><li> <strong>Modelo de parceiro</strong> (desenvolvido por Gemini 2.5 Flash) para recursos especializados</li><li><strong>Modelos personalizados</strong> (modelos específicos para cada marca, treinados com seus próprios recursos) para uma geração de conteúdo que se alinhe perfeitamente à identidade, ao estilo e às diretrizes visuais da sua marca.</li></ul>
<p>Para obter mais informações, consulte a <a href="../content/generative-models.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Atividade de entrega automatizada</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>A atividade de fluxo de trabalho <strong>Entrega automatizada</strong> já está disponível na paleta de fluxos de trabalho. Você pode usá-la para criar ou executar ações de entrega (preparar, enviar uma prova, preparar e iniciar etc.) diretamente do seu fluxo de trabalho. Selecione uma entrega existente criada fora do fluxo de trabalho para reutilizá-la em todas as execuções, ou crie uma nova entrega a partir de um modelo sempre que a atividade for executada.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Para obter mais informações, consulte a <a href="../workflows/activities/automated-delivery.md">documentação detalhada.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Várias ramificações de fluxo de trabalho e atividade Associação</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>Agora há suporte para <strong>várias ramificações</strong>. Em vez de usar uma <strong>Bifurcação</strong>, você pode clicar em <strong>Adicionar ramificação</strong> na barra de ferramentas. A atividade <strong>AND-join</strong> também foi aprimorada. Agora ela é uma atividade de <strong>Associação</strong> genérica que permite escolher entre as opções de associação AND e OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Para obter mais informações, consulte as páginas da documentação <a href="../workflows/orchestrate-activities.md#toolbar">Orquestrar atividades</a> e <a href="../workflows/activities/join.md">Associação</a>.</p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-3-improvements}

* A atividade de fluxo de trabalho **Iniciar** foi adicionada para melhorar a compatibilidade com o Console do cliente. Esta atividade é opcional e não é incluída por padrão nos novos fluxos de trabalho. No entanto, ela é adicionada automaticamente aos fluxos de trabalho existentes.
  [Saiba mais](../workflows/activities/about-activities.md#flow-control)
* O campo de seleção de fuso horário nas configurações de **Programação** de uma entrega foi movido para baixo do campo **Data de contato**. [Saiba mais](../msg/create-deliveries.md#gs-schedule)