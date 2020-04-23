---
title: AntiSpam 5.4.1 DBEB のまとめ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707916"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="785ee-102">エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正</span><span class="sxs-lookup"><span data-stu-id="785ee-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="785ee-103">この問題は、Microsoft ネットワークへの入力時に[電子メールアドレスが有効であるかどうか](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)を確認するために、bouncebacks を確認するときに発生します。</span><span class="sxs-lookup"><span data-stu-id="785ee-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="785ee-104">以下の操作を試してください。</span><span class="sxs-lookup"><span data-stu-id="785ee-104">Try the following:</span></span>

1. <span data-ttu-id="785ee-105">問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。</span><span class="sxs-lookup"><span data-stu-id="785ee-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="785ee-106">ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。</span><span class="sxs-lookup"><span data-stu-id="785ee-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="785ee-107">単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。</span><span class="sxs-lookup"><span data-stu-id="785ee-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="785ee-108">問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="785ee-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="785ee-109">一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="785ee-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="785ee-110">追加のヘルプが必要な場合は、サポートチケットを開いて、問題の範囲 (送信元のオブジェクトの種類を含む) を指定してください。これにより、より良いお手伝いができます。</span><span class="sxs-lookup"><span data-stu-id="785ee-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>