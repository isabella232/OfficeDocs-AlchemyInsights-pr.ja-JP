---
title: US/UK パスポート番号の DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507303"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="8b235-102">DLP の問題 - US/UK パスポート番号</span><span class="sxs-lookup"><span data-stu-id="8b235-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="8b235-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b235-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8b235-104">**US/UK パスポート番号に関する DLP の問題**</span><span class="sxs-lookup"><span data-stu-id="8b235-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="8b235-105">O365 で DLP 機密情報の種類を使用するときに、**US/UK パスポート番号**を含むコンテンツに対して**データ損失防止 (DLP)** が機能しないという問題がありますか?</span><span class="sxs-lookup"><span data-stu-id="8b235-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="8b235-106">その場合、DLP ポリシーが評価されるときに DLP ポリシーが探しているものに必要な情報がコンテンツに含まれていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8b235-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="8b235-107">たとえば、75% の信頼レベルで構成された **US/UK パスポート番号**では、以下の内容が評価されるため、ルールをトリガーするためにはこれらの内容が検出される必要があります</span><span class="sxs-lookup"><span data-stu-id="8b235-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="8b235-108">**[書式:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 9 桁の数字</span><span class="sxs-lookup"><span data-stu-id="8b235-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="8b235-109">**[パターン:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 9 桁の連続する数字</span><span class="sxs-lookup"><span data-stu-id="8b235-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="8b235-110">**[チェックサム:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** いいえ、チェックサムはありません</span><span class="sxs-lookup"><span data-stu-id="8b235-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="8b235-111">**[定義:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、75% の確証を持ってそれがこの種類の機密情報であると特定します。</span><span class="sxs-lookup"><span data-stu-id="8b235-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="8b235-112">関数 Func_usa_uk_passport がパターンに一致するコンテンツを検出した。</span><span class="sxs-lookup"><span data-stu-id="8b235-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="8b235-113">Keyword_passport のキーワードを検出した。</span><span class="sxs-lookup"><span data-stu-id="8b235-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="8b235-114">たとえば、次のサンプルでは **US/UK パスポート番号**ポリシー (U.S. Passport number 123456789) をトリガーします。</span><span class="sxs-lookup"><span data-stu-id="8b235-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="8b235-115">コンテンツに対して US/UK パスポート番号が検出されるために必要な情報の詳細については、この記事の「[US/UK パスポート番号に関する機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b235-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="8b235-116">さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」の記事でその他の種類に必要なものを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b235-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  