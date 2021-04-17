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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830038"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell のマイクロ遅延またはスロットル

Exchange Online でスクリプトとコマンドレットを実行すると、 "マイクロ遅延が適用されました" と警告または遅延が表示される場合があります。 これに関連する2つの提案は次の通りです。

- [Exchange Online v2 PowerShell モジュール](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)を使用してみることをお勧めします。これには REST API に基づくコマンドレットが含まれており、格段に高性能です。 これは、頻繁に使用される多くの Get- CMDlets に最適なソリューションになることがあります。
- まだ v2 モジュールには含まれていないコマンドレットを使用する必要がある場合は、「[Office 365 の PowerShell コマンドレットを実行している場合](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)」を参照してください。これは、Exchange Online で想定される PowerShell スロットル制限について説明します。
