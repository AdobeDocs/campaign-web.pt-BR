---
title: Diferenças entre o Campaign Standard e o Campaign v8
description: Saiba o que muda ao fazer a transição do Campaign Standard para o Campaign v8 e onde encontrar os detalhes
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 5a6b111d1aaa2a34ce165eaf6d1b1a997fd8bc85
workflow-type: tm+mt
source-wordcount: '1916'
ht-degree: 3%
---
# Diferenças entre o Campaign Standard e o Campaign v8 {#acs-v8-differences}

A maioria dos conceitos é a mesma no Campaign Standard e no Campaign v8. Esta página reúne as diferenças que afetam você após a transição e os links para a página que explica cada uma. Ele complementa os guias para [profissionais de marketing](marketers.md) e para [administradores e desenvolvedores](admin-developers.md).

* Para ver as alterações de terminologia, consulte [Terminologia](#terminology).
* Para que as verificações sejam executadas e os problemas relatados após uma transição, consulte [Verificações e solução de problemas após a transição](post-transition-checks.md).
* Para os recursos que estão disponíveis somente no console do cliente, consulte [Console do cliente do Campaign Web e do Campaign](../../v8/get-started/capability-matrix.md).

## Terminologia {#terminology}

A maioria dos conceitos é semelhante entre o Adobe Campaign v8 e o Adobe Campaign Standard. No entanto, há algumas diferenças, começando pela terminologia.

| No Campaign Standard | No Campaign v8 |
|---|---|
| Recursos personalizados | **Esquemas** |
| Mensagens | **Entregas** |
| Usuários do produto | **Operadores** |
| Funções | Configurado com **Direitos Nomeados** |
| Grupos de segurança | **Grupos de operadores** |
| Unidades organizacionais | Gerenciado através de **Permissões de pasta** |

Além disso, como usuário existente do Campaign, observe que alguns conceitos foram renomeados para alinhar-se aos padrões de terminologia mais recentes. Essas alterações se aplicam somente à interface da Web do Campaign e não são refletidas no console do cliente.

| No Campaign Standard | No Campaign Web | Saiba mais |
|---|---|---|
| Destinatários | **Perfis** | [Perfis](../../v8/audience/gs-audiences-recipients.md) |
| Seed addresses | **Perfis de teste** | [Testar entregas](../../v8/preview-test/test-deliveries.md) |
| Análise de entrega | **Preparação da entrega**. Para iniciar a preparação da mensagem, clique no botão **Preparar**. | [Preparar e enviar](../../v8/monitor/prepare-send.md) |
| Visualização de email | Disponível pelo botão **Simular conteúdo**. | [Visualizar e testar](../../v8/preview-test/preview-test.md) |
| Listas | **Públicos-alvo** | [Públicos-alvo](../../v8/audience/gs-audiences-recipients.md) |

## Canais e conteúdo {#channels}

As etapas para criar e enviar mensagens são semelhantes nos dois produtos, conforme descrito no [guia para profissionais de marketing](marketers.md). As diferenças abaixo estão relacionadas à disponibilidade do canal, deliveries de teste, landing pages e workflows de mala direta.

| O que muda | Saiba mais |
|---|---|
| O canal no aplicativo não está disponível no Campaign v8. | [Canal no aplicativo](marketers.md#acs-gs-marketers-in-app) |
| Para fazer a transição de workflows e deliveries por push existentes, entre em contato com o Gerente de transição da Adobe Campaign. | [Notificações por push](marketers.md#acs-gs-marketers-push) |
| No Campaign Standard, um perfil de teste pode ser marcado como uma **Trap** para receber o envio final. No Campaign v8, adicione um **Grupo de interceptação** nas configurações de Público-alvo da entrega. | [Grupo de interceptação](../../v8/audience/trap-group.md) |
| As landing pages criadas na interface da Web do Campaign não são compatíveis com campos de entrada ocultos ou JavaScript personalizados. | [Páginas de destino](../../v8/landing-pages/get-started-lp.md) |
| No Campaign Standard, a transição de saída de uma atividade de correspondência direta também carregava o arquivo gerado. No Campaign v8, ele carrega somente a população direcionada. Para enviar o arquivo a um servidor, adicione uma atividade **Extração de dados** e depois uma atividade **Transferência de arquivos**. | [Correspondência direta](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## Públicos, fluxos de trabalho e entregas {#data-and-workflows}

Essas diferenças afetam os públicos-alvo e os fluxos de trabalho migrados do Campaign Standard, algumas opções de entregas recorrentes e da atividade **Transferência de arquivos**, além do escopo dos relatórios dinâmicos.

| O que muda | Saiba mais |
|---|---|
| Os públicos-alvo criados com a atividade Query no Campaign Standard se tornam [filtros predefinidos](../../v8/query/build-query.md) no Campaign v8. O Campaign v8 também é compatível com a atividade de Query. | [Gerenciar públicos-alvo](marketers.md#acs-gs-marketers-audiences) |
| Uma atividade Read audience se torna uma atividade Query com um filtro predefinido. | [Gerenciar públicos-alvo](marketers.md#acs-gs-marketers-audiences) |
| Um filtro predefinido assume somente o valor mais recente após a migração do público-alvo. | [Gerenciar públicos-alvo](marketers.md#acs-gs-marketers-audiences) |
| Públicos do tipo arquivo se tornam públicos do tipo Lista sem dimensões. | [Gerenciar públicos-alvo](marketers.md#acs-gs-marketers-audiences) |
| Os logs históricos de workflows executados no Campaign Standard não são migrados. | [Criar um fluxo de trabalho](marketers.md#acs-gs-marketers-wf) |
| No Campaign Standard, você pode selecionar o período de agregação de um email recorrente. Essa opção não está disponível no Campaign v8. | [Atividades de canal](../../v8/workflows/activities/channels.md) |
| Os relatórios dinâmicos abrangem entregas de email, campanhas com entregas de email e mensagens transacionais. | [Relatórios](marketers.md#acs-gs-marketers-reporting) |

## Acesso e segurança {#access}

Os grupos de segurança, as funções e as unidades organizacionais do Campaign Standard são mapeados para grupos de operadores, direitos nomeados e permissões de pasta durante a transição. Analise os pontos abaixo, em especial se alguns usuários tiverem direitos mais amplos ou mais restritos do que antes.

| O que muda | Saiba mais |
|---|---|
| Os grupos de segurança, as funções e as unidades organizacionais são mapeados para grupos de operadores, direitos nomeados e permissões de pasta. As funções personalizadas não são migradas. | [Gerenciamento de acesso do usuário](user-management-acs.md) |
| Os usuários com a função de **Modelo de Dados**, mas não com a função de **Administração**, recebem acesso de **Administração**. | [Gerenciamento de acesso do usuário](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| Os usuários atribuídos a grupos de segurança com unidades organizacionais paralelas podem ter acesso mais amplo no Campaign v8. | [Atribuição de unidade organizacional paralela](user-management-acs.md#parallel-assignments) |
| O acesso a APIs transacionais a partir da instância de execução requer um novo perfil de produto. | [Mapeamento de perfil de produto](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| As solicitações de privacidade podem chegar ao Campaign Standard e ao Campaign v8 durante o período em que o ambiente do Campaign Standard permanece ativo. | [Privacidade e consentimento](admin-developers.md#privacy-and-consent) |

## APIs e integrações {#apis-and-integrations}

Essas diferenças afetam as integrações que chamam o Campaign por meio da REST API e as integrações com outras soluções e ferramentas da Adobe.

| O que muda | Saiba mais |
|---|---|
| Os valores de PKEY são alterados após a migração. Se você armazenar PKEYs fora do Campaign, siga os hrefs retornados pela API. | [Uso da chave](#key-usage) |
| Alguns campos de perfil migrados, como fuso horário e `ccpaOptOut`, são retornados somente pela API `profileAndServicesExt/profile`. | [Fuso horário do perfil e ccpaOptOut](#profile-timezone) |
| O Adobe migra suas configurações do Adobe Analytics e do Audience Manager. Você deve configurar os Triggers e as integrações do Adobe Target novamente. | [Gerenciar integrações do Adobe Campaign](admin-developers.md#acs-gs-integrations) |

## Recomendações e limitações da API REST {#rest-api-limitations}

As recomendações e limitações abaixo se aplicam às REST APIs ao fazer a transição do Campaign Standard para o Campaign v8.

### Permissões e segurança {#permissions}

#### Mapeamento de perfis de produto {#rest-product-profiles}

No Campaign Standard, você recebeu acesso elevado à função de administrador para APIs, independentemente do perfil de produto atribuído. O Campaign v8 apresenta um conjunto diferente de perfis de produto, exigindo o mapeamento do Campaign Standard para perfis de produto do Campaign v8.

Com a migração, dois perfis de produto são adicionados às suas contas técnicas existentes ou pré-criadas: Administrador e Centro de mensagens (para acessar APIs transacionais). Revise o mapeamento do perfil de produto e atribua o perfil de produto necessário se não quiser que o perfil de produto do administrador seja mapeado com sua conta técnica.

#### ID do locatário

Após a migração, para qualquer integração futura, é recomendável usar sua **ID de locatário do Campaign v8** em URLs REST, substituindo sua ID de locatário anterior do Campaign Standard.

#### Uso da chave

O gerenciamento de valores PKey difere entre o Campaign Standard e o Campaign v8. Se você estava armazenando PKeys com o Campaign Standard, certifique-se de que sua implementação formará dinamicamente chamadas de API subsequentes usando PKeys ou hrefs obtidos de chamadas de API anteriores.

### APIs disponíveis {#available-apis}

Por enquanto, as APIs REST listadas abaixo estão disponíveis para uso:

* **Perfis**
* **Serviços e assinaturas**
* **Recursos personalizados**
* **Fluxos de trabalho**
* **Mensagens transacionais**

>[!AVAILABILITY]
>
>As REST APIs listadas abaixo estão obsoletas e não estão disponíveis para uso:
>* Histórico de marketing
>* Unidades organizacionais
>* Gerenciamento de privacidade

### Filtragem {#rest-filtering}

* Para usar os filtros em cargas da API REST, é necessário editá-los no Campaign v8 e fornecer um nome para usar em suas cargas. Para fazer isso, acesse os parâmetros adicionais do filtro na guia **[!UICONTROL Parâmetros]** e forneça o nome desejado no campo **[!UICONTROL Nome do filtro na API REST]**.

  ![](assets/api-filtering.png)


* O prefixo &quot;by&quot; necessário para usar filtros personalizados não é mais necessário. O nome do filtro deve ser usado como está em suas solicitações.

  Exemplo:

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### Campos de banco de dados descartados {#dropped-fields}

Alguns campos do banco de dados estão sendo removidos durante a migração. Ao usar um campo solto, as APIs REST retornarão valores em branco. No futuro, todos os campos ignorados serão descontinuados e removidos.

### POST com recursos vinculados {#post-linked}

Ao usar o seguinte formato de corpo de solicitação, com &quot;vehicleOwner&quot; representando o link para &quot;nms:recipient&quot;:

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

As informações do link são ignoradas. Consequentemente, um novo registro é gerado em &quot;cusVehicle&quot; contendo apenas valores de &quot;vehicleNumber&quot; e &quot;vehicleName&quot;. No entanto, o link permanece nulo, resultando em &quot;vehicleOwner&quot; sendo definido como nulo.

No Campaign v8, quando a mesma estrutura de corpo de solicitação é usada e o &quot;veículo&quot; é vinculado a um perfil, ocorre um erro. Este erro ocorre porque a propriedade &quot;firstName&quot; não é reconhecida como válida para &quot;cusVehicle&quot;. No entanto, um corpo de solicitação que inclui apenas os atributos sem o link funciona sem problemas.

### Operações do PATCH {#patch}

* O Campaign v8 não é compatível com o PATCH com um corpo de solicitação vazio: retorna um status 204 Sem conteúdo.
* Embora o Campaign Standard seja compatível com PATCH em elementos/atributos em um esquema, observe que as operações do PATCH no local não são compatíveis com o Campaign v8. Tentar um PATCH no local resultará em um Erro interno do servidor 500 com uma mensagem de erro indicando que a propriedade &#39;zipCode&#39; não é válida para o recurso &#39;profile&#39;.

### Respostas REST {#rest-responses}

A seção abaixo lista pequenas diferenças entre as respostas REST do Campaign Standard e do v8.

* Para registros GET únicos, a resposta inclui o href na resposta.
* Quando consultado com o atributo, o Campaign v8 fornece Count e Pagination na resposta.
* Após as operações POST, os valores dos recursos vinculados são retornados na resposta.

### Códigos de erro e mensagens {#rest-errors}

A seção abaixo lista as diferenças entre códigos de erro e mensagens do Campaign Standard e do Campaign v8.

| Cenário | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| Usar uma PKey inválida no corpo da solicitação | 500 - Atributo &#39;O5iRp40EGA&#39; desconhecido (consulte a definição do esquema &#39;Profiles (nms:recipient)&#39;). XTK-170036 Não é possível analisar a expressão &#39;@id = @O5iRp40EGA&#39;. | 404 - Não é possível descriptografar a PKey. (PKey=@jksad) |
| Usar uma PKey Inválida no URI | 500 - Atributo &#39;O5iRp40EGA&#39; desconhecido (consulte a definição do esquema &#39;Profiles (nms:recipient)&#39;). XTK-170036 Não é possível analisar a expressão &#39;@id = @O5iRp40EGA&#39;. | 404 - Não é possível descriptografar a PKey. (PKey=@jksad) Endpoint sem suporte. (endpoint=rest/profileAndServices/profile/@jksad) |
| Uso de duas Pkeys brutas diferentes no URI e no corpo da solicitação | 500 - RST-360011 Ocorreu um erro - entre em contato com o administrador. RST-360012 Operação inconsistente no recurso &#39;serviço&#39; - Não é possível atualizar a chave &#39;SVC3&#39; para &#39;SVC4&#39;. | 500 - Ocorreu um erro - entre em contato com o administrador. |
| Uso de PKey no URI e de uma PKey bruta diferente no corpo da solicitação | 500 - Já existe um &#39;Serviço&#39; com a mesma chave &#39;SVC4&#39;. PGS-220000 Erro PostgreSQL: ERRO: o valor de chave duplicado viola a restrição exclusiva &quot;nmsservice_name&quot; DETAIL: A chave (sname)=(SVC4) já existe. | 500 - Ocorreu um erro - entre em contato com o administrador. |
| Uso de ID bruta não existente no URI | 404 - RST-360011 Ocorreu um erro - entre em contato com o administrador. Não é possível localizar o documento com o caminho &#39;Service&#39; da chave &#39;adobe_nl:0&#39; (documento com o esquema &#39;service&#39; e o nome &#39;adobe_nl&#39;) | 404 - Não é possível localizar o documento com o caminho &#39;Service&#39; da chave &#39;adobe_nl&#39; (documento com o esquema &#39;service&#39; e o nome &#39;adobe_nl&#39;) |
| Uso de raw-id não existente no corpo da solicitação | 404 - RST-360011 Ocorreu um erro - entre em contato com o administrador. Não é possível localizar o documento com o caminho &#39;Service&#39; da chave &#39;adobe_nl&#39; (documento com o esquema &#39;service&#39; e o nome &#39;adobe_nl&#39;) | 404 - Não é possível localizar o documento com o caminho &#39;Service&#39; da chave &#39;adobe_nl&#39; (documento com o esquema &#39;service&#39; e o nome &#39;adobe_nl&#39;) |
| - | 500 - RST-360011 Ocorreu um erro - entre em contato com o administrador. | 500 - Ocorreu um erro - entre em contato com o administrador. |
| Insira um perfil/serviço com valor de enumeração de gênero inválido (ou qualquer coisa) | 500 - RST-360011 Ocorreu um erro - entre em contato com o administrador. O valor &#39;invalid&#39; não é válido para a enumeração &#39;nms:recipient:gender&#39; do campo &#39;@gender&#39; | 500 -Ocorreu um erro - entre em contato com o administrador. |

### Fuso horário do perfil e ccpaOptOut {#profile-timezone}

Com o Campaign Standard, o fuso horário é exibido como parte da resposta JSON de **profileAndServices/profile** chamadas de API REST.

Com o Campaign v8, o fuso horário é exibido somente para o usuário como parte das chamadas de API REST **profileAndServicesExt/profile**. Não faz parte das chamadas REST API **profileAndServices/profile** porque está sendo adicionado em um esquema estendido.

O mesmo se aplica ao campo `ccpaOptOut`: ele é mostrado apenas como parte das chamadas REST API **profileAndServicesExt/profile**, não das chamadas **profileAndServices/profile**, já que é adicionado em um esquema estendido como parte da migração de dados.

### Sinais externos de fluxo de trabalho {#workflow-signals}

A API GET do Campaign Standard Workflow retorna nomes de parâmetros, como as variáveis de instância do workflow e seus tipos de dados (booleano, string etc.). Isso é usado para criar o corpo da solicitação JSON formatado corretamente ao acionar o sinal por meio de uma chamada de API POST.

O Campaign v8 não é compatível com variáveis de instância de fluxo de trabalho de publicidade, mas espera que os desenvolvedores saibam o que são. Dessa forma, após a migração, as informações de parâmetros no corpo da solicitação POST precisarão ser construídas sem a disponibilidade de informações de parâmetros na resposta da API GET.
