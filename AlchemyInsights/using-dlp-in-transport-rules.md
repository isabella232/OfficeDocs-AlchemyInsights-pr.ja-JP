---
title: トランスポート ルールで DLP を使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827221"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="35629-102">トランスポート ルールで DLP を使用する</span><span class="sxs-lookup"><span data-stu-id="35629-102">Using DLP in transport rules</span></span>

<span data-ttu-id="35629-103">データ損失防止 (DLP) を既存のトランスポートに統合するには、トランスポート ルールの設定で "**If the message contains...Sensitive Information**" (メッセージに...機密情報が含まれる場合) の条件を使用します。</span><span class="sxs-lookup"><span data-stu-id="35629-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="35629-104">**詳細については、次を参照してください。**</span><span class="sxs-lookup"><span data-stu-id="35629-104">**For more details, see:**</span></span>

- <span data-ttu-id="35629-105">トランスポート ルールでの統合された DLP 機密情報の種類: [機密情報ルールを統合する](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。</span><span class="sxs-lookup"><span data-stu-id="35629-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="35629-106">このルールでテスト モードを使用して、ポリシー テストあり、またはポリシー テストなしで、ルールをテストすることもできます。</span><span class="sxs-lookup"><span data-stu-id="35629-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="35629-107">ルールを作成してからテストするまで、30 分待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="35629-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="35629-108">「[メール フロー/トランスポート ルールをテストする](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35629-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="35629-109">**注**: トランスポート ルールを使用して新しい DLP ポリシーを EAC に実装する場合は、代わりに、[セキュリティ/コンプライアンスセンターで DLP ポリシー](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)を使用します。</span><span class="sxs-lookup"><span data-stu-id="35629-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
