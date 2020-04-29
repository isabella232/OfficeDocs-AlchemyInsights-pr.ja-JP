---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 8b5f22269cab0ed0984bcb33703b49e943ef2446
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642257"
---
# <a name="irm-protection-to-sharepoint-files"></a><span data-ttu-id="ab5ab-102">SharePoint ファイルに対する IRM 保護</span><span class="sxs-lookup"><span data-stu-id="ab5ab-102">IRM Protection to SharePoint files</span></span>


<span data-ttu-id="ab5ab-103">SharePoint Online では、リストおよびライブラリのレベルでファイルに IRM 保護が適用されます。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-103">Within SharePoint Online, IRM protection is applied to files at the list and library level.</span></span> <span data-ttu-id="ab5ab-104">組織で IRM 保護を使用するには、まず、Rights Management をセットアップしておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-104">Before your organization can use IRM protection, you must first set up Rights Management.</span></span> <span data-ttu-id="ab5ab-105">IRM は Azure Information Protection の Azure Rights Management サービスを利用して、暗号化と使用制限の割り当てを実施します。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-105">IRM relies on the Azure Rights Management service from Azure Information Protection to encrypt and assign usage restrictions.</span></span> <span data-ttu-id="ab5ab-106">Microsoft 365 サブスクリプションには Azure Rights Management が含まれているものと、含まれていないものがあります。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-106">Some Microsoft 365 subscriptions include Azure Rights Management, but not all.</span></span> 

<span data-ttu-id="ab5ab-107">詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-107">To learn more, see:</span></span>

- <span data-ttu-id="ab5ab-108">[Office のアプリケーションとサービスが Azure Rights Management をサポートするしくみ](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support)。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-108">[How Office applications and services support Azure Rights Management](https://docs.microsoft.com/azure/information-protection/understand-explore/office-apps-services-support).</span></span>

- <span data-ttu-id="ab5ab-109">[SharePoint 管理センターで Information Rights Management (IRM) を設定する](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center)。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-109">[Set up Information Rights Management (IRM) in SharePoint admin center](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center).</span></span>

- <span data-ttu-id="ab5ab-110">[IRM 対応の SharePoint ドキュメント ライブラリとリスト](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists)。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-110">[IRM-enable SharePoint document libraries and lists](https://docs.microsoft.com/office365/securitycompliance/set-up-irm-in-sp-admin-center#irm-enable-sharepoint-document-libraries-and-lists).</span></span>

- <span data-ttu-id="ab5ab-111">[Office の Information Rights Management](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c)。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-111">[Information Rights Management in Office](https://support.office.com/Article/Information-Rights-Management-in-Office-c7a70797-6b1e-493f-acf7-92a39b85e30c).</span></span>

- <span data-ttu-id="ab5ab-112">[Exchange Online での Information Rights Management](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online)。</span><span class="sxs-lookup"><span data-stu-id="ab5ab-112">[Information Rights Management in Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/information-rights-management-in-exchange-online).</span></span>


