---
title: AntiSpam 5.4.1 DBEB のまとめ
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
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821452"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="94578-102">エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正</span><span class="sxs-lookup"><span data-stu-id="94578-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="94578-103">この問題は、Microsoft ネットワークに入る際の[バウンスバックを防ぐためにメール アドレスが有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。</span><span class="sxs-lookup"><span data-stu-id="94578-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="94578-104">以下の操作を試してください。</span><span class="sxs-lookup"><span data-stu-id="94578-104">Try the following:</span></span>

1. <span data-ttu-id="94578-105">問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。</span><span class="sxs-lookup"><span data-stu-id="94578-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="94578-106">ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。</span><span class="sxs-lookup"><span data-stu-id="94578-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="94578-107">単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。</span><span class="sxs-lookup"><span data-stu-id="94578-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="94578-108">問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="94578-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="94578-109">一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="94578-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="94578-110">さらにサポートが必要な場合には、サポート チケットを開いて、より良いサポートをご提供できるよう問題の範囲 (送信先のオブジェクト タイプを含む) を明記してください。</span><span class="sxs-lookup"><span data-stu-id="94578-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>