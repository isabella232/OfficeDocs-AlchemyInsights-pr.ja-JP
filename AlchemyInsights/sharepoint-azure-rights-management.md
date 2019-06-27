---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 126cfa4e44b3b7e900e47de0b86602c60f3f0dc2
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223897"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="32b6c-102">SharePoint ファイルに対する IRM 保護</span><span class="sxs-lookup"><span data-stu-id="32b6c-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="32b6c-103">SharePoint Online では、リストおよびライブラリのレベルでファイルに IRM 保護が適用されます。</span><span class="sxs-lookup"><span data-stu-id="32b6c-103">IRM protection is applied to files at the SharePoint list and library levels.</span></span> <span data-ttu-id="32b6c-104">組織で IRM 保護を使用するには、まず、Rights Management をセットアップしておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="32b6c-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="32b6c-105">IRM は Azure Information Protection の Azure Rights Management サービスを利用して、暗号化と使用制限の割り当てを実施します。</span><span class="sxs-lookup"><span data-stu-id="32b6c-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="32b6c-106">Office 365 のプランには Azure Rights Management が含まれているものと、含まれていないものがあります。</span><span class="sxs-lookup"><span data-stu-id="32b6c-106">Some Office 365 plans include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="32b6c-107">詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32b6c-107">To learn more, see:</span></span>

- <span data-ttu-id="32b6c-108">[Office のアプリケーションとサービスが Azure Rights Management をサポートするしくみ](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)。</span><span class="sxs-lookup"><span data-stu-id="32b6c-108">For detailed information about how OneDrive handles IRM, see [How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="32b6c-109">[SharePoint 管理センターで Information Rights Management (IRM) を設定する](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="32b6c-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)</span></span>

- <span data-ttu-id="32b6c-110">[IRM 対応の SharePoint ドキュメント ライブラリとリスト](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)。</span><span class="sxs-lookup"><span data-stu-id="32b6c-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="32b6c-111">[Office の Information Rights Management](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)。</span><span class="sxs-lookup"><span data-stu-id="32b6c-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)</span></span>

- <span data-ttu-id="32b6c-112">[Exchange Online での Information Rights Management](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="32b6c-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)</span></span>


