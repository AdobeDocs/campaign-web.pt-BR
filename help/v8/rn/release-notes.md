---
title: Notas de versão da interface do Campaign Web v8
description: Conheça os novos recursos que acompanham a versão mais recente da interface do Campaign Web
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Notas de versão {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Notas de versão"
>abstract="As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, as notas de versão do Campaign são atualizadas várias vezes por mês, com os recursos, melhorias e correções mais recentes. Recomendamos que você as verifique regularmente."

As versões da interface do usuário do Adobe Campaign Web operam em um modelo de entrega contínua que permite uma abordagem à implantação de recursos mais dimensionável e em fases. Devido a isso, essas notas de versão são atualizadas várias vezes por mês. Verifique-as regularmente.

As alterações e aprimoramentos disponíveis nas versões anteriores estão listadas em [2024](release-notes-24.md) e [2025](release-notes-25.md).

## Versão de abril de 2025 {#25-4-release}

**Data de lançamento**: quarta-feira, 29 de abril de 2025


### Novos recursos {#25-4-features}

Os seguintes recursos estão disponíveis para todos os usuários a partir da versão de abril.

<table>
<thead>
<tr>
<th><strong>Canal da central de atendimento</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>O canal da central de atendimento agora está disponível na interface do usuário da Web do Campaign. Este canal se refere a um método de comunicação usado para gerenciar e rastrear comunicações ou interações realizadas por meio de uma central de atendimento — normalmente, chamadas telefônicas feitas por agentes para clientes ou clientes potenciais.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Para obter mais informações, consulte a <a href="../call-center/gs-call-center.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Novo construtor de regras</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Um novo construtor de regras agora está disponível para ajudar você a definir condições complexas em uma interface do usuário aprimorada. Você pode alternar do construtor de regras antigo para o novo, conforme necessário.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Para obter mais informações, consulte a <a href="../query/query-modeler-overview.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Criação de conta externa</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Como administrador do Campaign, agora você pode configurar novas conexões com sistemas externos por meio da interface da Web do Campaign.
Você também pode exibir, atualizar e gerenciar contas externas existentes.</p>
<p>Para obter mais informações, consulte a <a href="../administration/external-account.md">documentação detalhada</a>.</p>
</td>
</tr>
</tbody>
</table>

### Melhorias {#25-4-improvements}

**Melhorias gerais na interface**

* A descrição do Campo, as opções Adicionar aos favoritos e Distribuição de valores para atributos de esquema agora estão mais visíveis na interface do usuário. Para obter mais informações, consulte a [documentação detalhada](../get-started/attributes.md).
* Na interface, a data e a hora agora são exibidas de acordo com o idioma principal definido nas preferências do Experience League. Esse aprimoramento só está disponível para vários idiomas. Para ver a lista completa de idiomas suportados, consulte a [documentação detalhada](https://experienceleague.adobe.com/pt-br/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**Editor de email**: para aprimorar a acessibilidade na interface do usuário da Web do Campaign, dois novos campos agora estão disponíveis no Designer de email: eles correspondem ao elemento `title` e ao atributo lang no elemento `html` do seu conteúdo de email. É possível definir essas configurações além do campo Preheader, na seção email Body. Para obter mais informações, consulte a [documentação detalhada](../email/metadata.md).

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Esquemas**

* Agora é possível editar o schema temporário de uma lista na interface do usuário da Web do Campaign. Para obter mais informações, consulte a [documentação detalhada](../audience/manage-audience.md).
* Agora você pode visualizar os campos personalizados de um esquema em uma tela de amostra. Para obter mais informações, consulte a [documentação detalhada](../administration/custom-fields.md#add).
* Agora é possível mover campos personalizados na lista usando a função arrastar e soltar. Para obter mais informações, consulte a [documentação detalhada](../administration/custom-fields.md#add).


### Novos recursos em Disponibilidade limitada {#25-4-features-la}

>[!AVAILABILITY]
>
>Os seguintes recursos estão em Disponibilidade limitada (LA). Eles são restritos aos clientes que estão migrando o **do Adobe Campaign Standard para o Adobe Campaign v8** e não podem ser implantados em nenhum outro ambiente. Eles exigem uma atualização do servidor do Campaign para a v8.7.4.
>
>Consulte as seguintes páginas de documentação: [Transição do Campaign Standard para o Campaign v8](../rn/acs-migration.md) e [Recursos para usuários do Campaign Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=pt-BR).

* **Criação de entrega multilíngue** - Agora você pode enviar várias entregas de email em diferentes idiomas na Interface do Usuário da Web do Adobe Campaign. O recurso de delivery multilíngue permite escolher o idioma padrão do delivery, bem como os diferentes idiomas nos quais o delivery pode ser enviado. Você também pode visualizar esses deliveries nos idiomas escolhidos. Para obter mais informações, consulte a [documentação detalhada](../email/edit-content.md).

* **Relatórios Dinâmicos para Multilíngue** - Os relatórios dinâmicos agora estão disponíveis para entregas de email multilíngues. Para obter mais informações, consulte a [documentação detalhada](../reporting/global-reports.md).

* **Suporte à API REST (LA) de SMS** - A API REST de Mensagens Transacionais agora está disponível para o canal SMS. Quando email e mobilePhone estão presentes na carga, você pode usar o campo &quot;wishedChannel&quot; para especificar o canal. Se não for fornecido, o e-mail será usado por padrão, a menos que wishedChannel solicite explicitamente SMS. Para obter mais informações, consulte a [documentação detalhada](https://experienceleague.adobe.com/pt-br/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank}.

