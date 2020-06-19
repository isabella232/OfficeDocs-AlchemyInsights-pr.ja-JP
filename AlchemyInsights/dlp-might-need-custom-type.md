---
title: DLP のカスタム タイプの必要性
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507519"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="488b0-102">DLP のカスタム タイプの必要性</span><span class="sxs-lookup"><span data-stu-id="488b0-102">DLP might need a custom type</span></span>

<span data-ttu-id="488b0-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="488b0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="488b0-104">**DLP にはカスタム情報の種類が必要な場合があります**</span><span class="sxs-lookup"><span data-stu-id="488b0-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="488b0-105">データ損失防止（DLP）ポリシーを使用すると、組織内の機密データを識別し保護することができます。</span><span class="sxs-lookup"><span data-stu-id="488b0-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="488b0-106">場合によっては、組織のデータを保護するために独自の**カスタム**機密情報の種類を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="488b0-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="488b0-107">たとえば、組織では、固有の形式で従業員 ID やその他のデータを識別して保護する必要があることがあります。もしそうであれば、詳細について以下の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="488b0-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="488b0-108">**組み込みの機密情報の種類をカスタマイズする**</span><span class="sxs-lookup"><span data-stu-id="488b0-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="488b0-109">組み込みの機密情報の種類がほんの数回の調整でニーズを満たすとすれば、[組み込みの機密情報の種類はカスタマイズできます](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="488b0-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="488b0-110">たとえば、キーワードを追加または削除したり、日付や住所などの裏付けとなる証拠を追加または削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="488b0-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="488b0-111">**カスタムの機密情報の種類を作成する**</span><span class="sxs-lookup"><span data-stu-id="488b0-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="488b0-112">ですが、異なる種類の機密情報をすべて識別して保護する必要がある場合は、セキュリティ ＆ コンプライアンス センターの UI で[カスタムの機密情報の種類](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)を作成できます。</span><span class="sxs-lookup"><span data-stu-id="488b0-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="488b0-113">**セキュリティ ＆ コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成する**</span><span class="sxs-lookup"><span data-stu-id="488b0-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="488b0-114">最後に、UI が必要なオプションをすべて提供していない場合は、[ セキュリティ ＆ コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)できます。</span><span class="sxs-lookup"><span data-stu-id="488b0-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="488b0-115">XML ファイルを使って始めると、利用可能なすべてのオプションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="488b0-115">By starting with an XML file, you can use every option available.</span></span>
