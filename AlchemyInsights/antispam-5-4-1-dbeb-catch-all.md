---
title: AntiSpam 5.4.1 DBEB のまとめ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717366"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="17fc8-102">エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正</span><span class="sxs-lookup"><span data-stu-id="17fc8-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="17fc8-103">この問題は、Microsoft ネットワークに入る際の[バウンスバックを防ぐためにメール アドレスが有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。</span><span class="sxs-lookup"><span data-stu-id="17fc8-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="17fc8-104">以下の操作を試してください。</span><span class="sxs-lookup"><span data-stu-id="17fc8-104">Try the following:</span></span>

1. <span data-ttu-id="17fc8-105">問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。</span><span class="sxs-lookup"><span data-stu-id="17fc8-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="17fc8-106">ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。</span><span class="sxs-lookup"><span data-stu-id="17fc8-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="17fc8-107">単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。</span><span class="sxs-lookup"><span data-stu-id="17fc8-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="17fc8-108">問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="17fc8-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="17fc8-109">一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="17fc8-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="17fc8-110">さらにサポートが必要な場合には、サポート チケットを開いて、より良いサポートをご提供できるよう問題の範囲 (送信先のオブジェクト タイプを含む) を明記してください。</span><span class="sxs-lookup"><span data-stu-id="17fc8-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>