---
title: クレジット カード番号の DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507411"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="36f57-102">クレジット カード番号に関する DLP 問題</span><span class="sxs-lookup"><span data-stu-id="36f57-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="36f57-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36f57-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="36f57-104">**クレジット カード番号に関する DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="36f57-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="36f57-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span><span class="sxs-lookup"><span data-stu-id="36f57-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="36f57-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span><span class="sxs-lookup"><span data-stu-id="36f57-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="36f57-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span><span class="sxs-lookup"><span data-stu-id="36f57-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="36f57-108">**[書式:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 書式設定あり、または書式設定なし (dddddddddddddddd) の 16 桁の数字 (Luhn テストに合格する必要あり)。</span><span class="sxs-lookup"><span data-stu-id="36f57-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="36f57-109">**[パターン:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** 世界規模の主要ブランドのカード (Visa、MasterCard、Discover Card、JCB、American Express、ギフト カード、Dinars Club Card など) を検出する非常に複雑で信頼性の高いパターンです。</span><span class="sxs-lookup"><span data-stu-id="36f57-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="36f57-110">**[チェックサム:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** あり (Luhn のチェックサム)。</span><span class="sxs-lookup"><span data-stu-id="36f57-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="36f57-111">**[定義:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。</span><span class="sxs-lookup"><span data-stu-id="36f57-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="36f57-112">関数 Func_credit_card がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="36f57-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="36f57-113">次のいずれかの条件に該当する:</span><span class="sxs-lookup"><span data-stu-id="36f57-113">One of the following is true:</span></span>

  - <span data-ttu-id="36f57-114">Keyword_cc_verification のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="36f57-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="36f57-115">Keyword_cc_name のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="36f57-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="36f57-116">関数 Func_expiration_date が適切な日付形式の日付を検出した。</span><span class="sxs-lookup"><span data-stu-id="36f57-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="36f57-117">チェックサムが渡される。</span><span class="sxs-lookup"><span data-stu-id="36f57-117">The checksum passes</span></span>

    <span data-ttu-id="36f57-118">たとえば、次の例は DLP クレジット カード番号ポリシーに対してトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="36f57-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="36f57-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="36f57-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="36f57-120">有効期限: 2/2009</span><span class="sxs-lookup"><span data-stu-id="36f57-120">Expires: 2/2009</span></span>

<span data-ttu-id="36f57-121">コンテンツに対して**クレジット カード番号**を検出するために必要なものに関する詳細については、この記事の「[What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)」(クレジット カード番号に関する機密情報の種類の検索基準) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36f57-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="36f57-122">さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」の記事でその他の種類に必要なものを参照してください。</span><span class="sxs-lookup"><span data-stu-id="36f57-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  