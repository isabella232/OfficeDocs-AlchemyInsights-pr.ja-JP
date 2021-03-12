---
title: Exchange Server の更新プログラムをインストールする場合に発生する問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9421"
ms.openlocfilehash: 04daad34d1097da0039ac63a13f793a550b68414
ms.sourcegitcommit: 13d96a612b67e01c725d5c2a5a0212d824031f6e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696548"
---
# <a name="issues-when-installing-exchange-server-updates"></a><span data-ttu-id="dae0b-102">Exchange Server の更新プログラムをインストールする場合に発生する問題</span><span class="sxs-lookup"><span data-stu-id="dae0b-102">Issues when installing Exchange Server updates</span></span>

<span data-ttu-id="dae0b-103">Exchange Server の更新プログラムをインストールする前に、「ベスト プラクティス」 セクションで「[Exchange を最新の累積的な更新プログラムにアップグレードする](https://docs.microsoft.com/Exchange/plan-and-deploy/install-cumulative-updates)」を参照します。</span><span class="sxs-lookup"><span data-stu-id="dae0b-103">Before installing Exchange Server updates, see the 'Best Practices' section of the article [Upgrade Exchange to the latest Cumulative Update](https://docs.microsoft.com/Exchange/plan-and-deploy/install-cumulative-updates).</span></span> <span data-ttu-id="dae0b-104">Microsoft Update を通じて更新プログラムをインストールしていない限り、管理者特権の CMD プロンプトを使用して更新プログラムをインストールすることが特に重要です。</span><span class="sxs-lookup"><span data-stu-id="dae0b-104">It is especially important to install updates using the elevated CMD prompt (unless updates are installed through Microsoft Update).</span></span> <span data-ttu-id="dae0b-105">これは累積的な更新プログラムとセキュリティ更新プログラムの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="dae0b-105">This applies to both Cumulative and Security updates!</span></span>

<span data-ttu-id="dae0b-106">セキュリティ更新プログラムをインストールした場合、または更新プログラムのインストール後にエラーが表示される場合は、「[トラブルシューティングによるインストールの失敗](https://aka.ms/exupdatefaq)」を参照します。</span><span class="sxs-lookup"><span data-stu-id="dae0b-106">If you see errors when installing security updates or after update was installed, see [this article about troubleshooting failed installations](https://aka.ms/exupdatefaq).</span></span>
