---
title: Migração de usuários técnicos para o console do Adobe Developer
description: Saiba como migrar o gerenciamento de acesso do usuário do Campaign Standard para o Campaign v8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 1dd416d0a1a3579075462821edd4d55e738e602f
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 2%

---

# Gerenciamento de acesso do usuário do Campaign Standard para o Campaign v8 {#user-management-acs}

O Adobe Campaign Standard e o Adobe Campaign v8 permitem que os usuários definam e gerenciem permissões para usuários/operadores diferentes. Essas permissões consistem em direitos específicos que concedem aos usuários acesso a vários recursos do produto. No entanto, os dois produtos usam abordagens e implementações distintas para gerenciar o acesso do usuário.

Os seguintes conceitos são usados no Adobe Campaign Standard e no Campaign v8 para obter o gerenciamento de acesso do usuário:

| Campaign Standard | Campaign v8 |
|---------|----------|
| Usuário(a)  | Operador |
| Função | Nomeado à direita |
| Grupo de segurança | Grupo de Operadores |
| Entidade organizacional | Permissão de pasta |

## Abordagem de migração do grupo de segurança para o grupo de operadores

>[!IMPORTANT]
>
>Os recursos dessas Funções/Direitos nomeados podem variar na implementação, causando possivelmente problemas de autorização (por exemplo, elevação de privilégios ou interrupções de funcionalidade). Recomendamos que os usuários analisem esses mapeamentos após a transição para garantir o controle de acesso adequado. [Saiba mais sobre permissões](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

A tabela abaixo descreve a abordagem de migração para grupos de funções de usuário ao fazer a transição do Adobe Campaign Standard para o Campaign v8. No Campaign Standard, um **grupo de segurança**, conhecido como um **grupo de operadores** no Campaign v8, é usado para atribuir um conjunto de funções a um usuário. Embora alguns grupos de segurança/grupos de operadores estejam disponíveis prontamente, os usuários podem criar novos grupos ou modificar os existentes, se necessário.

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologia**  | Grupo de segurança | Grupo de Operadores |

Tanto no Adobe Campaign Standard quanto no Campaign v8, os **grupos de segurança** e os **grupos de operadores** estão mapeados para perfis de produto no Admin Console. Se quiser atribuir um **Grupo de segurança** ou **Grupo de operadores** a um usuário, você poderá vincular o **Perfil de produto** correspondente no Admin Console. Essa associação é sincronizada quando o usuário faz logon. [Saiba mais sobre o Perfil do produto](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Grupo de segurança do Campaign Standard** | **Grupo de operadores do Campaign v8** |
|----------|---------|
| Administradores | Administradores |
| Supervisores de entrega | Administradores |
| Supervisores de workflow | Supervisores de workflow  |

## Abordagem de migração de Funções de usuário para Direitos nomeados

>[!IMPORTANT]
>
>Durante a migração do Adobe Campaign Standard para o Campaign v8, os usuários com a função **Modelo de Dados**, mas não **Administração**, terão acesso automático ao **Administração**, pois a criação de esquemas no Campaign v8 requer direitos de administração. Para evitar isso, remova a função de **Modelo de Dados** antes da migração.

No Adobe Campaign Standard, o termo **Função de usuário** é chamado de **Direito nomeado** no Campaign v8. A tabela abaixo descreve a terminologia usada para **Direitos nomeados** no Campaign v8 correspondente a **Funções do usuário** no Campaign Standard.

| **Função de Usuário do Campaign Standard** | **Direito nomeado do Campaign v8** | **Descrição**  |
|----------|---------|---------|
| Administração | Administração | O usuário com o direito de Administração tem acesso total à instância. |
| Modelo de dados  | Administração | Direito de executar publicações e criar recursos personalizados. Funcionalidade relacionada à criação de esquema disponível para o Administrador no Campaign v8.  |
| Capacidade de entrega  | Administração  | Direito de aprovar deliveries anteriormente analisados.  |
| Exportar | Exportar | Direito de exportar dados.  |
| Acesso ao arquivo  | Acesso a arquivos  | Direito de aprovar deliveries anteriormente analisados.  |
| Importação genérica  | Importar  | Direito de importação de dados genéricos |
| Preparar deliveries | Preparar deliveries | Direito de criar, modificar, preparar e excluir deliveries.  |
| Execução de Script SQL | Execução de Script SQL | Direito de executar qualquer comando SQL diretamente no banco de dados. |
| Iniciar deliveries  | Iniciar deliveries  | Direito de aprovar deliveries anteriormente analisados.  |
| Execução de Comando do Sistema | Execução do programa | Direito de executar comandos do sistema no servidor. |
| Fluxo de trabalho | Fluxo de trabalho | Direito de gerenciar a execução de workflows início, parada, pausa etc. |

## Abordagem de migração da unidade organizacional

>[!IMPORTANT]
>
>As unidades organizacionais na Adobe Campaign Standard sem **Todas (todas)** como um pai direto ou indireto não serão migradas para o Campaign v8.
></br>
>Os usuários em vários grupos de segurança recebem a unidade organizacional do grupo de segurança com a classificação mais alta. Se vários grupos tiverem unidades organizacionais paralelas de nível superior, o sistema selecionará a unidade organizacional para o usuário no Campaign Standard e o usuário só terá acesso à unidade organizacional selecionada pelo sistema e seus filhos. No Campaign v8 após a migração, o usuário teria acesso a **todas as unidades organizacionais atribuídas e seus filhos**, possivelmente aumentando os privilégios. Para evitar isso, evite atribuir usuários a grupos de segurança com unidades organizacionais paralelas. Saiba mais sobre [atribuição de unidade organizacional paralela](#parallel-assignments).


No Adobe Campaign Standard, a **unidade organizacional** está mapeada para o modelo de hierarquia **Pasta** existente no Campaign v8 para manter um controle de acesso semelhante. [Saiba mais sobre o gerenciamento de pastas](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign v8** |
|---------|----------|---------|
| **Terminologia**  | Entidade organizacional | Pasta |


### Sobre a atribuição de unidade organizacional paralela {#parallel-assignments}

Uma atribuição de unidade organizacional paralela ocorre quando um usuário tem acesso a várias unidades (atribuídas por meio de grupos de segurança) que existem em ramificações separadas da hierarquia sem ter acesso a uma unidade organizacional principal comum. Isso cria um risco de segurança durante a migração.

Por exemplo, considere a seguinte hierarquia de unidade organizacional:

![Diagrama de exemplo de atribuição de unidade organizacional paralela](assets/do-not-localize/parallel-org-units-sample.png){width="50%" zoomable="yes"}

Uma atribuição sem unidades organizacionais paralelas seria semelhante a:

![Sem diagrama de amostra da unidade organizacional paralela](assets/do-not-localize/without-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

Aqui, o usuário tem acesso às unidades organizacionais A, A1 e A2-1, todas conectadas na unidade organizacional principal A. O usuário pode acessar tudo em A.

A atribuição a seguir contém unidades organizacionais paralelas:

![Com diagrama de amostra da unidade organizacional paralela](assets/do-not-localize/with-parallel-org-units-assignment.png){width="50%" zoomable="yes"}

O usuário tem acesso a A1-1, A2 e A2-1, que existem em ramificações separadas sem pai atribuído comum.


**Implicações de segurança**

* No Campaign Standard, o sistema seleciona uma unidade organizacional de nível superior (A1-1 ou A2) para o usuário, limitando o acesso somente a essa unidade e seus filhos.
* Após a migração para o Campaign V8, o usuário obtém acesso aos recursos em todas as unidades organizacionais atribuídas e seus filhos.

**Resolução**

A atribuição de unidade organizacional paralela pode ser resolvida garantindo que todas as unidades organizacionais atribuídas a um usuário se enquadrem em uma única unidade pai comum que também esteja atribuída ao usuário.

Algumas maneiras de fazer isso são mencionadas abaixo:

1. Remover acesso a várias ramificações: cancele o acesso a várias ramificações paralelas e verifique se todo o acesso está em um único pai.
1. Atribuir um pai comum: conceda acesso a uma unidade organizacional principal comum apropriada que inclua todos os pontos de acesso necessários.
1. Reestruturar a hierarquia: modifique a estrutura da unidade organizacional para colocar todo o acesso necessário em uma única ramificação.

Para o exemplo acima, onde um usuário tem acesso a A1-1, A2 e A2-1, as etapas de resolução específicas são:

1. Remover o acesso a várias ramificações:

   1. Revogar acesso a A1-1, deixando somente acesso a A2 (que inclui A2-1), ou
   1. Revogar acesso a A2 e A2-1, deixando somente acesso a A1-1

1. Atribuir um pai comum:

   1. Conceder acesso à unidade organizacional A, que é a entidade pai comum de A1-1 e A2, ou
   1. Conceder acesso a Todos, que abrange toda a hierarquia

1. Reestruturar a hierarquia:

   1. Mova A1-1 em A2, ou
   1. Mover A2 e A2-1 em A1-1


## Abordagem de migração do Programa

No Campaign v8, **Programas** são representados como **Pastas**. O Campaign v8 permite a criação de pastas e a restrição de acesso a elas.

Ao usar **Grupos** e **Direitos nomeados**, os **Operadores** podem receber acesso a **Pastas** específicas da hierarquia de navegação, com a capacidade de atribuir permissões de leitura, gravação e exclusão. [Saiba mais sobre o gerenciamento de pastas](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Como um **Programa** é tratado como uma **Pasta** no Campaign v8, seu acesso pode ser gerenciado da mesma forma que qualquer outra pasta. Após a migração, os administradores do Campaign Standard podem seguir estas etapas:

1. No Explorer, clique com o botão direito do mouse em qualquer pasta e selecione **[!UICONTROL Propriedades...]**.

1. Navegue até a guia **[!UICONTROL Segurança]**.

1. Modifique as permissões do grupo de operadores de acordo com o modelo de acesso desejado. 

## Mapeamento de perfil de produto para acessar APIs REST 

Para acessar APIs transacionais da instância de execução no Campaign v8, é necessário um novo **Perfil de produto**, além dos perfis de produto **Administrador** e **Centro de Mensagens**. Este novo **Perfil de produto** será adicionado às contas técnicas existentes ou pré-criadas na Campaign Standard.

Após a migração, os usuários do Campaign Standard devem examinar seus **mapeamentos de Perfil de Produto** e atribuir o **Perfil de Produto** apropriado se não quiserem vincular suas **contas técnicas** ao Perfil de Produto do **Administrador**. Para integrações futuras, recomendamos usar a **ID do locatário** do Campaign v8 na **URL REST** em vez da **ID do locatário** do Campaign Standard anterior.

## Migração de acesso aos recursos integrados do Campaign para operadores do Campaign Standard

Os operadores migrados do Campaign Standard terão acesso de leitura a recursos integrados específicos no Campaign v8.

## Funções e grupos de segurança não migrados {#non-migrated-groups-roles}

Veja abaixo uma lista de funções do Campaign Standard que não foram migradas:

* Conta de Retransmissão Padrão 

* Push do Centro de mensagens 

Veja abaixo uma lista de mapeamentos de grupos de segurança do Campaign Standard que não foram migrados.

* Agentes do Centro de mensagens

* Agentes de push do centro de mensagens

* gerentes de aplicativos Adobe Experience Manager

* Conta de retransmissão

Observe que as funções personalizadas criadas e atribuídas a usuários no Adobe Campaign Standard não serão migradas para o Campaign v8.
