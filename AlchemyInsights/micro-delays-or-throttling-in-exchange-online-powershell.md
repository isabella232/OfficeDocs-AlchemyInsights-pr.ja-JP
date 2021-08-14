---
title: Exchange Online PowerShell のマイクロ遅延またはスロットル
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868539"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell のマイクロ遅延またはスロットル

Exchange Online でスクリプトとコマンドレットを実行すると、 "マイクロ遅延が適用されました" と警告または遅延が表示される場合があります。 これを解決する方法をいくつか提案します。

- 診断を実行して、テナントの PowerShell スロットル ポリシーを緩和してください。 このソリューションは、ほとんどの問題を解決します。
- それでも問題が解決しない場合は、[Exchange Online v2 PowerShell モジュール](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)を使用してください。これには REST API に基づくコマンドレットが含まれており、格段に高性能です。 これは、頻繁に使用される多くの Get- CMDlets に最適なソリューションになることがあります。
- v2 モジュールには含まれていないコマンドレットを使用する必要がある場合は、「[Office 365 で多数のユーザー向けに PowerShell コマンドレットを実行する](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)」を参照してください。これは、Exchange Online の PowerShell スロットル制限を回避する方法について説明しています。
