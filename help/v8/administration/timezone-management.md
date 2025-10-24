---
title: Gerenciamento de fuso horário
description: Saiba como a interface do usuário da Web do Adobe Campaign exibe valores de data e hora com base no navegador, operador, fluxo de trabalho e fusos horários do servidor.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 4%

---

# Gerenciamento de fuso horário {#timezone-management}

A interface do usuário da Web do Adobe Campaign exibe todos os valores de data e hora de acordo com o **fuso horário local do navegador da Web do usuário**. Esse comportamento pode levar a diferenças ao comparar carimbos de data e hora entre a interface da Web e o console do cliente.

Esta seção explica as diferenças esperadas entre os fusos horários da **Interface do Usuário da Web**, **Console do Cliente** e **execução do fluxo de trabalho**.

>[!NOTE]
>
>Nenhum dado armazenado no servidor é modificado. Somente sua exibição na interface é alterada.

## Principais conceitos

* **Fuso horário do servidor**: o fuso horário do servidor corresponde ao fuso horário configurado no sistema operacional do servidor. Todos os carimbos de data e hora são armazenados internamente em UTC no servidor.

* **Comportamento do Console do Cliente**: o Console do Cliente exibe carimbos de data/hora usando o **fuso horário do operador**, definido nas configurações do operador. Por padrão, isso corresponde ao fuso horário do **servidor**.

* **Comportamento da interface da Web**: a interface da Web exibe carimbos de data/hora usando o **fuso horário local do navegador**. Quando um usuário altera o fuso horário do navegador ou do sistema, os valores de data/hora exibidos são atualizados automaticamente.

* **Comportamento do fluxo de trabalho**: os fluxos de trabalho interpretam carimbos de data/hora locais com base no **fuso horário configurado pelo fluxo de trabalho**. Se não for especificado, o fuso horário do **servidor** será usado por padrão.

## Exemplo

| Interface | Fuso horário usado | Exemplo de exibição |
|------------|----------------|-----------------|
| Console do cliente | Do operador (padrão = servidor) | `2025-10-20 14:00:00` |
| Interface da web | Fuso horário local do navegador | `2025-10-20 21:00:00` (para navegador em UTC +7) |

Neste exemplo, ambas as interfaces fazem referência ao mesmo carimbo de data e hora UTC subjacente, mas cada uma renderiza usando um fuso horário diferente.

## Impacto

As diferenças nos tempos exibidos podem aparecer em:

* Campos de perfil ou dados contendo `datetime` valores
* Logs de entrega ou datas de contato
* Carimbos de data e hora de execução e importação do fluxo de trabalho

Os dados subjacentes permanecem idênticos. A diferença está apenas na **renderização**.

>[!NOTE]
>
>Se usuários de várias regiões colaborarem na mesma instância, podem ocorrer discrepâncias aparentes entre a interface da Web e os carimbos de data e hora do Console.

## Recomendações

Para alinhar valores de exibição em interfaces, é possível:

* Altere o **fuso horário do navegador** para corresponder ao **fuso horário do operador ou servidor**.
* Ao exportar dados (as exportações usam UTC), verifique se a conversão é consistente nas ferramentas de relatório.
* Ao criar fluxos de trabalho, defina explicitamente o **fuso horário do fluxo de trabalho** nas propriedades da atividade para um agendamento previsível e comportamento de importação.
* Comunique aos usuários empresariais que as diferenças de carimbo de data e hora entre a interface do usuário da Web e as exibições do Console do Cliente são **normais e esperadas**.
