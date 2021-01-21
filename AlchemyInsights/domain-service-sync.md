---
title: ドメイン サービスの同期
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885814"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="b82ff-102">ドメイン サービスの同期</span><span class="sxs-lookup"><span data-stu-id="b82ff-102">Domain service synchronization</span></span>

<span data-ttu-id="b82ff-103">Azure Active Directory Domain Services (Azure AD DS) 管理ドメイン内のオブジェクトと資格情報は、ドメイン内でローカルに作成することも、Azure Active Directory (Azure AD) テナントから同期することもできます。</span><span class="sxs-lookup"><span data-stu-id="b82ff-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="b82ff-104">Azure AD DS を初めて展開するときは、自動一方向同期が構成され、Azure AD からオブジェクトを複製するように開始されます。</span><span class="sxs-lookup"><span data-stu-id="b82ff-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="b82ff-105">この一方向の同期はバックグラウンドで実行され続け、Azure AD DS 管理ドメインは Azure AD からの変更によって最新の状態に保たれます。</span><span class="sxs-lookup"><span data-stu-id="b82ff-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="b82ff-106">Azure AD DS から Azure AD への同期は行われません。</span><span class="sxs-lookup"><span data-stu-id="b82ff-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="b82ff-107">Azure Active Directory Domain Services の同期の詳細については、「[Domain Services の同期](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b82ff-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
