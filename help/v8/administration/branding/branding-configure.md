---
title: Identidade visual
description: Saiba como configurar sua marca
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 29%

---

# Configurar marcas {#branding-configure}

>[!IMPORTANT]
>
>As marcas não podem ser criadas ou modificadas pelos usuários finais: essas operações têm de ser efetuadas pelo administrador técnico do Adobe Campaign. Para receber qualquer solicitação, entre em contato com o Atendimento ao cliente da Adobe.

No Adobe Campaign V8, as Marcas podem ser encontradas no menu **[!UICONTROL Administração > Plataforma > Marca]**.

Uma **[!UICONTROL Marca]** é definida pelas seguintes características:

* Uma **[!UICONTROL identidade]** que define e personaliza sua marca. Esta seção contém os seguintes campos:

   * **[!UICONTROL Rótulo]** visível na interface
   * **[!UICONTROL ID]**
   * **[!UICONTROL Nome da marca]**
   * **[!UICONTROL URL do site]** e **[!UICONTROL Rótulo do site]** da marca
   * **[!UICONTROL Logotipo da marca]**

  ![](assets/branding_1.png)

* **[!UICONTROL Parâmetros de cabeçalho de emails enviados]** que personaliza o que os recipients das campanhas verão. Esta seção contém os seguintes campos:

   * **[!UICONTROL Remetente (endereço de email)]** com o endereço de email da marca.
   * **[!UICONTROL Remetente (nome)]** com o nome da marca.
   * **[!UICONTROL Responder a (endereço de email)]** com o endereço de email ao qual o cliente pode responder.
   * **[!UICONTROL Responder a (nome)]** com o nome da marca.
   * **[!UICONTROL Erro (endereço de email)]** com o endereço de email que será usado em caso de erro.

  >[!IMPORTANT]
  >
  >Após atualizar os parâmetros de cabeçalho dos emails, caso o nome e o endereço de email do remetente não tiverem sido alterados no email criado a partir do modelo, verifique as configurações avançadas do modelo.

  ![](assets/branding_2.png)

* As **[!UICONTROL Configurações de marca]** definem os servidores usados para rastreamento também para acesso à página de aterrissagem. Esta seção contém os seguintes campos:

   * **[!UICONTROL Subdomínio da marca]** refere-se à URL do subdomínio designado específica para essa marca, solicitada para delegação da Adobe.

  Observe que a configuração para rastreamento, espelhamento e servidores de aplicativos é armazenada em contas externas separadas associadas ao roteamento. Essas configurações são aplicadas durante o provisionamento e não devem ser modificadas. Para exibir URLs, acesse a guia **[!UICONTROL Prefixos de marca]** da sua conta externa.

  ![](assets/branding_3.png)

* O menu **[!UICONTROL Configurações de URL de rastreamento]** permite que você aprimore o rastreamento de URL definindo parâmetros adicionais para integração com ferramentas de análise da Web, como Adobe Analytics e Google Analytics.

  Use o menu **[!UICONTROL Parâmetros de URL Adicionais]** para criar parâmetros adicionais como pares de valor-chave junto com suas condições de aplicabilidade. Cada nome de parâmetro deve ser exclusivo e não vazio, e cada valor de parâmetro deve ser não vazio. A condição de aplicabilidade pode estar vazia, mas nenhum desses valores pode incluir tags JST.

  Esses parâmetros serão aplicados às URLs rastreadas que correspondem a qualquer nome de domínio especificado na **[!UICONTROL Lista de Nomes de Domínio]**, que pode incluir expressões regulares.

  **Exemplo:** Uma URL rastreada como `https://www.example.com` se tornará `https://www.example.com/?age=21&deliveryName=DM101` quando os parâmetros adicionais `age=21` e `deliveryName=DM101` estiverem configurados para esse domínio.

## Configurar identidade visual para mensagens transacionais {#branding-transactional-config}

>[!IMPORTANT]
>
>Esta seção se aplica somente a mensagens transacionais (Centro de Mensagens).
>
>Embora os recursos transacionais estejam disponíveis na interface do usuário da Web do Campaign, as etapas abaixo devem ser executadas no console do cliente do Campaign v8 (instância de controle).

Se você estiver usando mensagens transacionais (Centro de mensagens) com marca, será necessária uma configuração adicional.

### Fórmulas de rastreamento para instâncias em tempo real

Quando a identidade visual é ativada em uma instância de controle em tempo real (RT), opções específicas de rastreamento são usadas para gerenciar fórmulas de rastreamento. Essas fórmulas são configuradas centralmente na instância de Controle RT, em vez de individualmente em cada instância de Execução RT.

As opções a seguir definem as fórmulas de rastreamento usadas pelos deliveries de RT:

* **`NmsTracking_RT_ClickFormula`**: especifica a fórmula usada para rastreamento de cliques em instâncias RT

* **`NmsTracking_RT_OpenFormula`**: especifica a fórmula usada para rastreamento aberto em instâncias RT

Se sua implementação exigir fórmulas de rastreamento personalizadas para mensagens transacionais, use a opção abaixo:

* **`Branding_RT_ListXtkOptions_toPublish`**: liste aqui os nomes de opção XTK para suas fórmulas personalizadas (separadas por vírgulas). Isso garante que os deliveries de RT possam aplicar as fórmulas de rastreamento personalizadas.