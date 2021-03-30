---
title: メールボックスの転送先アドレスを確認する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403316"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="c248a-102">メールボックスの転送先アドレスを確認する</span><span class="sxs-lookup"><span data-stu-id="c248a-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="c248a-103">ハッカーは、ユーザーのメール メッセージを自分宛に転送することがあるので、まずメールボックスの転送アドレスと転送ルールを確認します。</span><span class="sxs-lookup"><span data-stu-id="c248a-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="c248a-104">次に、監査ログを確認します。</span><span class="sxs-lookup"><span data-stu-id="c248a-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="c248a-105">転送アドレスを確認する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c248a-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="c248a-106">**[ユーザー]** > **[アクティブ ユーザー]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="c248a-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="c248a-107">アカウントが侵害されたユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="c248a-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="c248a-108">表示されるポップアップで、**[メール設定]** を展開し、**[メールの転送]** の **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c248a-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="c248a-109">見覚えのない転送アドレスを削除します。</span><span class="sxs-lookup"><span data-stu-id="c248a-109">Remove any forwarding addresses you don't recognize.</span></span>