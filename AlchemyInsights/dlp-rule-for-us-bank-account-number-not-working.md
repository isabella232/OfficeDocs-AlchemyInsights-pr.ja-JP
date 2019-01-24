---
title: 動作していない米国の銀行口座番号の DLP ルール
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476684"
---
<span data-ttu-id="f1deb-p101">**データ損失防止 (DLP)** O365 で DLP の機密性の高い情報の種類を使用する場合は、**米国の銀行口座番号**を含むコンテンツの動作していない問題が発生しているでしょうか。場合は、確認してください、コンテンツが含まれています DLP ポリシーは、探しているものが評価されるときに必要な情報にはです。</span><span class="sxs-lookup"><span data-stu-id="f1deb-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="f1deb-104">などの 85% の信頼レベルで構成されているポリシーの**米国の銀行口座番号**、次は評価され、ルールをトリガーするを検出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1deb-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="f1deb-105">**[形式:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 桁の数字</span><span class="sxs-lookup"><span data-stu-id="f1deb-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="f1deb-106">**[パターン:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 の連続した数字です。</span><span class="sxs-lookup"><span data-stu-id="f1deb-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="f1deb-107">**[チェックサム:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムがないです。</span><span class="sxs-lookup"><span data-stu-id="f1deb-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="f1deb-108">**[定義:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP ポリシーとは、75% が確実にこのような機密性の高い情報が検出されたが、近くにある 300 文字以内の場合。</span><span class="sxs-lookup"><span data-stu-id="f1deb-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="f1deb-109">正規表現 Regex_usa_bank_account_number がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="f1deb-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="f1deb-110">Keyword_usa_Bank_Account のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="f1deb-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="f1deb-111">**米国の銀行口座番号**のポリシーの次の例では、たとえば、: 当座預金口座 78344011</span><span class="sxs-lookup"><span data-stu-id="f1deb-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="f1deb-112">**米国の銀行口座番号**をコンテンツの検出に必要なものの詳細については、この資料の次のセクションを参照してください:[どのような機密性の高い情報の種類](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="f1deb-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="f1deb-113">組み込まれている機密情報を別の型を使用して [その他の種類に必要なものについては、次の資料を参照してください:[どのような機密性の高い情報の種類を探します](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f1deb-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

