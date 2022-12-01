---
audience: end-user
title: Configurações avançadas
description: Documentação da Web do Campaign v8
source-git-commit: c90d8a5eff6169945d381f3250cb3e4d06194d31
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 34%

---

# Configurações avançadas {#advanced-settings}

>[!NOTE]
>
>Esta documentação está em construção e é atualizada com frequência. A versão final desse conteúdo estará pronta em janeiro de 2023.

Essas configurações são parâmetros técnicos de delivery definidos no template de email. Se quiser modificar qualquer um deles para um delivery específico, continue com cautela.

## Configurações de delivery de email {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Todos os parâmetros técnicos de delivery do template.
Somente altere parâmetros, sem criação aqui.
De acordo com permissões, os profissionais não devem modificar isso, tenha cuidado. Verifique e altere somente a regra de tipologia -> rest definido no modelo

## Tipologia {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Tipologia"
>abstract="A tipologia permite controlar, filtrar e monitorar o envio de deliveries."

### Parâmetro de pressão {#pressure-parameter}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Peso da entrega"
>abstract="Os pesos do delivery permitem identificar deliveries de alta prioridade dentro da estrutura do gerenciamento de pressão. As mensagens com o peso mais alto têm prioridade."

### Configurações de capacidade {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Importância do destinatário"
>abstract="TBC"


## Público-alvo {#audience}

## Entrega {#delivery}

### Tentativas {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Número máximo de tentativas"
>abstract="Se uma mensagem falhar devido a um erro temporário, novas tentativas serão executadas durante a duração do delivery."

## Aprovação {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Aprovação modo"
>abstract="Cada etapa de um delivery pode ser sujeita a aprovação para garantir o monitoramento e o controle totais dos vários processos."

## Validade {#validity}

### Período de validade {#validity-period}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Duração da entrega"
>abstract="O campo Delivery duration permite inserir o limite de novas tentativas de delivery globais. Isso significa que o Adobe Campaign envia as mensagens começando na data de início e, em seguida, para mensagens que retornam somente um erro, tentativas regulares e configuráveis são executadas até que o limite de validade seja atingido."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Limite da validade de recursos"
>abstract="O campo Validity limit é usado para recursos carregados, principalmente para a mirror page e imagens. Os recursos desta página são válidos por um tempo limitado."


### Rastreamento {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Período de validade"
>abstract="Essa opção define a duração para a qual o rastreamento será ativado nos URLs."














