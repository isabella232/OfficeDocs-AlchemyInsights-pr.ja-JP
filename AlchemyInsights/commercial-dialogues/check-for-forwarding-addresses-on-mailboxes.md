---
title: メールボックスの転送先アドレスを確認する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484171"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="8ed90-102">メールボックスの転送先アドレスを確認する</span><span class="sxs-lookup"><span data-stu-id="8ed90-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="8ed90-103">ハッカーは、ユーザーのメール メッセージを自分宛に転送することがあるので、まずメールボックスの転送アドレスと転送ルールを確認します。</span><span class="sxs-lookup"><span data-stu-id="8ed90-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="8ed90-104">次に、監査ログを確認します。</span><span class="sxs-lookup"><span data-stu-id="8ed90-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="8ed90-105">転送アドレスを確認する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="8ed90-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="8ed90-106">**[ユーザー]** > **[アクティブ ユーザー]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="8ed90-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="8ed90-107">アカウントが侵害されたユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="8ed90-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="8ed90-108">表示されるポップアップで、**[メール設定]** を展開し、**[メールの転送]** の **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8ed90-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="8ed90-109">見覚えのない転送アドレスを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ed90-109">Remove any forwarding addresses you don't recognize.</span></span>