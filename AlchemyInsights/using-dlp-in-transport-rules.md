---
title: トランスポート ルールで DLP を使用する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2020
ms.locfileid: "43918429"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="f3d34-102">トランスポート ルールで DLP を使用する</span><span class="sxs-lookup"><span data-stu-id="f3d34-102">Using DLP in transport rules</span></span>

<span data-ttu-id="f3d34-103">データ損失防止 (DLP) を既存のトランスポートに統合するには、トランスポート ルールの設定で "**If the message contains...Sensitive Information**" (メッセージに...機密情報が含まれる場合) の条件を使用します。</span><span class="sxs-lookup"><span data-stu-id="f3d34-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="f3d34-104">**詳細については、次を参照してください。**</span><span class="sxs-lookup"><span data-stu-id="f3d34-104">**For more details, see:**</span></span>

- <span data-ttu-id="f3d34-105">トランスポート ルールでの統合された DLP 機密情報の種類: [機密情報ルールを統合する](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。</span><span class="sxs-lookup"><span data-stu-id="f3d34-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="f3d34-106">このルールでテスト モードを使用して、ポリシー テストあり、またはポリシー テストなしで、ルールをテストすることもできます。</span><span class="sxs-lookup"><span data-stu-id="f3d34-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="f3d34-107">ルールを作成してからテストするまで、30 分待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3d34-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="f3d34-108">「[メール フロー/トランスポート ルールをテストする](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3d34-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="f3d34-109">**注**: トランスポート ルールを使用して新しい DLP ポリシーを EAC に実装する場合は、代わりに、[セキュリティ/コンプライアンスセンターで DLP ポリシー](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)を使用します。</span><span class="sxs-lookup"><span data-stu-id="f3d34-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
