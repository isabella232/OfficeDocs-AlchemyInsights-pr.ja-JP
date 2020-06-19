---
title: SSN に関する DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507375"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="9cbe9-102">社会保障番号に伴う DLP の問題</span><span class="sxs-lookup"><span data-stu-id="9cbe9-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="9cbe9-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9cbe9-104">**SSN に関する DLP の問題**</span><span class="sxs-lookup"><span data-stu-id="9cbe9-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="9cbe9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="9cbe9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="9cbe9-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span><span class="sxs-lookup"><span data-stu-id="9cbe9-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="9cbe9-107">たとえば、85% の信頼レベルで構成された SSN ポリシーでは、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9cbe9-108">**[書式:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 桁の数字、書式設定されたパターンの場合もあれば、書式設定されていないパターンの場合もあります。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="9cbe9-109">**[パターン:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 次の 4 つの関数が 4 つの異なるパターンで SSN を検索します。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="9cbe9-110">Func_ssn は、2011 年以前の厳密な書式の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="9cbe9-111">Func_unformatted_ssn は、2011 年以前の厳密な書式の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="9cbe9-112">Func_randomized_formatted_ssn は、2011 年以降の SSN を検索します。これはダッシュまたはスペース (ddd-dd-dddd または ddd dd dddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="9cbe9-113">Func_randomized_unformatted_ssn は、2011 年以降の SSN を検索します。これは 9 桁の連続した数字 (ddddddddd) の形式になっています。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="9cbe9-114">**[チェックサム:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** いいえ、チェックサムはありません。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="9cbe9-115">**[定義:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、85% の確証を持ってそれがこの種類の機密情報であると特定します。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9cbe9-116">[関数 Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="9cbe9-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span><span class="sxs-lookup"><span data-stu-id="9cbe9-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="9cbe9-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span><span class="sxs-lookup"><span data-stu-id="9cbe9-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="9cbe9-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="9cbe9-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="9cbe9-120">コンテンツに対して SSN を検出するために必要なものに関する詳細については、この記事の「[SSN に関する機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="9cbe9-121">さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」の記事でその他の種類に必要なものを参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cbe9-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  