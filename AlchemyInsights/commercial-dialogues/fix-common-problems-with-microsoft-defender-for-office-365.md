---
title: Microsoft Defender for Office365 の一般的な問題を修正する
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
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751428"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="e0b93-102">Microsoft Defender for Office365 の一般的な問題を修正する</span><span class="sxs-lookup"><span data-stu-id="e0b93-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="e0b93-103">Microsoft Defender for Office365 の一般的な問題に対するいくつかの解決策を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0b93-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="e0b93-104">**メッセージの遅延:** メッセージの配信が遅れる問題が発生している場合は、安全な添付ファイル ポリシー内で **動的配信** オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="e0b93-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="e0b93-105">詳細については、「[安全な添付ファイル ポリシー内の動的配信](https://go.microsoft.com/fwlink/?linkid=2094106)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0b93-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="e0b93-106">**誤検知または誤検知の結果を報告する:** 次のリンクを使用して Microsoft にメッセージを報告してください: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835)。</span><span class="sxs-lookup"><span data-stu-id="e0b93-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="e0b93-107">**安全なリンクの保護を有効にする:**</span><span class="sxs-lookup"><span data-stu-id="e0b93-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="e0b93-108">[Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)にログインします。</span><span class="sxs-lookup"><span data-stu-id="e0b93-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="e0b93-109">**[脅威管理]** > **[ポリシー]** > **[安全なリンク]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="e0b93-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="e0b93-110">**[特定の受信者に適用されるポリシー]** で、構成されたポリシーを開きます。</span><span class="sxs-lookup"><span data-stu-id="e0b93-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="e0b93-111">**[設定]** の下側にある **[組織内で送信されるメッセージに安全なリンクを適用する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e0b93-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
