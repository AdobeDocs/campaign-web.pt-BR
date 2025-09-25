---
title: Introdução ao Adobe Campaign v8 para administradores e desenvolvedores.
description: Este tutorial fornece uma visão geral da principal funcionalidade administrativa e de gerenciamento de dados do Campaign v8. Ele é direcionado para administradores e profissionais de marketing técnico que estão migrando do Campaign Standard para o Campaign v8.
role: Admin, Developer
level: Beginner, Experienced
exl-id: 1554f85f-22e1-4b51-a916-194ea0d24816
source-git-commit: 2093338e3ba9f31954561171029ec0f7336c73c4
workflow-type: tm+mt
source-wordcount: '2777'
ht-degree: 9%

---

# Introdução para administradores e desenvolvedores {#acs-gs-admin}

Esta página fornece uma visão geral da principal funcionalidade administrativa e de gerenciamento de dados do Campaign v8. Ele é para administradores e profissionais técnicos de marketing que estão fazendo a transição do Campaign Standard para o Campaign v8.

A grande mudança para você é a introdução do console do cliente, o aplicativo nativo que se comunica com o servidor de aplicativos do Adobe Campaign.

O console do cliente do Campaign centraliza todos os recursos e configurações. Ele é sincronizado com a interface da Web do Campaign, garantindo a consistência entre os dois ambientes.

![](assets/client_console.png){zoomable="yes"}

[Saiba mais sobre a interface do usuário do console do cliente do Adobe Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"}.

## Arquitetura do Campaign v8 {#acs-gs-admi-archi}

A arquitetura do Campaign é detalhada na documentação do Campaign v8 (console). Aprenda o básico em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}.

Link útil para começar:

* Os componentes do Adobe Campaign e a arquitetura global estão descritos em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/ac-components){target="_blank"}.

* Consulte [Introdução à arquitetura do Campaign](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} para entender a arquitetura do Campaign antes de começar a estruturar sua instância.

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* As mensagens transacionais (Centro de mensagens) são o módulo do Campaign v8 criado para gerenciar mensagens acionadas. Depende de um modelo de arquitetura específico que é detalhado em [esta seção](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"}.

## Console do cliente do Campaign {#acs-gs-console}

### Instalar o console do cliente {#acs-gs-admin-console}

As tarefas de administração e configuração são executadas no console do cliente. A primeira etapa é configurar o ambiente.

O console do cliente do Campaign é um aplicativo nativo que se comunica com o servidor de aplicativos do Adobe Campaign por meio de protocolos padrão de Internet, como SOAP e HTTP. O Console do cliente do Campaign centraliza todos os recursos e configurações e requer largura de banda mínima, pois depende de um cache local. Projetado para facilitar a implantação, o console do cliente do Campaign pode ser implantado a partir de um navegador da Internet, atualizado automaticamente e não requer nenhuma configuração de rede específica, pois gera apenas tráfego HTTP(S).

O vídeo a seguir explica como baixar e instalar o Console do cliente do Adobe Campaign e gerenciar a conexão com sua instância.

>[!VIDEO](https://video.tv.adobe.com/v/335375?quality=12&learn=on){transcript=true}

Para obter mais informações, consulte [Conectar ao Campaign com o console do cliente](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/new/connect){target="_blank"}.

Observe que o console do cliente deve ser instalado em um ambiente compatível. Saiba mais na [matriz de compatibilidade do Campaign v8 (console)](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}.

### Conheça a interface do console do cliente  {#acs-gs-ui}

Saiba mais sobre a interface do usuário do Adobe Campaign v8 e como navegar pelos recursos principais com este vídeo tutorial.

>[!VIDEO](https://video.tv.adobe.com/v/334496?quality=12&learn=on){transcript=true}

Consulte [Trabalhar com o console do cliente](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} para obter mais detalhes.

## Administrar o ambiente {#acs-gs-admin-env}

Depois que o console do cliente for instalado, siga as etapas desta documentação para criar a conexão com o servidor de aplicativos: [Conexão com a documentação do servidor de aplicativos](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}.

As práticas de segurança estão profundamente enraizadas em nossos processos e ferramentas internos de desenvolvimento e operações de software e são rigorosamente seguidas por nossas equipes multifuncionais para evitar, detectar e responder a incidentes de maneira adequada. Saiba mais em [Práticas recomendadas de segurança do Campaign](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

### Direitos e permissões de acesso {#acs-gs-admin-rights}

O Adobe Campaign permite definir e gerenciar os direitos atribuídos aos usuários. Essas permissões são definidas combinando permissões de grupo de operadores, direitos nomeados e permissões em pastas.

Como usuário do Campaign Standard em transição para o Campaign v8, suas permissões e direitos de acesso permanecem os mesmos. Os grupos de segurança foram movidos pelo Adobe para os grupos de operadores do Campaign v8 e suas permissões por unidades organizacionais foram transferidas para permissões de pasta. Usuários do Campaign   use o Adobe ID para se conectar ao Campaign v8 e, em seguida, use o mesmo logon e senha do Campaign Standard.

Campanha [pastas](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} são nós na árvore do explorador do console do cliente. Com base no tipo, eles contêm determinados tipos de dados. Os programas são materializados por pastas no Campaign v8. É possível criar pastas e gerenciar permissões para elas, a fim de restringir o acesso. [Saiba mais](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Saiba mais na [documentação sobre permissões de usuário](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.


### Painel de controle do Campaign {#acs-gs-admin-cp}

Quanto ao Campaign Standard, você pode usar o Painel de controle do Campaign para administrar seu ambiente. Observe que, para a v8, o Painel de controle do Campaign fornece recursos adicionais.

O Painel de controle do Campaign ajuda a aumentar a eficiência do seu trabalho como administrador de produtos do Adobe Campaign, permitindo que você gerencie configurações e rastreie os usos de cada uma de suas instâncias. Sua interface intuitiva permite monitorar facilmente o uso dos principais ativos, além de realizar tarefas administrativas, como adicionar lista de permissão de endereços IP, monitoramento de armazenamentos SFTP, gerenciamento de chaves e muito mais.

Saiba mais nos [tutoriais do Painel de controle](https://experienceleague.adobe.com/en/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} e na [documentação do Painel de controle](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=pt-BR){target="_blank"}.

* **Adicionar endereços IP** - O Painel de Controle do Campaign permite configurar novas conexões para suas instâncias adicionando intervalos de endereços IP à lista de permissões. Saiba mais na [documentação da lista de permissões de IP](https://experienceleague.adobe.com/en/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

* **Configuração de subdomínio** - Você pode configurar uma subseção do seu domínio (tecnicamente uma &quot;zona DNS&quot;) para usar com o Adobe Campaign.
Saiba mais na [documentação de delegação de subdomínio](https://experienceleague.adobe.com/en/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

* **Gerenciar servidores SFTP** - No Painel de Controle, é possível interagir com todos os servidores SFTP conectados às instâncias do Campaign às quais você tem acesso. Saiba mais na [documentação de gerenciamento de SFTP](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Trilha de auditoria {#acs-gs-admin-audit-trail}

Como já está disponível no Campaign Standard, a Trilha de auditoria pode ser usada no Campaign v8 para acessar o histórico completo de alterações feitas na instância.

Na Interface do usuário da Web do Adobe Campaign, o recurso de trilha de auditoria fornece aos usuários visibilidade total de todas as modificações feitas em entidades importantes na sua instância, normalmente aquelas que afetam significativamente uma operação suave da instância. Saiba mais na [Documentação da trilha de auditoria](../../v8/reporting/audit-trail.md)

### Pacotes de dados {#acs-gs-admin-audit-packages}

Semelhante ao que pode ser obtido no Campaign Standard, os administradores podem definir pacotes para trocar recursos entre diferentes instâncias do Adobe Campaign por meio de arquivos XML estruturados. Eles podem ser parâmetros ou dados de configuração.

Você pode usar pacotes de dados para exportar e importar dados e configurações personalizadas da plataforma. Um pacote pode conter diferentes tipos de configurações e componentes, filtrados ou não. Saiba como trabalhar com pacotes de dados no Campaign v8 [nesta documentação](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/developer/packages){target="_blank"}.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### Personalizar a interface do usuário {#acs-gs-admin-ui}

Várias opções estão disponíveis para personalizar a interface do usuário no console do cliente, como:

* **Exibição de lista e dados** - As diretrizes para gerenciar configurações da interface do usuário, como listas, unidades ou exibição de dados, estão disponíveis neste documento: [Documentação de configurações da interface do usuário](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **Gerenciamento de pastas** - Pastas são objetos no Adobe Campaign que permitem organizar seus componentes e dados. Eles também são usados para gerenciar permissões. Saiba como [trabalhar com pastas](../../v8/get-started/work-with-folders.md).

* **Campos personalizados** - Os campos personalizados são atributos adicionais adicionados aos esquemas prontos para uso por meio do console do Adobe Campaign. Esses campos personalizados são exibidos em várias telas, por exemplo, os detalhes de um perfil ou um perfil de teste. Saiba mais na [documentação de configuração de campos personalizados](../../v8/administration/custom-fields.md).

## Configurar a identidade visual {#acs-gs-admin-branding}

Todas as empresas têm diretrizes de marca que definem os elementos visuais e os detalhes técnicos. Quanto ao Adobe Campaign Standard, o Adobe Campaign v8 ajuda você a gerenciar essas diretrizes de maneira central, para que possa apresentar uma imagem de marca consistente aos seus clientes em tudo o que você faz, desde logotipos em emails até URLs e domínios usados em suas campanhas. Como administrador técnico, você pode criar e gerenciar várias marcas no Adobe Campaign.

Saiba mais na [Documentação de marca](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}.

## Entender a criação do modelo de dados {#acs-gs-admin-data-model-creation}

Semelhante ao Campaign Standard, o Adobe Campaign v8 vem com seu modelo de dados predefinido. O Adobe Campaign depende de um banco de dados na nuvem que contém tabelas vinculadas. Saiba mais na [documentação sobre o modelo de dados](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}.

Um esquema é um documento XML associado a uma tabela de banco de dados. Ele define a estrutura de dados e descreve a definição SQL da tabela. Consulte a [documentação sobre criação de esquemas](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Saiba como criar um esquema e estender um esquema existente no Campaign v8 neste vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Semelhante aos recursos disponíveis no Campaign Standard, você pode criar recursos personalizados. No Campaign v8, os recursos personalizados são **esquemas** personalizados ou estendidos.

* Saiba como trabalhar com esquema [nesta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

* Saiba como estender um esquema existente em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}.

* Saiba como criar um novo esquema em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}.

* Ao criar ou estender um esquema, é necessário criar ou modificar os formulários de entrada associados para tornar essas alterações visíveis para os usuários finais. Um formulário de entrada permite editar uma instância associada a um schema de dados do console do cliente do Adobe Campaign. O formulário é identificado por seu nome e namespace. Consulte a [Documentação de criação de formulários de entrada](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Fluxos de trabalho e gerenciamento de dados {#acs-gs-admin-data-management}

Assim como no Adobe Campaign Standard, o Adobe Campaign v8 inclui um módulo de fluxo de trabalho que possibilita orquestrar a gama completa de processos e tarefas através dos módulos diferentes do servidor de aplicativos. Esse ambiente gráfico abrangente permite criar processos, incluindo segmentação, execução de campanha, processamento de arquivos, participação humana etc. O motor de workflow executa e rastreia esses processos. Saiba como iniciar fluxos de trabalho no Campaign v8 [nesta documentação](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/data/workflows){target="_blank"}.

Consulte os links para outros recursos úteis abaixo:

* Saiba o que são as dimensões de direcionamento e as tabelas de trabalho, e como o Adobe Campaign gerencia os dados em diferentes fontes de dados neste vídeo:

  >[!VIDEO](https://video.tv.adobe.com/v/339992?quality=12&learn=on){transcript=true}

* O Campaign ajuda a adicionar contatos ao banco de dados da nuvem. Você pode carregar um arquivo, agendar e automatizar várias atualizações de contato, coletar dados na Web ou inserir informações de perfil diretamente na tabela do recipient.  Saiba mais na [documentação de Importação de dados (console)](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/data/import){target="_blank"}.

* É possível exportar facilmente seus diferentes relatórios para o formato PDF ou CSV, o que permite compartilhá-los, manipulá-los ou imprimi-los. Saiba mais na [documentação sobre exportação de dados](../../v8/reporting/export-reports.md).

## REST APIs {#acs-gs-admin-apis}

As APIs REST do Campaign permitem criar integrações com o Adobe Campaign e criar seu próprio ecossistema, conectando o Adobe Campaign ao painel de tecnologias que você usa.

Como usuário do Campaign Standard em transição para o Campaign v8, as APIs REST estão disponíveis.

Saiba mais na [Documentação da API Rest](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}.

Observe que algumas recomendações e limitações se aplicam às APIs REST ao fazer a transição do Campaign Standard para o Campaign v8. Eles estão listados em [esta página](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/limitations){target="_blank"}. Restrições específicas também se aplicam durante a transição para o Campaign v8, conforme listado na Nota de disponibilidade abaixo:

>[!AVAILABILITY]
>
>* Os valores de PKEYs mudam entre a instância existente do Campaign Standard e a instância migrada do Campaign v8. Caso os PKEYs estejam sendo armazenados no banco de dados externo, a implementação precisa ser alterada de forma que seja necessário chamar as APIs principais do Adobe Campaign v8, que fornecem links pkeys/hrefs com PKEYs e as chamadas de API subsequentes precisam ser formadas dinamicamente pelo consumo de pkeys /hrefs das chamadas de API anteriores&#x200B;
>
>* No Campaign v8, para o mesmo corpo em que o veículo vinculado ao perfil&#x200B; receberíamos um erro de que a propriedade firstName não é válida para `cusVehicle`, mas um corpo de solicitação com apenas os atributos sem link funciona bem. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* O fuso horário é mostrado ao usuário como parte da chamada à API REST `profileAndServicesExt/profile` e não da chamada à API REST `profileAndServices/profile`, pois está sendo adicionado a um esquema estendido como parte da migração de dados.&#x200B;
>
>* O `ccpaOptOut` é mostrado ao usuário somente como parte da chamada à API REST `profileAndServicesExt/profile` e não da chamada à API REST `profileAndServices/profile`, pois está sendo adicionado em um esquema estendido como parte da migração de dados.
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## Privacidade e consentimento

Ao mudar do Campaign Standard para o Campaign v8, é importante analisar como as regulamentações de privacidade afetam suas operações de dados. Dependendo da sua empresa e das jurisdições nas quais você opera, os clientes podem ter o direito legal de acessar os dados que você mantém sobre eles ou solicitar sua exclusão.

No Campaign v8, todas as solicitações de privacidade devem ser gerenciadas por meio da integração do **Adobe Privacy Service**. Saiba mais na [documentação do Campaign v8 (console)](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/privacy/privacy).

Lembre-se de que o ambiente do Campaign Standard permanece ativo por um período após a transição. Durante esse período, as solicitações de privacidade podem chegar a ambos os sistemas. Para garantir a conformidade e evitar lacunas, fale com o Adobe Transition Manager para lidar corretamente com as solicitações em ambos os ambientes.

## Serviços de assinatura {#acs-gs-admin-sub}

Como no Campaign Standard, como administrador, você pode criar serviços de assinatura e os profissionais de marketing podem enviar mensagens aos assinantes. Os principais conceitos e etapas de implementação estão alinhados à Campaign Standard. Você pode encontrar links e vídeos úteis abaixo.

Saiba como configurar e gerenciar assinaturas e direcionar assinantes.

>[!VIDEO](https://video.tv.adobe.com/v/334305?quality=12&learn=on){transcript=true}

* Consulte a [documentação da interface de usuário da Web](../../v8/audience/manage-subscribers.md) dos serviços de assinatura.

* Consulte também a documentação para definir serviços de assinaturas no console do cliente em [esta seção](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"}.

## Mensagens e entregas{#acs-gs-msg}

### Configurar canais de entrega {#acs-gs-admin-channels}

Como Campaign Standard, o Adobe Campaign v8 ajuda a enviar campanhas entre canais, incluindo emails, SMS, notificações por push e correspondência direta, e medir sua eficácia usando vários relatórios dedicados. Essas mensagens são criadas e enviadas através de entregas e podem ser personalizadas para cada destinatário. As funcionalidades principais incluem direcionamento, definição e personalização de mensagens, execução de comunicações e relatórios operacionais associados. O principal ponto de acesso funcional é o assistente de entrega. Esse ponto de acesso leva a vários recursos cobertos pelo Adobe Campaign.

Como administrador, você deve definir as configurações de canal. Consulte os links abaixo para saber mais.

* **Email** - As configurações de email estão detalhadas em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"}.
* **SMS** - Saiba como configurar seu canal de SMS no [esta documentação](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.
* **Notificações por push** - As etapas para configurar o canal de notificações por push estão detalhadas [nesta seção](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
* **Mensagens transacionais** - As etapas para configurar [Mensagens transacionais](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} no Campaign v8 estão detalhadas [nesta seção](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### Contas externas {#acs-gs-ext-accounts}

Como administrador, você é responsável por configurar e manter as contas externas do Campaign. Como no Campaign Standard, as contas externas são usadas por processos técnicos, como workflows técnicos ou workflows da campanha.

O processo de transição para o Campaign v8 cuida das contas externas existentes do Campaign Standard.

Saiba mais na [documentação de conta externa](../../v8/administration/external-account.md).


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### Conteúdo dinâmico {#acs-gs-dyn-content}

Use o Campaign para criar conteúdo dinâmico e enviar mensagens personalizadas. Os recursos de personalização podem ser combinados para melhorar suas mensagens e criar uma experiência do usuário personalizada.

Com o Campaign v8, como administrador, você pode definir blocos de conteúdo dinâmico e como usá-los para personalizar o conteúdo do seu delivery de email neste vídeo:

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

Links úteis:

* [Introdução à personalização](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [Usar blocos de personalização](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [Criar conteúdo condicional](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [fontes de dados do Personalization](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### Modelos de entrega {#acs-gs-templates}

O uso de modelos de entrega é um requisito no Campaign v8, como no Campaign Standard.

Para um processo de design acelerado e aprimorado, crie modelos de delivery para reutilizar facilmente o conteúdo e as configurações personalizadas em suas campanhas. Essa funcionalidade permite padronizar a aparência criativa para ser mais rápido na execução e na inicialização de campanhas. Saiba como criar modelos de entrega na [interface da Web do Campaign](../../v8/msg/delivery-template.md). Veja também como criar modelos de entrega no console do cliente [nesta seção](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/send/create-templates){target="_blank"}.

### Regras de tipologia {#acs-gs-admin-rules}

Como administrador, você é responsável por criar e manter regras de tipologia para seus deliveries. Assim como no Adobe Campaign Standard, no Campaign v8, as regras de tipologia são regras de negócios que permitem executar verificações e filtrar a mensagem antes de enviá-la.

Ao fazer a transição de um ambiente do Campaign Standard para o Campaign v8, suas regras de tipologia são movidas para o Campaign v8.

No Campaign v8, as regras de tipologia vêm com uma Otimização de campanha específica. Este módulo permite controlar, filtrar e monitorar o envio de deliveries. Para evitar conflitos entre campanhas, o Adobe Campaign pode testar várias combinações aplicando regras de restrição específicas. Isso garante que as mensagens enviadas atendam às necessidades e expectativas dos clientes e às políticas de comunicação da empresa. Saiba mais na [documentação sobre regras de tipologia](https://experienceleague.adobe.com/pt-br/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}.

### Gerenciamento de quarentena {#acs-gs-admin-quarantine}

Todos os endereços em quarentena e as regras de quarentena foram migrados do seu ambiente do Campaign Standard para o Campaign v8. Nenhuma ação específica é necessária para o gerenciamento de quarentena.

Como administrador, familiarize-se com o gerenciamento de quarentena no Campaign v8 a partir de [esta página](../../v8/audience/quarantine.md). Consulte também a documentação detalhada do console do cliente sobre gerenciamento de quarentena em [esta seção](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"}.


## Gerenciar integrações do Adobe Campaign {#acs-gs-integrations}

Você pode conectar sua instância do Campaign com as soluções da Adobe Experience Cloud para combinar recursos. O Adobe Campaign vem com vários conectores que permitem a comunicação com aplicativos externos, conexão com mecanismos de banco de dados, compartilhamento e sincronização de dados. Saiba como combinar suas soluções na [esta documentação](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/integration){target="_blank"}.

Como um usuário do Campaign Standard que está migrando para o Campaign v8, o seguinte se aplica a você:

* Se você estava usando essas integrações com o Campaign Standard, suas configurações e dados do **Adobe Analytics** e do **Audience Manager** foram migrados pela Adobe.
* Se o seu ambiente do Campaign Standard foi integrado ao **Adobe Experience Manager**, a Adobe recomenda mudar para o **Adobe Experience Manager as a Cloud Service** para que você possa usar esse recurso ao criar emails na interface da Web do Campaign e facilitar o gerenciamento simplificado do conteúdo e dos formulários de entrega de email diretamente no seu ambiente do Adobe Experience Manager. Saiba mais em [esta página](../../v8/integrations/aem-content.md).
Observe que o Campaign também pode ser integrado ao Adobe Experience Manager 6.5. Para configurar essa integração, consulte [esta documentação](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}.
* Se seu ambiente do Campaign Standard foi integrado com **Triggers**, você deve configurar essa integração no Campaign v8 conforme detalhado em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}.
* Se seu ambiente do Campaign Standard foi integrado ao **Adobe Target**, você deve configurar essa integração no Campaign v8 conforme detalhado em [esta página](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}.
