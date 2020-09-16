---
title: アカウントが侵害された場合に推奨される対処方法
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "957"
- "3100016"
ms.openlocfilehash: acce676ebb9f4000794669ffb268e7b4fe057f77
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771285"
---
# <a name="recommended-steps-to-take-if-an-account-is-compromised"></a><span data-ttu-id="9cb2c-102">アカウントが侵害された場合に推奨される対処方法</span><span class="sxs-lookup"><span data-stu-id="9cb2c-102">Recommended steps to take if an account is compromised</span></span>

[<span data-ttu-id="9cb2c-103">ビデオ: 侵害されたアカウントの修復</span><span class="sxs-lookup"><span data-stu-id="9cb2c-103">VIDEO: Fixing a compromised account</span></span>](https://www.microsoft.com/videoplayer/embed/RE2jvOb?pid=ocpVideo0-innerdiv-oneplayer&amp;postJsllMsg=true&amp;maskLevel=20&amp;autoplay=true)
  
1. <span data-ttu-id="9cb2c-p101">[ユーザーのパスワードを直ちにリセット](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords)します。新しいパスワードはメールでエンド ユーザーに伝えないでください。</span><span class="sxs-lookup"><span data-stu-id="9cb2c-p101">[Reset the user's password](https://docs.microsoft.com/microsoft-365/admin/add-users/reset-passwords) immediately. Do not communicate the new password through email to the end user.</span></span>

2. <span data-ttu-id="9cb2c-106">メールボックス レベルで設定される疑わしい[転送アドレス](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)をすべて削除します。</span><span class="sxs-lookup"><span data-stu-id="9cb2c-106">Remove any suspicious [forwarding addresses](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding) set at the mailbox level.</span></span>

3. <span data-ttu-id="9cb2c-107">メールボックス内に設定されている[受信トレイのルー](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED)を削除します。</span><span class="sxs-lookup"><span data-stu-id="9cb2c-107">Remove any suspicious [inbox rules](https://support.office.com/article/1433E3A0-7FB0-4999-B536-50E05CB67FED) set within the mailbox.</span></span>

4. <span data-ttu-id="9cb2c-p102">ユーザーがメールの送信をブロックされている場合は、[[制限されたユーザー] ページに移動してアカウントのブロックを解除](https://protection.office.com/?hash=/restrictedusers) します。この操作を完了すると、1 時間以内にメッセージの送信を再開できるようになります。</span><span class="sxs-lookup"><span data-stu-id="9cb2c-p102">If the user is blocked from sending email, [go to the Restricted Users page to unblock the account](https://protection.office.com/?hash=/restrictedusers). Once done, the user should be able to resume sending messages within 1 hour.</span></span>

5. <span data-ttu-id="9cb2c-110">アカウントが侵害されていないと確信できるまでは、すべての[管理ロール グループ](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles)からそのユーザー アカウントを削除します。</span><span class="sxs-lookup"><span data-stu-id="9cb2c-110">Remove the user account from any [administrative role groups](https://docs.microsoft.com/microsoft-365/admin/add-users/assign-admin-roles) until you are confident that the account is no longer compromised.</span></span>

<span data-ttu-id="9cb2c-111">将来のデータ漏えいやアカウントの侵害の可能性を最小限に抑えるために、[Microsoft 365 のセキュリティのロードマップ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap)を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9cb2c-111">To minimize the potential of a data breach or a compromised account in the future, we recommend reading our [Microsoft 365 security roadmap ](https://docs.microsoft.com//office365/securitycompliance/security-roadmap).</span></span>
  