---
title: Migração de usuários técnicos para o console do Adobe Developer
description: Saiba como migrar o gerenciamento de acesso do usuário do Campaign Standard para o Campaign V8
feature: Technote
role: Admin
exl-id: a7f333ba-0b84-47de-8f91-b6c8f3f3322a
source-git-commit: 31befa42b04bef1a2777df9f2bd494481ccf67cd
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 2%

---

# Gerenciamento de acesso do usuário do Campaign Standard para o Campaign V8 {#user-management-acs}

O Adobe Campaign Standard e o Adobe Campaign V8 permitem que os usuários definam e gerenciem permissões para usuários/operadores diferentes. Essas permissões consistem em direitos específicos que concedem aos usuários acesso a vários recursos do produto. No entanto, os dois produtos usam abordagens e implementações distintas para gerenciar o acesso do usuário.

Os seguintes conceitos são usados no Adobe Campaign Standard e no Campaign V8 para obter o gerenciamento de acesso do usuário:

| Campaign Standard | Campaign V8 |
|---------|----------|
| Usuário(a)  | Operador |
| Função | Nomeado à direita |
| Grupo de segurança | Grupo de Operadores |
| Entidade organizacional | Permissão de pasta |

## Abordagem de migração do grupo de segurança para o grupo de operadores

>[!CAUTION]
>
>Os recursos dessas Funções/Direitos nomeados podem variar na implementação, causando possivelmente problemas de autorização (por exemplo, elevação de privilégios ou interrupções de funcionalidade). Recomendamos que os usuários analisem esses mapeamentos após a transição para garantir o controle de acesso adequado. [Saiba mais sobre permissões](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

A tabela abaixo descreve a abordagem de migração para grupos de funções de usuário ao fazer a transição do Adobe Campaign Standard para o Campaign V8. No Campaign Standard, um **grupo de segurança**, conhecido como um **grupo de operadores** no Campaign V8, é usado para atribuir um conjunto de funções a um usuário. Embora alguns grupos de segurança/grupos de operadores estejam disponíveis prontamente, os usuários podem criar novos grupos ou modificar os existentes, se necessário.

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **Terminologia**  | Grupo de segurança | Grupo de Operadores |

Tanto no Adobe Campaign Standard quanto no Campaign V8, os **grupos de segurança** e os **grupos de operadores** estão mapeados para perfis de produto no Admin Console. Se quiser atribuir um **Grupo de segurança** ou **Grupo de operadores** a um usuário, você poderá vincular o **Perfil de produto** correspondente no Admin Console. Essa associação é sincronizada quando o usuário faz logon. [Saiba mais sobre o Perfil do produto](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

| **Grupo de segurança do Campaign Standard** | **Grupo de operadores do Campaign V8** |
|----------|---------|
| Administradores | Administradores |
| Supervisores de entrega | Administradores |
| Supervisores de workflow | Supervisores de workflow  |

## Abordagem de migração de Funções de usuário para Direitos nomeados

>[!CAUTION]
>
>Durante a migração do Adobe Campaign Standard para o Campaign V8, os usuários com a função **Modelo de Dados**, mas não **Administração**, terão acesso automático ao **Administração**, pois a criação de esquemas no Campaign V8 requer direitos de administração. Para evitar isso, remova a função de **Modelo de Dados** antes da migração.

No Adobe Campaign Standard, o termo **Função de usuário** é chamado de **Direito nomeado** no Campaign V8. A tabela abaixo descreve a terminologia usada para **Direitos nomeados** no Campaign V8 correspondente a **Funções do usuário** no Campaign Standard.

| **Função de Usuário do Campaign Standard** | **Campaign V8 com nome correto** | **Descrição**  |
|----------|---------|---------|
| Administração | Administração | O usuário com o direito de Administração tem acesso total à instância. |
| Modelo de dados  | Administração | Direito de executar publicações e criar recursos personalizados. Funcionalidade relacionada à criação de esquema disponível para o Administrador no Campaign V8.  |
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

>[!CAUTION]
>
>As unidades organizacionais na Adobe Campaign Standard sem **Todas (todas)** como um pai direto ou indireto não serão migradas para o Campaign V8.
></br>
>Os usuários em vários grupos de segurança recebem a unidade organizacional do grupo de segurança com a classificação mais alta. Se vários grupos tiverem unidades de nível superior paralelas, o logon é restrito no Campaign Standard, mas concede acesso mais amplo no Campaign v8 após a migração, o que pode aumentar os privilégios. Para evitar isso, evite atribuir usuários a grupos de segurança com unidades organizacionais paralelas.

No Adobe Campaign Standard, a **unidade organizacional** t está mapeada para o modelo de hierarquia **Pasta** existente no Campaign V8 para manter um controle de acesso semelhante. [Saiba mais sobre o gerenciamento de pastas](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

| | **Campaign Standard** | **Campaign V8** |
|---------|----------|---------|
| **Terminologia**  | Entidade organizacional | Pasta |

## Abordagem de migração do Programa

No Campaign V8, **Programas** são representados como **Pastas**. O Campaign V8 permite a criação de pastas e a restrição de acesso a elas.

Ao usar **Grupos** e **Direitos nomeados**, os **Operadores** podem receber acesso a **Pastas** específicas da hierarquia de navegação, com a capacidade de atribuir permissões de leitura, gravação e exclusão. [Saiba mais sobre o gerenciamento de pastas](https://experienceleague.adobe.com/pt-br/docs/campaign/campaign-v8/admin/permissions/folder-permissions)

Como um **Programa** é tratado como uma **Pasta** no Campaign V8, seu acesso pode ser gerenciado da mesma forma que qualquer outra pasta. Após a migração, os administradores do Campaign Standard podem seguir estas etapas:

1. No Explorer, clique com o botão direito do mouse em qualquer pasta e selecione **[!UICONTROL Propriedades...]**.

1. Navegue até a guia **[!UICONTROL Segurança]**.

1. Modifique as permissões do grupo de operadores de acordo com o modelo de acesso desejado. 

## Mapeamento de perfil de produto para acessar APIs REST 

Para acessar APIs transacionais da instância de execução no Campaign V8, é necessário um novo **Perfil de produto**, além dos perfis de produto **Administrador** e **Centro de Mensagens**. Este novo **Perfil de produto** será adicionado às contas técnicas existentes ou pré-criadas na Campaign Standard.

Após a migração, os usuários do Campaign Standard devem examinar seus **mapeamentos de Perfil de Produto** e atribuir o **Perfil de Produto** apropriado se não quiserem vincular suas **contas técnicas** ao Perfil de Produto do **Administrador**. Para integrações futuras, recomendamos usar a **ID do Locatário** do Campaign V8 na **URL REST** em vez da **ID do Locatário** do Campaign Standard anterior.

## Migração de acesso aos recursos integrados do Campaign para operadores do Campaign Standard

Os operadores migrados do Campaign Standard terão acesso de leitura a recursos integrados específicos no Campaign V8.

## Funções e grupos de segurança não migrados {#non-migrated-groups-roles}

Veja abaixo uma lista de funções do Campaign Standard que não foram migradas:

* Conta de Retransmissão Padrão 

* Push do Centro de mensagens 

Veja abaixo uma lista de mapeamentos de grupos de segurança do Campaign Standard que não foram migrados.

* Agentes do Centro de mensagens

* Agentes de push do centro de mensagens

* gerentes de aplicativos Adobe Experience Manager

* Conta de retransmissão

Observe que as funções personalizadas criadas e atribuídas a usuários no Adobe Campaign Standard não serão migradas para o Campaign V8.
