---
title: テナント ポリシーを修正 (アクションの上書き)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751293"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="1aaba-102">テナント ポリシーを修正 (アクションの上書き)</span><span class="sxs-lookup"><span data-stu-id="1aaba-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="1aaba-103">テナントの迷惑メール対策ポリシーがこのメッセージに影響を与えました。</span><span class="sxs-lookup"><span data-stu-id="1aaba-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="1aaba-104">ポリシーを確認するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="1aaba-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="1aaba-105">[Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動し、**[脅威の管理]** > **[ポリシー]** > [[スパム対策]](https://go.microsoft.com/fwlink/?linkid=2101518) の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="1aaba-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="1aaba-106">**ポリシー ソース** で以下が表示されているかどうかを確認します:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span><span class="sxs-lookup"><span data-stu-id="1aaba-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="1aaba-107">その場合は、**[カスタム]** で、メッセージに影響を与えたポリシーの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="1aaba-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="1aaba-108">すべての Exchange Online Protection のユーザーに適用された **標準設定** によってメッセージが影響された可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1aaba-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="1aaba-109">迷惑メール フィルター ポリシーの構成の詳細については、「[迷惑メール フィルター ポリシーを構成する](https://go.microsoft.com/fwlink/?linkid=2101431)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1aaba-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
