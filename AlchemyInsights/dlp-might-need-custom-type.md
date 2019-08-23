---
title: DLP にカスタムの種類が必要な場合があります
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 612b6652b445914063ac825847f5698d3afc3a00
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530356"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="870c9-102">DLP にカスタムの種類が必要な場合があります</span><span class="sxs-lookup"><span data-stu-id="870c9-102">DLP might need a custom type</span></span>

<span data-ttu-id="870c9-103">データ損失防止 (DLP) ポリシーを使用すると、組織内の機密データを識別して保護することができます。</span><span class="sxs-lookup"><span data-stu-id="870c9-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="870c9-104">シナリオによっては、組織のデータを保護するために、独自の**カスタム**の機密情報の種類を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="870c9-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="870c9-105">たとえば、組織では、組織に固有の形式で従業員 Id またはその他のデータを識別して保護する必要がある場合があります。その場合、詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="870c9-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="870c9-106">**組み込みの機密情報の種類をカスタマイズする**</span><span class="sxs-lookup"><span data-stu-id="870c9-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="870c9-107">組み込みの機密情報の種類がいくつかの微調整でニーズを満たす場合は、[組み込みの機密情報の種類をカスタマイズ](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)できます。</span><span class="sxs-lookup"><span data-stu-id="870c9-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="870c9-108">たとえば、キーワードを追加または削除したり、日付やアドレスなどのサポートの証拠を追加または削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="870c9-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="870c9-109">**カスタムの機密情報の種類を作成する**</span><span class="sxs-lookup"><span data-stu-id="870c9-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="870c9-110">ただし、さまざまな種類の機密情報を識別して保護する必要がある場合は、セキュリティ & コンプライアンスセンターの UI で[カスタムの機密情報の種類を作成](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)することができます。</span><span class="sxs-lookup"><span data-stu-id="870c9-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="870c9-111">**セキュリティ & コンプライアンスセンターの PowerShell でカスタムの機密情報の種類を作成する**</span><span class="sxs-lookup"><span data-stu-id="870c9-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="870c9-112">最後に、UI が必要なすべてのオプションを提供していない場合は、[セキュリティ & コンプライアンスセンターの PowerShell でカスタムの機密情報の種類を作成](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)できます。</span><span class="sxs-lookup"><span data-stu-id="870c9-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="870c9-113">XML ファイルでは、使用可能なすべてのオプションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="870c9-113">By starting with an XML file, you can use every option available.</span></span>
