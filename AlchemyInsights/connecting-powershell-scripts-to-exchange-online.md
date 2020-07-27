---
title: PowerShell スクリプトを Exchange Online に接続する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 34301e62a25e11c5d4c353166f8208ef74245dfa
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/22/2020
ms.locfileid: "45424291"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="7b9ac-102">PowerShell スクリプトを Exchange Online に接続する</span><span class="sxs-lookup"><span data-stu-id="7b9ac-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="7b9ac-103">Exchange Online の基本認証は廃止されます。今後の方法は、スクリプトおよび無人タスクに証明書ベースの認証を使用して接続することです。</span><span class="sxs-lookup"><span data-stu-id="7b9ac-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="7b9ac-104">詳細については、[「EXO V2 モジュールの無人スクリプトのアプリ専用の認証」](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b9ac-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>