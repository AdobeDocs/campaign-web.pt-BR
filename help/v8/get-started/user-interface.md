---
audience: end-user
title: Conheça a interface
description: Interface do Adobe Campaign Web
hidefromtoc: true
hide: true
robots: noindex
googlebot: noindex
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 4e5840f8566fb511ef2d862833a09b581f0250c2
workflow-type: tm+mt
source-wordcount: '1525'
ht-degree: 99%

---

# Conheça a interface {#user-interface}

A nova interface do Adobe Campaign Web oferece uma experiência de usuário moderna e intuitiva para simplificar o design e a entrega de campanhas de marketing. Esta interface se integra aos aplicativos e soluções da Adobe Experience Cloud.

Saiba como se conectar ao Adobe Campaign e conheça os princípios básicos de navegação da Experience Cloud [neste artigo](connect-to-campaign.md).

>[!NOTE]
>
>Esta documentação é atualizada com frequência para refletir as últimas alterações na interface do produto. No entanto, algumas capturas de tela podem ser um pouco diferentes da sua interface.

## Página inicial do Campaign {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recentes"
>abstract="A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação."

A página inicial do Campaign permite que você navegue de forma rápida e fácil pelos principais recursos, indicadores e componentes.

A seção superior da página inicial exibe detalhes sobre as últimas atualizações e novos recursos disponíveis no produto, com links para notas de versão e a documentação detalhada. Use a seta para a esquerda para mover-se pelos cartões de recursos.

![Captura de tela mostrando a página inicial com cartões de recursos e opções de navegação](assets/home.png){zoomable="yes"}

A seção **Principais indicadores de desempenho** permite que você verifique a eficácia da sua plataforma por meio de KPIs comuns. Saiba mais sobre esses KPIs [nesta página](../reporting/kpis.md).

A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário e as datas de criação e modificação. Clique no link **Mostrar mais** para carregar entregas adicionais.

Além disso, é possível acessar as principais páginas de ajuda do Adobe Campaign Web por meio da seção **Aprendizado** da página.

### Link Sobre {#user-interface-about}

>[!CONTEXTUALHELP]
>id="acw_about"
>title="Página Sobre"
>abstract="A página Sobre fornece detalhes sobre a instância do Adobe Campaign."

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="Sobre a instância "
>abstract="A seção Instância fornece informações importantes sobre seu cliente de console, incluindo a versão e o número de build associado."

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="Sobre a Web"
>abstract="A seção Web exibe a versão da interface do Campaign Web, com a data da última atualização, se disponível."

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="Sobre pacotes instalados"
>abstract="A seção Pacotes instalados lista todos os módulos, recursos e integrações presentes na instância."

Na parte inferior da página, o link **[!UICONTROL Sobre]** fornece detalhes sobre a instância do Adobe Campaign. Esses detalhes estão em modo somente leitura.

![Captura de tela mostrando o link Sobre na parte inferior da página](assets/about-link.png){zoomable="yes"}

A seção **Instância** fornece informações importantes sobre o cliente de console, incluindo a **versão** e o número de **build** associado.

* A **versão** refere-se à versão oficial de lançamento que você está usando.
* A **build** se refere a uma iteração específica dessa versão.

Os números de versão e build são essenciais para a solução de problemas, pois ajudam a determinar os recursos e correções presentes no seu ambiente.

A seção **Web** exibe a versão da interface do Campaign Web, juntamente com a data da última atualização, se disponível. Isso ajuda a monitorar alterações ou melhorias feitas na interface do Campaign Web.

A seção **Pacotes instalados** lista todos os módulos, recursos e integrações presentes na sua instância. Esses pacotes estendem a funcionalidade do Adobe Campaign, habilitando tarefas especializadas, como integração com outras soluções da Adobe ou suporte a fluxos de trabalho específicos. Dado o grande número de pacotes, é possível usar esta seção para consultar rapidamente se há um módulo específico instalado em sua instância.

![Captura de tela mostrando a seção Pacotes instalados com a funcionalidade de pesquisa](assets/about.png){zoomable="yes"}

## Menu de navegação esquerdo {#user-interface-left-nav}

Navegue pelos links à esquerda para acessar os recursos do Adobe Campaign Web. Vários links exibem listas de objetos que podem ser classificados e filtrados. Você também pode configurar colunas para exibir todas as informações necessárias. Consulte esta [seção](#list-screens). Algumas telas de lista são do tipo somente leitura. Os itens exibidos no menu de navegação esquerdo e nas listas dependem das permissões de usuário. Saiba mais sobre permissões [nesta seção](permissions.md).

### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="O menu **Explorer** exibe todos os componentes e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8, verifique as permissões associadas e crie pastas e subpastas neste menu."

O menu **Explorer** exibe todos os recursos e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8 e crie entregas, fluxos de trabalho e campanhas. 

Os itens exibidos no **Explorer** dependem das permissões de usuário. Também é possível adicionar pastas e subpastas caso você tenha os direitos adequados. Saiba mais sobre permissões [nesta seção](permissions.md).

Você pode configurar colunas para personalizar a exibição e visualizar todas as informações necessárias. Consulte esta [seção](#list-screens). Também é possível adicionar pastas e subpastas, conforme detalhado [nesta seção](permissions.md#folders).

Para obter mais informações sobre o Explorer do Campaign, a hierarquia de pastas e os recursos, consulte esta [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=pt-BR#ac-explorer-ui){target="_blank"}.

### Gerenciamento de campanhas {#user-interface-campaign-management}

A seção **Gerenciamento de campanhas** fornece acesso a campanhas de marketing, entregas e fluxos de trabalho.

* **Campanhas**: esta é a lista de suas campanhas e modelos de campanha. Por padrão, é possível ver as datas de início, término, criação e última modificação, o status atual e o nome do criador de cada campanha. É possível filtrar a lista por status, datas de início/término, pasta ou criar um filtro avançado para definir seus próprios critérios de filtragem. Saiba mais sobre campanhas [nesta seção](../campaigns/gs-campaigns.md).

* **Entregas**: navegue pela lista de entregas. Por padrão, é possível ver o estado, a data da última modificação e os principais KPIs. É possível filtrar a lista por status, data de contato ou canal. Clique em uma entrega de email para abrir o painel e obter uma visão geral dos detalhes da entrega. As entregas em outros canais são do tipo somente leitura. Saiba mais sobre entregas [nesta seção](../msg/gs-messages.md).

  Use o botão **Mais ações** para excluir ou duplicar uma entrega.

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"} [Captura de tela mostrando o botão Mais ações com opções para excluir ou duplicar uma entrega.]

* **Workflows** - Nessa tela, é possível acessar a lista completa de fluxos de trabalho e modelos de fluxos de trabalho. É possível verificar o status, as datas da última/próxima execução e criar um novo fluxo de trabalho ou um novo modelo de fluxo de trabalho. É possível filtrar a lista com os mesmos critérios de outros objetos. Além disso, é possível filtrar fluxos de trabalho que pertencem ou não a uma campanha. Saiba mais sobre fluxos de trabalho [nesta seção](../workflows/gs-workflows.md).

### Gerenciamento de conteúdo {#user-interface-content-management}

A seção **Gerenciamento de conteúdo** permite exibir seus modelos e fragmentos de conteúdo.

* **Modelos de conteúdo**: para um processo de design acelerado e aprimorado, você pode criar modelos independentes e reutilizar facilmente o conteúdo personalizado no [!DNL Adobe Campaign]. Disponível apenas para emails, essa funcionalidade permite que os usuários orientados por conteúdo trabalhem em modelos independentes para que a equipe de marketing possa reutilizá-los e adaptá-los em suas próprias campanhas de email. Saiba mais [nesta seção](../content/create-email-templates.md).

* **Fragmentos** - Um fragmento é um componente reutilizável que pode ser referenciado em uma ou mais entregas em campanhas. Ao modificar um fragmento, todos os conteúdos que o usam serão atualizados. [Aprenda a trabalhar com fragmentos](../content/fragments.md).

Essa funcionalidade permite pré-criar vários blocos de conteúdo personalizados que os usuários de marketing podem usar para organizar rapidamente o conteúdo do email com um processo de design aprimorado.

### Gerenciamento de clientes {#user-interface-customer-management}

Na seção **Gerenciamento de clientes**, é possível ver seus perfis, públicos-alvo e assinaturas. Essas listas são somente leitura.

* **Perfis**: crie e gerencie perfis e acesse o banco de dados do destinatário. Por padrão, é possível ver o endereço de email, nome e sobrenome. Saiba mais sobre perfis [nesta seção](../audience/about-recipients.md).
* **Públicos-alvo**: esta é a lista de públicos-alvo. Por padrão, é possível ver o tipo, a origem, a criação, as últimas datas de modificação e o rótulo. É possível filtrar a lista por origem. Saiba mais sobre públicos-alvo e listas [nesta seção](../audience/about-recipients.md).
* **Serviços de assinatura**: navegue pelas suas listas de assinaturas. Por padrão, é possível ver o tipo, o modo e o rótulo. Aprenda a gerenciar assinaturas e cancelamentos de assinaturas na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=pt-BR){target="_blank"}.
* **Filtros predefinidos**: são filtros personalizados criados e salvos para estarem disponíveis para uso futuro. Eles podem ser usados como atalhos durante qualquer operação de filtragem com o modelador de consulta, por exemplo, ao filtrar uma lista de dados ou criar o público-alvo de uma entrega. Saiba mais [nesta seção](predefined-filters.md).

### Gestão de decisões {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Navegue pelas listas de ofertas e modelos de ofertas que foram criados no console usando o módulo **Interação**. Essas listas são somente leitura."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/start/offers" text="Adicionar ofertas à uma entrega"

A seção **Gestão de decisões** permite ver as ofertas e os modelos de ofertas. Essas listas são somente leitura.

* **Ofertas**: navegue pela lista de ofertas e modelos de ofertas criados no console usando o módulo **Interação**. Por padrão, é possível ver o status, as datas de início/término e o ambiente. É possível filtrar a lista por status e datas de início/término. Os modelos de oferta também estão disponíveis.

Saiba como criar e enviar ofertas por email e SMS [nesta seção](../msg/offers.md).

### Relatórios {#left-nav-reporting}

* **Relatórios**: a entrada **Relatório** oferece um resumo geral consolidado das métricas de tráfego e engajamento de cada canal no ambiente do Campaign. Esses relatórios consistem em vários dispositivos, cada um oferecendo uma perspectiva distinta sobre a campanha ou o desempenho de entrega. Saiba mais [nesta seção](../reporting/global-reports.md).

### Administração {#left-nav-admin}

* **Trilha de auditoria**: a entrada **Trilha de auditoria** fornece aos usuários visibilidade total das modificações feitas em entidades importantes dentro da sua instância, em especial aquelas que afetam significativamente o bom funcionamento da instância. [Saiba mais](../reporting/audit-trail.md).

* **Contas externas**: crie novas contas externas usando a interface da Web para atender às suas necessidades específicas e garantir transferências de dados perfeitas. [Saiba mais](../administration/external-account.md).

* **Esquemas**: campos personalizados são outros atributos adicionados aos esquemas prontos para uso por meio do console do Adobe Campaign. [Saiba mais](../administration/custom-fields.md).

<!--* **Delivery Alerting** - Delivery Alerting is an alert management system that enables groups of users to automatically receive email notifications with information on their delivery executions. [Learn more](../msg/delivery-alerting.md).-->

## Saiba mais {#learn-more}

Saiba como procurar, pesquisar e filtrar listas disponíveis no ambiente do Campaign [nesta página](list-filters.md).



<!--CONTEXTUAL HELP TO DISPATCH IN DOCS ONCE FEATURE LIVE-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_notification"
>title="Entrega contínua"
>abstract="Entrega contínua"
