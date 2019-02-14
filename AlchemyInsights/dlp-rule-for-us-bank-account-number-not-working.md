---
title: 米国の銀行口座番号の DLP ルールが機能しない場合
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916421"
---
<span data-ttu-id="84c26-p101">Office 365 で DLP 機密情報の種類を使用しているときに、**米国の銀行口座番号**を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題が発生した場合は、DLP ポリシーに必要な情報がコンテンツに含まれていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="84c26-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="84c26-104">たとえば、85% の信頼レベルで構成された**米国の銀行口座番号**では、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。</span><span class="sxs-lookup"><span data-stu-id="84c26-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="84c26-105">**[書式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 ～ 17 桁の数字</span><span class="sxs-lookup"><span data-stu-id="84c26-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="84c26-106">**[パターン:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 ～ 17 桁の連続する数字。</span><span class="sxs-lookup"><span data-stu-id="84c26-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="84c26-107">**[チェックサム:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムはありません。</span><span class="sxs-lookup"><span data-stu-id="84c26-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="84c26-108">**[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、75% の確証を持ってそれがこの種類の機密情報であると特定します。</span><span class="sxs-lookup"><span data-stu-id="84c26-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="84c26-109">正規表現 Regex_usa_bank_account_number がパターンに一致するコンテンツを検出した</span><span class="sxs-lookup"><span data-stu-id="84c26-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="84c26-110">Keyword_usa_Bank_Account のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="84c26-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="84c26-111">たとえば、次の当座預金口座 78344011 では、**米国の銀行口座番号** のポリシーがトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="84c26-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="84c26-112">コンテンツに対して**米国の銀行口座番号**が検出されるために必要な情報の詳細については、この記事の「[米国の銀行口座番号 SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84c26-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="84c26-113">さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。</span><span class="sxs-lookup"><span data-stu-id="84c26-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

