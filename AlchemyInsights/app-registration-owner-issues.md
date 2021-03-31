---
title: アプリ登録所有者の問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405815"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="cb58d-102">アプリ登録所有者の問題</span><span class="sxs-lookup"><span data-stu-id="cb58d-102">App Registration Owner issues</span></span>

<span data-ttu-id="cb58d-103">以下は、アプリ登録の所有者としてプリンシパルを追加するために使用できる方法です。</span><span class="sxs-lookup"><span data-stu-id="cb58d-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="cb58d-104">Azure AD PowerShell モジュールの使用 -</span><span class="sxs-lookup"><span data-stu-id="cb58d-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="cb58d-105">参照: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="cb58d-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="cb58d-106">Azure CLI を使用する - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="cb58d-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="cb58d-107">参照: [az 広告アプリの所有者](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="cb58d-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="cb58d-108">MS Graph を使用する - </span><span class="sxs-lookup"><span data-stu-id="cb58d-108">Using MS Graph -</span></span>

    <span data-ttu-id="cb58d-109">参照: [所有者を追加 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="cb58d-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="cb58d-110">Azure AD ポータルを使用する - [portal.azure.com](https://portal.azure.com/) > [AzureActiveDirectory] > [アプリの登録] > [アプリケーションの選択] > [所有者] > [所有者の追加] の順に移動します</span><span class="sxs-lookup"><span data-stu-id="cb58d-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="cb58d-111">**アプリケーションの所有者であるにもかかわらず、アプリ登録ブレードでアプリケーションを表示できませんか?**</span><span class="sxs-lookup"><span data-stu-id="cb58d-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="cb58d-112">アプリの所有者は管理者のロールとは異なります。</span><span class="sxs-lookup"><span data-stu-id="cb58d-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="cb58d-113">[[Azure AD 管理ポータルへのアクセスを制限する]](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) 設定が有効になっている場合、管理者だけがアプリ登録ポータルでアプリケーションを表示できます。</span><span class="sxs-lookup"><span data-stu-id="cb58d-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="cb58d-114">所有者がアプリケーションを表示できるようにするには、([いいえ]に設定して) この設定を無効にするか、特定のアプリケーションについてのみ所有者に管理者の役割を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="cb58d-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="cb58d-115">ただし、このためには、Azure AD Premium P2 ライセンスがあること、および[特権 ID 管理](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb58d-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
