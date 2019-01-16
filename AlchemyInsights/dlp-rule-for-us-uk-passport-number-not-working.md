---
title: 米国の DLP ルールと動作していない、英国パスポート番号
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298295"
---
<span data-ttu-id="ae578-p101">**データ損失防止 (DLP)** のコンテンツが含まれているために動作していない問題が発生している、**米国と英国のパスポート番号**O365 で DLP の機密性の高い情報の種類を使用する場合でしょうか。場合は、確認してください、コンテンツが含まれています DLP ポリシーは、探しているものが評価されるときに必要な情報にはです。</span><span class="sxs-lookup"><span data-stu-id="ae578-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="ae578-104">などの**米国と英国のパスポート番号**の 75% の信頼レベルで構成されているポリシーは、次は評価され、ルールをトリガーするを検出する必要があります</span><span class="sxs-lookup"><span data-stu-id="ae578-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="ae578-105">**[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 桁</span><span class="sxs-lookup"><span data-stu-id="ae578-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="ae578-106">**[パターン:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 9 つの連続した数字</span><span class="sxs-lookup"><span data-stu-id="ae578-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="ae578-107">**[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムがないです。</span><span class="sxs-lookup"><span data-stu-id="ae578-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="ae578-108">**[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP ポリシーとは、75% が確実にこのような機密性の高い情報が検出されたが、近くにある 300 文字以内の場合。</span><span class="sxs-lookup"><span data-stu-id="ae578-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="ae578-109">関数 Func_usa_uk_passport がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="ae578-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="ae578-110">Keyword_passport のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="ae578-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="ae578-111">次の例では、たとえば、**米国と英国のパスポート番号**ポリシー: u. s. パスポート番号 123456789</span><span class="sxs-lookup"><span data-stu-id="ae578-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="ae578-112">米国に必要なものの詳細については、コンテンツのために認識されるようにイギリスのパスポート番号は、この資料の次のセクションを参照してください/:[ではどのような機密性の高い情報の種類の外観と英国のパスポート番号](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="ae578-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="ae578-113">組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ae578-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

