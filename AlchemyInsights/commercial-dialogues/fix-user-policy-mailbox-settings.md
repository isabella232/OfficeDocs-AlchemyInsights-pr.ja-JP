---
title: ユーザー ポリシー/メールボックスの設定を修正する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751414"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="dc3de-102">ユーザー ポリシー/メールボックスの設定を修正する</span><span class="sxs-lookup"><span data-stu-id="dc3de-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="dc3de-103">メールボックスの迷惑メールの設定は、このメッセージに影響しました。</span><span class="sxs-lookup"><span data-stu-id="dc3de-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="dc3de-104">設定を確認するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="dc3de-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="dc3de-105">Exchange 管理シェルを起動します。</span><span class="sxs-lookup"><span data-stu-id="dc3de-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="dc3de-106">詳細については、「[Exchange 管理シェルを開く](https://go.microsoft.com/fwlink/?linkid=2101432)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc3de-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="dc3de-107">次のコマンドを実行します (ユーザーのメール アドレスを使用):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="dc3de-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="dc3de-108">送信者のメール アドレスが **TrustedSendersAndDomains** または **BlockedSendersAndDomains** の一部であるかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="dc3de-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="dc3de-109">メール アドレスがリストにある場合は、削除する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="dc3de-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="dc3de-110">詳細については、[Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc3de-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
