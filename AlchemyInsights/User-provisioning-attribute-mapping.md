---
title: ユーザー プロビジョニングの属性マッピング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/22/2021
ms.locfileid: "49950155"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="8f388-102">ユーザー プロビジョニングの属性マッピング</span><span class="sxs-lookup"><span data-stu-id="8f388-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="8f388-103">既知の属性マッピングの問題のトラブルシューティングについては、「[属性マッピング](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f388-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="8f388-104">Microsoft Azure Active Directory (AD) は、Salesforce、G Suite などのサードパーティ製 SaaS アプリケーションへのユーザー プロビジョニングをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8f388-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="8f388-105">サードパーティ製 SaaS アプリケーションのユーザー プロビジョニングを有効にすると、Azure portal は属性マッピングを介してその属性値を制御します。</span><span class="sxs-lookup"><span data-stu-id="8f388-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="8f388-106">既定の属性マッピングをカスタマイズする方法については、「[Azure Active Directory の SaaS アプリケーションのユーザー プロビジョニングの属性マッピングをカスタマイズする](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f388-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="8f388-107">SaaS アプリのユーザー プロビジョニングの詳細については、「[Azure AD の自動化された SaaS アプリのユーザー プロビジョニングとは](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f388-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="8f388-108">ユーザー プロビジョニング用に属性マッピングをカスタマイズする場合、マッピングする属性が [ソース属性] リストに表示されない場合があります。</span><span class="sxs-lookup"><span data-stu-id="8f388-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="8f388-109">「[アプリケーションにプロビジョニングするためにオンプレミスの Active Directory から Azure AD に属性を同期する](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping)」の記事では、オンプレミスの AD から Azure AD に同期することで、不足している属性を追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="8f388-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
