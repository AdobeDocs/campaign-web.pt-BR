---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 28%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

## Versão de março de 2026 {#26-3-release}

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
<p>O recurso de criação de esquema agora está disponível para todos os clientes (GA). Esse recurso permite criar e gerenciar esquemas diretamente na interface do usuário da Web do Campaign. Você pode criar novas tabelas, estender esquemas existentes e criar formulários personalizados. Você pode definir estruturas de dados personalizadas para atender às suas necessidades comerciais específicas sem precisar acessar o Console do cliente.</p>
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
<p>Os temas fornecem uma experiência de criação aprimorada para emails, permitindo definir estilos de tema reutilizáveis que se ajustem às diretrizes da sua marca. Agora é possível usar variáveis de tema em fragmentos, garantindo um estilo consistente em seus modelos de email. Esse recurso permite criar emails mais rapidamente com módulos predefinidos que abstraem elementos de conteúdo, como títulos, descrições, imagens e links, enquanto mantêm a consistência da marca.</p>
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
<p>Permita a integração perfeita de modelos Firefly padrão e personalizados, juntamente com modelos de imagem de terceiros aprovados, para oferecer maior flexibilidade, controle e alinhamento de marca ao gerar imagens.</p>
<p>Escolha o modelo certo para suas necessidades:</p>
<ul><li> <strong>Modelo do Adobe</strong> (desenvolvido pela Firefly Image Model 4) para geração imediata de imagens sem configuração adicional</li><li> <strong>Modelo de parceiro</strong> (viabilizado pelo Gemini 2.5 Flash) para recursos especializados</li><li><strong>Modelos personalizados</strong> (modelos específicos da marca treinados em seus próprios ativos) para geração de itens sob marca que se alinham precisamente à identidade, ao estilo e às diretrizes visuais da sua marca.</li></ul>
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
<p>A atividade de fluxo de trabalho <strong>Entrega automatizada</strong> agora está disponível na paleta de fluxo de trabalho. Você pode usá-lo para criar ou executar ações de delivery (preparar, enviar uma prova, preparar e iniciar etc.) diretamente no seu fluxo de trabalho. Selecione um delivery existente criado fora do workflow para reutilizá-lo em cada execução ou crie um novo delivery a partir de um template sempre que a atividade for executada.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Para obter mais informações, consulte a <a href="../workflows/activities/automated-delivery.md">documentação detalhada.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Várias ramificações de fluxo de trabalho e Atividade de junção</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p>Agora há suporte para <strong>Várias ramificações</strong>. Em vez de usar uma <strong>Bifurcação</strong>, você pode clicar em <strong>Adicionar ramificação</strong> na barra de ferramentas. A atividade <strong>AND-join</strong> também foi aprimorada. Agora é uma atividade genérica <strong>Join</strong> que permite escolher entre as opções de associação AND e OR.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Para obter mais informações, consulte as páginas de documentação de <a href="../workflows/orchestrate-activities.md#toolbar">Orquestrar atividades</a> e <a href="../workflows/activities/join.md">Ingressar</a>.</p>
</td>
</tr>
</tbody>
</table>

### Aprimoramentos {#26-3-improvements}

* A atividade de fluxo de trabalho **Start** foi adicionada para melhorar a compatibilidade com o Console do Cliente. Essa atividade é opcional e não é inserida por padrão em novos workflows. No entanto, ele é adicionado automaticamente aos workflows existentes.
  [Saiba mais](../workflows/activities/about-activities.md#flow-control)
* O campo de seleção de fuso horário nas configurações de **Agenda** de uma entrega foi movido para baixo do campo **Data de contato**. [Saiba mais](../msg/create-deliveries.md#gs-schedule)