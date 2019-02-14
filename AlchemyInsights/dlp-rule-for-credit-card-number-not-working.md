---
title: クレジット カード番号の DLP ルールが機能しない
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919085"
---
<span data-ttu-id="e3835-p101">O365 で機密情報の種類 DLP を使用しているときに、**クレジット カード番号**を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題が発生する場合があります。その場合は、評価時に DLP ポリシーをトリガーするのに必要な情報がコンテンツに含まれていることを確認してください。たとえば、85% の信頼レベルで構成されている**クレジット カード ポリシー**の場合は、ルールをトリガーするために以下が評価され、検出される必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3835-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="e3835-105">**[書式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 書式設定あり、または書式設定なし (dddddddddddddddd) の 16 桁の数字 (Luhn テストに合格する必要あり)。</span><span class="sxs-lookup"><span data-stu-id="e3835-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="e3835-106">**[パターン:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 世界規模の主要ブランドのカード (Visa、MasterCard、Discover Card、JCB、American Express、ギフト カード、Dinars Club Card など) を検出する非常に複雑で信頼性の高いパターンです。</span><span class="sxs-lookup"><span data-stu-id="e3835-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="e3835-107">**[チェックサム:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** あり (Luhn のチェックサム)。</span><span class="sxs-lookup"><span data-stu-id="e3835-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="e3835-108">**[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。</span><span class="sxs-lookup"><span data-stu-id="e3835-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="e3835-109">関数 Func_credit_card がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="e3835-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="e3835-110">次のいずれかの条件に該当する:</span><span class="sxs-lookup"><span data-stu-id="e3835-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="e3835-111">Keyword_cc_verification のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="e3835-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="e3835-112">Keyword_cc_name のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="e3835-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="e3835-113">関数 Func_expiration_date が適切な日付形式の日付を検出した。</span><span class="sxs-lookup"><span data-stu-id="e3835-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="e3835-114">チェックサムが渡される。</span><span class="sxs-lookup"><span data-stu-id="e3835-114">The checksum passes</span></span>
    
    <span data-ttu-id="e3835-115">たとえば、次の例は DLP クレジット カード番号ポリシーに対してトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="e3835-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="e3835-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="e3835-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="e3835-117">有効期限: 2/2009</span><span class="sxs-lookup"><span data-stu-id="e3835-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="e3835-118">コンテンツに対して**クレジット カード番号**を検出するために必要なものに関する詳細については、この記事の「[What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)」(クレジット カード番号に関する機密情報の種類の検索基準) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3835-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="e3835-119">さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3835-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

