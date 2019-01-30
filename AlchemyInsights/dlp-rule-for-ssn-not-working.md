---
title: SSN に関する DLP ルールが機能しない
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477582"
---
<span data-ttu-id="4d2d0-p101">Office 365 で機密情報の類を使用しているときに、**社会保障番号 (SSN)** を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題は発生していませんか。発生している場合は、コンテンツに DLP ポリシーに必要な情報が含まれていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365? If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4d2d0-104">たとえば、85% の信頼レベルで構成された SSN ポリシーでは、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4d2d0-105">**[書式:](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 桁の数字、書式設定されたパターンの場合もあれば、書式設定されていないパターンの場合もあります。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-105">9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="4d2d0-106">**[パターン:](https://msconnect.microsoft.com/https:/docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 次の 4 つの関数が 4 つの異なるパターンで SSN を検索します。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-106">Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="4d2d0-107">Func_ssn は、2011 年以前の厳密な書式の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="4d2d0-108">Func_unformatted_ssn は、2011 年以前の厳密な書式の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="4d2d0-109">Func_randomized_formatted_ssn は、2011 年以降の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="4d2d0-110">Func_randomized_unformatted_ssn は、2011 年以降の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="4d2d0-111">**[チェックサム:](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** いいえ、チェックサムはありません。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-111">**[Checksum:](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="4d2d0-112">**[定義:](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-112">A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="4d2d0-113">[関数 Func_ssn](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-113">The function Func_ssn finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="4d2d0-p102">[Keyword_ssn](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) から 1 つのキーワードが見つかった。キーワードの例には、*Social Security、Social Security#、Soc Sec、SSN* が含まれます。たとえば、**SSN: 489-36-8350** は DLP SSN ポリシーをトリガーします。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-p102">A keyword from [Keyword_ssn](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found. Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  . For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="4d2d0-117">コンテンツに対して SSN を検出するために必要なものに関する詳細については、この記事の「[SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4d2d0-118">さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d2d0-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/ja-JP/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

