---
title: スパム対策 5.4.1 DBEB キャッチオール
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
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2019
ms.locfileid: "37973184"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="29c8e-102">エラーコード 550 5.4.1 Relay アクセスが拒否された場合の配信に関する問題の修正</span><span class="sxs-lookup"><span data-stu-id="29c8e-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="29c8e-103">この問題は、Office 365 ネットワークへの入力時に[電子メールアドレスが有効であるかどうかを確認するために、bouncebacks が有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。</span><span class="sxs-lookup"><span data-stu-id="29c8e-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="29c8e-104">次の方法を試します。</span><span class="sxs-lookup"><span data-stu-id="29c8e-104">Try the following:</span></span>

1. <span data-ttu-id="29c8e-105">問題がドメイン全体に特有なものか、単一の電子メールアドレスであるかを判別します。</span><span class="sxs-lookup"><span data-stu-id="29c8e-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="29c8e-106">ドメイン全体: ドメインを同期する必要がある場合があります。[ドメインを内部に設定してから、権限のあるものに戻し](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)てください。</span><span class="sxs-lookup"><span data-stu-id="29c8e-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="29c8e-107">単一の電子メールアドレス: 場合によっては、アドレスを同期する必要があります。smtp プロキシアドレスを変更した後、それを再度変更することができます。</span><span class="sxs-lookup"><span data-stu-id="29c8e-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="29c8e-108">問題がグループまたはパブリックフォルダーに固有かどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="29c8e-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="29c8e-109">オブジェクトの種類によっては、Azure Active Directory にオブジェクトを手動で作成する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="29c8e-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="29c8e-110">追加のヘルプが必要な場合は、サポートチケットを開いて、問題の範囲 (「送信するオブジェクトの種類」) を指定してください。これにより、より良いお手伝いができます。</span><span class="sxs-lookup"><span data-stu-id="29c8e-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>