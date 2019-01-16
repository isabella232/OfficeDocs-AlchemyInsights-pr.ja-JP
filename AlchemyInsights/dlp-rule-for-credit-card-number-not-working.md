---
title: 動作していないクレジット カード番号の DLP ルール
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: a56f32b54e6cb32fa044d26d08868bac8c368de5
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297399"
---
<span data-ttu-id="70de6-p101">**データ損失防止 (DLP)** O365 で DLP の機密性の高い情報の種類を使用する場合は、**クレジット カード番号**を含むコンテンツの動作していない問題が発生しているでしょうか。その場合は、コンテンツには、トリガーに必要な情報が含まれていることを確認して、DLP ポリシーが評価されるときです。などの 85% の信頼レベルで構成されている**クレジット カードのポリシー** 、次は評価され、ルールをトリガーするを検出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="70de6-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="70de6-105">**[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 桁の数字書式を設定することができますが、または書式設定されていない (dddddddddddddddd) と、Luhn のテストに合格する必要があります。</span><span class="sxs-lookup"><span data-stu-id="70de6-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="70de6-106">**[パターン:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Visa、Mastercard、カードの検出、安全、アメリカン エキスプレス、ギフト カード、および給仕のカードを含め、全世界のすべての主要ブランドからカードを検出する非常に複雑で堅牢なパターンです。</span><span class="sxs-lookup"><span data-stu-id="70de6-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="70de6-107">**[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** はい、Luhn のチェックサム</span><span class="sxs-lookup"><span data-stu-id="70de6-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="70de6-108">**[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP ポリシーとは、85% をこの種類の機密情報を検出したことを確信、近くにある 300 文字以内の場合。</span><span class="sxs-lookup"><span data-stu-id="70de6-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="70de6-109">関数 Func_credit_card がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="70de6-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="70de6-110">次のいずれかの条件に該当する:</span><span class="sxs-lookup"><span data-stu-id="70de6-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="70de6-111">Keyword_cc_verification のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="70de6-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="70de6-112">Keyword_cc_name からキーワードが見つかりました</span><span class="sxs-lookup"><span data-stu-id="70de6-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="70de6-113">関数 Func_expiration_date が適切な日付形式の日付を検出した。</span><span class="sxs-lookup"><span data-stu-id="70de6-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="70de6-114">チェックサム パス</span><span class="sxs-lookup"><span data-stu-id="70de6-114">The checksum passes</span></span>
    
    <span data-ttu-id="70de6-115">たとえば、次の例を DLP のクレジット カード番号のポリシーのトリガー。</span><span class="sxs-lookup"><span data-stu-id="70de6-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="70de6-116">Visa: 4485 3647 3952 の 7352</span><span class="sxs-lookup"><span data-stu-id="70de6-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="70de6-117">有効期限: 2009 年 2 月</span><span class="sxs-lookup"><span data-stu-id="70de6-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="70de6-118">**クレジット カード番号**をコンテンツの検出に必要なものの詳細については、この資料の次のセクションを参照してください:[どのような機密性の高い情報の種類のクレジット カード番号の確認](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="70de6-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="70de6-119">組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="70de6-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

