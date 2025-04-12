---
audience: end-user
title: Conheça a interface
description: Interface do Adobe Campaign Web
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1548'
ht-degree: 49%

---

# Conheça a interface {#user-interface}

A nova interface da Web do Adobe Campaign fornece uma experiência do usuário moderna e intuitiva para simplificar o design e o delivery de campanhas de marketing. Essa interface se integra a aplicativos e soluções da Adobe Experience Cloud.

Saiba como se conectar ao Adobe Campaign e explorar as noções básicas de navegação do Experience Cloud [neste artigo](connect-to-campaign.md).

>[!NOTE]
>
>Essa documentação é atualizada com frequência para refletir as alterações mais recentes na interface do usuário do produto. No entanto, algumas capturas de tela podem ser um pouco diferentes da interface do usuário.

## Página inicial do Campaign {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recentes"
>abstract="A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação."

A home page do Campaign permite navegar de maneira rápida e fácil pelos principais recursos, indicadores e componentes.

A seção superior da página inicial exibe detalhes sobre as atualizações mais recentes e os novos recursos disponíveis no produto, com links para as Notas de versão e a documentação detalhada. Use a seta para a esquerda para rolar pelos cartões de recursos.

![Captura de tela mostrando a página inicial com cartões de recursos e opções de navegação](assets/home.png){zoomable="yes"}

A seção **Indicadores-chave de desempenho** permite verificar a eficácia da plataforma por meio de KPIs comuns. Saiba mais sobre esses KPIs [nesta página](../reporting/kpis.md).

A lista **Recentes** fornece atalhos para as entregas criadas e modificadas recentemente. Esta lista mostra o canal, status, proprietário, datas de criação e modificação. Clique no link **Mostrar mais** para carregar entregas adicionais.

Além disso, você pode acessar as principais páginas de ajuda da Web do Adobe Campaign na seção **Aprendizado** da página.

### Link Sobre {#user-interface-about}

>[!CONTEXTUALHELP]
>id="acw_about"
>title="Página Sobre"
>abstract="A página Sobre fornece detalhes sobre a instância do Adobe Campaign."

>[!CONTEXTUALHELP]
>id="acw_about_instance"
>title="Sobre a Instância "
>abstract="A seção Instância fornece informações importantes sobre o cliente do console, incluindo a versão e o número de build associado."

>[!CONTEXTUALHELP]
>id="acw_about_web"
>title="Sobre a Web"
>abstract="A seção Web exibe a versão da interface do Campaign Web, com a data da última atualização, se disponível."

>[!CONTEXTUALHELP]
>id="acw_about_packages"
>title="Sobre pacotes instalados"
>abstract="A seção Pacotes instalados lista todos os módulos, recursos e integrações presentes na instância."

Na parte inferior da página, o link **[!UICONTROL Sobre]** fornece detalhes sobre a instância do Adobe Campaign. Esses detalhes estão no modo somente leitura.

![Captura de tela mostrando o link Sobre na parte inferior da página](assets/about-link.png){zoomable="yes"}

A seção **Instância** fornece informações importantes sobre o cliente de console, incluindo a **versão** e o número de **build** associado.

* A **versão** se refere à versão oficial que você está usando.
* A **build** se refere a uma iteração específica dessa versão.

Os números de versão e build são essenciais para a solução de problemas, pois ajudam a determinar os recursos e correções presentes em seu ambiente.

A seção **Web** exibe a versão da interface da Web do Campaign, juntamente com a data da última atualização, se disponível. Isso ajuda a rastrear alterações ou melhorias feitas na interface do Campaign Web.

A seção **Pacotes instalados** lista todos os módulos, recursos e integrações presentes na sua instância. Esses pacotes ampliam a funcionalidade do Adobe Campaign, permitindo tarefas especializadas, como a integração com outras soluções da Adobe ou o suporte a workflows específicos. Dado o grande número de pacotes, você pode pesquisar nesta seção para verificar rapidamente se um módulo específico está instalado em sua instância.

![Captura de tela mostrando a seção Pacotes instalados com a funcionalidade de pesquisa](assets/about.png){zoomable="yes"}

## Menu de navegação esquerdo {#user-interface-left-nav}

Navegue pelos links à esquerda para acessar os recursos do Adobe Campaign Web. Vários links exibem listas de objetos que podem ser classificados e filtrados. Você também pode configurar colunas para exibir todas as informações necessárias. Consulte esta [seção](#list-screens). Algumas telas de lista são do tipo somente leitura. Os itens exibidos no menu de navegação esquerdo e nas listas dependem das permissões de usuário. Saiba mais sobre permissões [nesta seção](permissions.md).

### Explorer {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Explorer"
>abstract="O menu **Explorer** exibe todos os componentes e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Procure todos os componentes, pastas e esquemas do Campaign v8, verifique as permissões associadas e crie pastas e subpastas neste menu."

O menu **Explorer** exibe todos os recursos e objetos do Campaign com a mesma hierarquia de pastas que a do console do cliente. Navegue por todos os componentes, pastas e esquemas do Campaign v8 e crie entregas, fluxos de trabalho e campanhas.

Os itens exibidos no **Explorer** dependem das permissões de usuário. Também é possível adicionar pastas e subpastas se você tiver os direitos apropriados. Saiba mais sobre permissões [nesta seção](permissions.md).

Você pode configurar colunas para personalizar a exibição e visualizar todas as informações necessárias. Consulte esta [seção](#list-screens). Também é possível adicionar pastas e subpastas, conforme detalhado [nesta seção](permissions.md#folders).

Para obter mais informações sobre o explorador do Campaign, a hierarquia de pastas e os recursos, consulte esta [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=pt-BR#ac-explorer-ui){target="_blank"}.

### Gerenciamento de campanhas {#user-interface-campaign-management}

Na seção **Campaign management**, você pode acessar campanhas de marketing, entregas e fluxos de trabalho.

* **Campanhas** - Esta é a lista de suas campanhas e modelos de campanha. Por padrão, para cada campanha, é possível visualizar as datas de início, término, criação e última modificação, o status atual e o nome do operador da campanha que a criou. É possível filtrar a lista por status, datas de início/término, pasta ou criar um filtro avançado para definir seus próprios critérios de filtragem. Saiba mais sobre campanhas [nesta seção](../campaigns/gs-campaigns.md).

* **Entregas**: navegue pela lista de entregas. Por padrão, é possível visualizar o estado, a data da última modificação e os KPIs principais. É possível filtrar a lista por status, data de contato ou canal. Clique em uma entrega de email para abrir o painel e obter uma visão geral dos detalhes da entrega. As entregas em outros canais são do tipo somente leitura. Saiba mais sobre entregas [nesta seção](../msg/gs-messages.md).

  Use o botão **Mais ações** para excluir ou duplicar uma entrega.

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"} [Captura de tela mostrando o botão Mais ações com opções para excluir ou duplicar uma entrega.]

* **Workflows** - Nessa tela, é possível acessar a lista completa de workflows e modelos de workflows. É possível verificar o status, as datas da última/próxima execução e criar um novo workflow ou um novo modelo de workflow. É possível filtrar a lista com os mesmos critérios de outros objetos. Além disso, você pode filtrar workflows que pertencem ou não a uma campanha. Saiba mais sobre fluxos de trabalho [nesta seção](../workflows/gs-workflows.md).

### Gerenciamento de conteúdo {#user-interface-content-management}

Na seção **Gestão de conteúdo**, você pode exibir seus modelos e fragmentos de conteúdo.

* **Modelos de conteúdo**: para um processo de design acelerado e aprimorado, você pode criar modelos independentes e reutilizar facilmente o conteúdo personalizado no [!DNL Adobe Campaign]. Disponível apenas para emails, essa funcionalidade permite que os usuários orientados por conteúdo trabalhem em modelos independentes para que a equipe de marketing possa reutilizá-los e adaptá-los em suas próprias campanhas de email. Saiba mais [nesta seção](../email/create-email-templates.md).

* **Fragmentos** - Um fragmento é um componente reutilizável que pode ser referenciado em uma ou mais entregas em campanhas. Ao modificar um fragmento, todos os conteúdos que o usam serão atualizados. [Saiba como trabalhar com fragmentos](../content/fragments.md).

Essa funcionalidade permite pré-criar vários blocos de conteúdo personalizados que os usuários de marketing podem usar para reunir rapidamente o conteúdo de email em um processo de design aprimorado.

### Gerenciamento de clientes {#user-interface-customer-management}

Na seção **Gerenciamento de clientes**, você pode exibir seus perfis, públicos-alvo e assinaturas. Essas listas são do tipo somente leitura.

* **Perfis**: crie e gerencie perfis e acesse o banco de dados do destinatário. Por padrão, você pode exibir o endereço de email, nome e sobrenome. Saiba mais sobre perfis [nesta seção](../audience/about-recipients.md).
* **Públicos-alvos**: esta é a lista de públicos. Por padrão, você pode exibir o tipo, a origem, a criação, as datas da última modificação e o rótulo. É possível filtrar a lista por origem. Saiba mais sobre públicos-alvo e listas [nesta seção](../audience/about-recipients.md).
* **Serviços de assinatura** - Procure suas listas de assinatura. Por padrão, é possível visualizar o tipo, o modo e o rótulo. Saiba mais sobre como gerenciar assinaturas e seus cancelamentos na [documentação do Adobe Campaign v8 (console)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=pt-BR){target="_blank"}.
* **Filtros predefinidos** - Filtros predefinidos são filtros personalizados criados e salvos para ficarem disponíveis para uso futuro. Elas podem ser usadas como atalhos durante qualquer operação de filtragem com o modelador de consultas, por exemplo, ao filtrar uma lista de dados ou criar o público-alvo de um delivery. Saiba mais [nesta seção](predefined-filters.md).

### Gestão de decisões {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Ofertas"
>abstract="Navegue pelas listas de ofertas e modelos de ofertas que foram criados no console usando o módulo **Interação**. Essas listas são do tipo somente leitura."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=pt-BR" text="Adicionar ofertas à uma entrega"

Na seção **Gestão de decisões**, você pode exibir as ofertas e os modelos de ofertas. Essas listas são do tipo somente leitura.

* **Ofertas** - Navegue pela lista de ofertas e modelos de ofertas criados no console usando o módulo **Interação**. Por padrão, você pode visualizar o status, as datas de início/término e o ambiente. É possível filtrar a lista por status e datas de início/término. Os modelos de oferta também estão disponíveis.

Saiba como criar e enviar ofertas por email e SMS [nesta seção](../msg/offers.md).

### Relatórios {#left-nav-reporting}

* **Relatórios**: a entrada **Relatório** oferece um resumo geral consolidado das métricas de tráfego e engajamento de cada canal no ambiente do Campaign. Esses relatórios consistem em vários dispositivos, cada um oferecendo uma perspectiva distinta sobre a campanha ou o desempenho de entrega. Saiba mais [nesta seção](../reporting/global-reports.md).

### Administração {#left-nav-admin}

* **Trilha de auditoria** - A entrada **Trilha de auditoria** fornece aos usuários visibilidade total de todas as modificações feitas em entidades importantes em sua instância, normalmente aquelas que afetam significativamente a operação suave da instância. [Saiba mais](../reporting/audit-trail.md).

* **Contas externas** - Crie novas contas externas usando a Interface de Usuário da Web para atender às suas necessidades específicas e garantir transferências de dados sem interrupção. [Saiba mais](../administration/external-account.md).

* **Esquemas**: campos personalizados são outros atributos adicionados aos esquemas prontos para uso por meio do console do Adobe Campaign. [Saiba mais](../administration/custom-fields.md).

* **Alertas de entrega**: é um sistema de gerenciamento de alertas que permite que grupos de usuários recebam automaticamente notificações por email com informações sobre suas execuções de entrega. [Saiba mais](../msg/delivery-alerting.md).

## Saiba mais {#learn-more}

Saiba como procurar, pesquisar e filtrar listas disponíveis no ambiente do Campaign [nesta página](list-filters.md).