---
title: 同期の問題のまとめ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000037"
- "1674"
- "9000241"
- "1951"
ms.openlocfilehash: 681bdc16efac19c4b8ea0b91b13aa38cd4e9007c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819409"
---
# <a name="basic-outlook-sync-troubleshooting"></a><span data-ttu-id="c27a5-102">基本的な Outlook 同期のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="c27a5-102">Basic Outlook sync troubleshooting</span></span>

<span data-ttu-id="c27a5-103">同期の問題がある場合には、以下を試してください。</span><span class="sxs-lookup"><span data-stu-id="c27a5-103">If you're having sync issues, try the following:</span></span>

- <span data-ttu-id="c27a5-104">影響を受けるマシンで[この診断ツール](https://aka.ms/sara-outlooksendreceive)を実行します。</span><span class="sxs-lookup"><span data-stu-id="c27a5-104">Run [this diagnostic tool](https://aka.ms/sara-outlooksendreceive) on the affected machine.</span></span>
- <span data-ttu-id="c27a5-105">プライマリまたは共有メールボックスのフォルダー数を減らします。</span><span class="sxs-lookup"><span data-stu-id="c27a5-105">Reduce the number of folders in the primary or shared mailbox.</span></span> <span data-ttu-id="c27a5-106">「[キャッシュ モードの .ost ファイルまたは .pst ファイルのフォルダー内の項目が多すぎるフォルダーがある場合、Outlook のパフォーマンスの問題が発生する](https://support.microsoft.com/help/2768656/outlook-performance-issues-when-there-are-too-many-items-or-folders-in)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c27a5-106">See [Outlook performance issues when there are too many items or folders in a Cached mode .ost or .pst file folder](https://support.microsoft.com/help/2768656/outlook-performance-issues-when-there-are-too-many-items-or-folders-in).</span></span>
- <span data-ttu-id="c27a5-107">すべての共有フォルダーのキャッシュを無効にします。</span><span class="sxs-lookup"><span data-stu-id="c27a5-107">Disable caching of all shared folders.</span></span>
- <span data-ttu-id="c27a5-108">プロファイルでセカンダリ Exchange メールボックスの構成を2つ目の Exchange アカウントに変更します。</span><span class="sxs-lookup"><span data-stu-id="c27a5-108">Change the configuration of the secondary Exchange mailbox to a second Exchange account in your profile.</span></span>
- <span data-ttu-id="c27a5-109">ユーザーがインターネットに接続できることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c27a5-109">Make sure the user can connect to the Internet.</span></span> 
- <span data-ttu-id="c27a5-110">[自身がオンラインであることを確認します](https://support.office.com/article/2460e4a8-16c7-47fc-b204-b1549275aac9)。</span><span class="sxs-lookup"><span data-stu-id="c27a5-110">[Verify that you are online](https://support.office.com/article/2460e4a8-16c7-47fc-b204-b1549275aac9).</span></span>
- <span data-ttu-id="c27a5-111">[ルールが適用されているかどうかを判断します](https://support.office.com/article/C24F5DEA-9465-4DF4-AD17-A50704D66C59)。</span><span class="sxs-lookup"><span data-stu-id="c27a5-111">[Determine whether a rule is applied](https://support.office.com/article/C24F5DEA-9465-4DF4-AD17-A50704D66C59).</span></span>
- <span data-ttu-id="c27a5-112">[**共有フォルダーのダウンロード**]が有効になっていることを、[**ファイル**] >  [**アカウント設定**] >  [**アカウント設定**] >  [**詳細設定**] >  [**詳細設定**] の順に移動して確認します。</span><span class="sxs-lookup"><span data-stu-id="c27a5-112">Verify that **Download Shared Folders** is enabled by going to **File** > **Account Settings** > **Account Settings** > **More Settings** > **Advanced**.</span></span>
