---
title: ドメインまたはメール送信者に安全マークを付ける必要がありますか?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803250"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="4fb1b-102">ドメインまたはメール送信者に安全マークを付ける必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="4fb1b-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="4fb1b-103">組織がスパム、フィッシング、なりすまし攻撃にさらされる可能性があるため、**差出人セーフ リストの使用は推奨されません**。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="4fb1b-104">ただし、ビジネス要件がある場合は、**[メール フロー ルール](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** を使用することを**お勧めします**。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="4fb1b-105">私たちのガイダンスは、送信者の認証を保証します (送信ドメインがなりすましではないことを確認します)。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="4fb1b-106">**注**: スパム フィルター処理の例外により、組織がセキュリティ攻撃を受ける可能性があるため、差出人セーフ リストを使用して誤検知を管理することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="4fb1b-107">ユーザーが誤って迷惑メールまたは迷惑メールとしてマーク付けされたメッセージを受信した場合は、**[メッセージとファイルを Microsoft に報告してください](https://protection.office.com/reportsubmission)**。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="4fb1b-108">Outlook の差出人セーフ リスト、スパム対策ポリシーの許可された送信者リスト、または許可されたドメイン リストは、送信者がすべてのスパム、なりすまし、フィッシング保護、送信者認証 (SPF、DKIM、DMARC) をバイパスするため、**避ける必要があります**。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="4fb1b-109">この方法は、一時的なテストのみに最適です。</span><span class="sxs-lookup"><span data-stu-id="4fb1b-109">This method is best used for temporary testing only.</span></span>
