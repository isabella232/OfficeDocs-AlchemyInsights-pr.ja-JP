---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b1ec30a55ec0c08b291228ee90771bc56a55a36d
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751749"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="0de76-102">SharePoint ファイルへの IRM による保護</span><span class="sxs-lookup"><span data-stu-id="0de76-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="0de76-103">SharePoint Online では、IRM 保護はリストおよびライブラリレベルでファイルに適用されます。</span><span class="sxs-lookup"><span data-stu-id="0de76-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="0de76-104">組織で IRM 保護を使用するには、最初に Rights Management を設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0de76-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="0de76-105">IRM は azure Information Protection からの Azure Rights Management サービスに依存して、使用制限を暗号化して割り当てます。</span><span class="sxs-lookup"><span data-stu-id="0de76-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="0de76-106">一部の Office 365 プランには、Azure Rights Management は含まれていますが、すべてではありません。</span><span class="sxs-lookup"><span data-stu-id="0de76-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="0de76-107">詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0de76-107">To learn more, see:</span></span>

- <span data-ttu-id="0de76-108">[Office アプリケーションとサービスがどのように Azure Rights Management をサポートしているか](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)。</span><span class="sxs-lookup"><span data-stu-id="0de76-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="0de76-109">[SharePoint 管理センターで Information Rights Management (IRM) を設定](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)します。</span><span class="sxs-lookup"><span data-stu-id="0de76-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="0de76-110">[IRM-SharePoint ドキュメントライブラリとリストを有効に](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)します。</span><span class="sxs-lookup"><span data-stu-id="0de76-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="0de76-111">[Office の Information Rights Management](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)。</span><span class="sxs-lookup"><span data-stu-id="0de76-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="0de76-112">[Exchange Online での Information Rights Management](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="0de76-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


