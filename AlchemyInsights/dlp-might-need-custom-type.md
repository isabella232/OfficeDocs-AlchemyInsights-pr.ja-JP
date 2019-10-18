---
title: DLP のカスタム タイプの必要性
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530356"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="c865f-102">DLP のカスタム タイプの必要性</span><span class="sxs-lookup"><span data-stu-id="c865f-102">DLP might need a custom type</span></span>

<span data-ttu-id="c865f-103">データ損失防止（DLP）ポリシーを使用すると、組織内の機密データを識別し保護することができます。</span><span class="sxs-lookup"><span data-stu-id="c865f-103">With a data loss prevention (DLP) policy, you can identify, monitor, and protect sensitive information across Office 365.</span></span> <span data-ttu-id="c865f-104">場合によっては、組織のデータを保護するために独自の**カスタム**機密情報の種類を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c865f-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="c865f-105">たとえば、組織では、固有の形式で従業員 ID やその他のデータを識別して保護する必要があることがあります。もしそうであれば、詳細について以下の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c865f-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="c865f-106">**組み込みの機密情報の種類をカスタマイズする**</span><span class="sxs-lookup"><span data-stu-id="c865f-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="c865f-107">組み込みの機密情報の種類がほんの数回の調整でニーズを満たすとすれば、[組み込みの機密情報の種類はカスタマイズできます](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="c865f-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="c865f-108">たとえば、キーワードを追加または削除したり、日付や住所などの裏付けとなる証拠を追加または削除したりできます。</span><span class="sxs-lookup"><span data-stu-id="c865f-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="c865f-109">**カスタムの機密情報の種類を作成する**</span><span class="sxs-lookup"><span data-stu-id="c865f-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="c865f-110">ですが、異なる種類の機密情報をすべて識別して保護する必要がある場合は、セキュリティ ＆ コンプライアンス センターの UI で[カスタムの機密情報の種類](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)を作成できます。</span><span class="sxs-lookup"><span data-stu-id="c865f-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="c865f-111">**セキュリティ ＆ コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成する**</span><span class="sxs-lookup"><span data-stu-id="c865f-111">See **Create a custom sensitive information type in Security & Compliance Center PowerShell**.</span></span>

<span data-ttu-id="c865f-112">最後に、UI が必要なオプションをすべて提供していない場合は、[ セキュリティ ＆ コンプライアンス センター PowerShell でカスタムの機密情報の種類を作成](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)できます。</span><span class="sxs-lookup"><span data-stu-id="c865f-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="c865f-113">XML ファイルを使って始めると、利用可能なすべてのオプションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="c865f-113">By starting with an XML file, you can use every option available.</span></span>
