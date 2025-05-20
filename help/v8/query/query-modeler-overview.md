---
audience: end-user
title: Trabalhar com o modelador de consultas
description: Saiba como trabalhar com o modelador de consultas à Web do Adobe Campaign.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 609718356ace500b831601dac077f9a3333e00e9
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 22%

---

# Trabalhar com o modelador de consultas {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Novo construtor de regras"
>abstract="Um novo construtor de regras agora está disponível para ajudar você a definir condições complexas em uma interface aprimorada. Você pode alternar do construtor de regras antigo para o novo, conforme necessário."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=pt-BR" text="Consulte as notas de versão"

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="Novo modelador de consultas"
>abstract="O Adobe Campaign Web apresenta um modelador de consultas que simplifica o processo de filtragem de bancos de dados, selecionando itens específicos com base em vários critérios. Isso inclui o uso de expressões e operadores avançados. O modelador de consultas está disponível em todo contexto onde é preciso definir regras para filtrar dados."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Modelador de consulta"
>abstract="Defina os critérios de filtragem para destinatários ou qualquer outra dimensão de direcionamento do banco de dados. Aproveite o público da Adobe Experience Platform para refinar ainda mais o seu público-alvo e maximizar o impacto da campanha."

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Refinar público-alvo"
>abstract="Essas regras só podem ser alteradas no console do cliente."

A interface de usuário da Web do Adobe Campaign apresenta um modelador de consultas que simplifica o processo de filtragem do banco de dados com base em vários critérios. Ele garante total compatibilidade com as queries criadas no console do cliente, facilitando uma transição contínua para a interface do usuário da Web.

Além disso, o modelador de consultas gerencia consultas muito complexas e longas com eficiência, oferecendo flexibilidade e precisão aprimoradas. Também oferece suporte a filtros predefinidos em condições, permitindo que os usuários refinem consultas com facilidade enquanto utilizam expressões e operadores avançados para estratégias abrangentes de direcionamento e segmentação de público.

## Acessar o modelador de consultas

O modelador de consultas está disponível em todo contexto onde é preciso definir regras para filtrar dados.

| Uso | Exemplo |
|  ---  |  ---  |
| **Definir públicos-alvo**: especifique a população que deseja direcionar em suas mensagens ou fluxos de trabalho e crie facilmente novos públicos-alvo adaptados às suas necessidades. [Saiba como criar públicos-alvo](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagem mostrando como acessar a interface de criação de público-alvo] |
| **Personalizar atividades do fluxo de trabalho**: aplique regras nas atividades do fluxo de trabalho, como **Divisão** e **Reconciliação**, para alinhar-se aos seus requisitos específicos. [Saiba mais sobre atividades de fluxo de trabalho](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagem mostrando como acessar opções de personalização de fluxo de trabalho] |
| **Filtros predefinidos**: crie filtros predefinidos que servem como atalhos durante várias operações de filtragem, quer você esteja trabalhando com listas de dados ou formando o público-alvo para uma entrega. [Saiba como trabalhar com filtros predefinidos](../get-started/predefined-filters.md) | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagem mostrando como acessar filtros predefinidos] |
| **Filtrar dados de relatórios**: adicione regras para filtrar os dados exibidos nos relatórios. [Saiba como trabalhar com relatórios](../reporting/gs-reports.md) | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagem mostrando como filtrar dados em relatórios] |
| **Personalizar listas**: crie regras personalizadas para filtrar os dados exibidos em listas como destinatários ou listas de entregas. [Saiba como filtrar listas](../get-started/list-filters.md#list-built-in-filters) | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [Imagem mostrando como personalizar filtros de lista] |
| **Criar conteúdo condicional**: torne o conteúdo do email dinâmico criando condições que definem qual conteúdo deve ser exibido para destinatários diferentes, garantindo mensagens personalizadas e relevantes. [Saiba como criar conteúdo condicional](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [Imagem mostrando como criar conteúdo condicional] |

>[!NOTE]
>
>Ao acessar um objeto criado no console do cliente onde as regras foram aplicadas, como um público ou um filtro predefinido, a seção **[!UICONTROL Refinar destino]** poderá ser exibida. Isso significa que parâmetros adicionais foram configurados para refinar o target da regra. Esses parâmetros só podem ser modificados no console.
>
>![Imagem mostrando um aviso sobre refinamento de destinos](assets/target-warning.png){zoomable="yes"}

## Interface do modelador de consulta {#interface}

O modelador de consulta fornece uma tela central onde você cria a consulta e um painel direito que fornece informações sobre a consulta.

>[!IMPORTANT]
>
>Uma interface totalmente nova para o modelador de Consulta está disponível. O novo construtor de regras permite criar a consulta com mais facilidade graças à interface simplificada. Para alternar para essa experiência, pressione o botão de alternância no canto superior direito. Você pode voltar para o modelador de Query clássico a qualquer momento que desejar simplesmente pressionando o botão de alternância de volta para desativar a nova interface. Você pode aplicar os mesmos princípios que o modelador de consultas nessa nova interface.
>![Imagem mostrando a alternância para a nova interface do construtor de regras](assets/query-modeler-toggle.png){zoomable="yes"}


>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Nova experiência do construtor de regras"
>abstract="Use esse botão de alternância para alternar entre o modelador de consultas clássico e a nova experiência do construtor de regras. O novo construtor de regras permite criar a consulta com mais facilidade, graças à interface simplificada e intuitiva."

![Imagem mostrando a interface do modelador de consultas](assets/query-interface.png){zoomable="yes"}

### A tela central {#canvas}

A tela central do modelador de consultas é onde você adiciona e combina os diferentes componentes para criar sua consulta. [Saiba como criar uma consulta](build-query.md)

>[!BEGINTABS]

>[!TAB Modelador de Consulta Clássica]

A barra de ferramentas localizada no canto inferior direito da tela fornece opções para manipular facilmente os componentes de consulta e navegar pela tela:

* **Modo de seleção múltipla**: selecione vários componentes de filtragem para copiá-los e colá-los no local de sua escolha.
* **Girar**: Alternar a tela verticalmente.
* **Ajustar à tela**: adapte o nível de zoom da tela à sua tela.
* **Menos zoom** / **Mais zoom**: Menos zoom ou mais zoom na tela.
* **Exibir mapa**: abra um instantâneo da tela mostrando sua localização atual.

>[!TAB Nova experiência do construtor de regras]

A barra de ferramentas localizada no canto superior direito da tela fornece opções para manipular facilmente os componentes de consulta e navegar pela tela:

* **Mover seleção para cima**: move o componente uma linha para cima.
* **Mover seleção para baixo**: move o componente uma linha para baixo.
* **Seleção de grupo**: coloque dois componentes em um grupo.
* **Desagrupar seleção**: Separe os componentes de um único grupo.
* **Expandir tudo**: expandir todos os grupos.
* **Recolher tudo**: Recolher todos os grupos.
* **Remover tudo**: remover todos os grupos e componentes.

>[!ENDTABS]

### O painel de propriedades Regra {#rule-properties}

No lado direito, o painel **[!UICONTROL Propriedades da regra]** fornece informações sobre a consulta. Ela permite executar várias operações para verificar a consulta e garantir que ela atenda às suas necessidades. Este painel é exibido ao criar uma consulta para criar um público-alvo. [Saiba como verificar e validar sua consulta](build-query.md#check-and-validate-your-query)
