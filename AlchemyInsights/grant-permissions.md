---
title: アクセス許可を付与する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901744"
---
# <a name="grant-permissions"></a><span data-ttu-id="50eb1-102">アクセス許可を付与する</span><span class="sxs-lookup"><span data-stu-id="50eb1-102">Grant permissions</span></span>

1. <span data-ttu-id="50eb1-103">**テナント全体の管理者の同意を付与する**: Azure ポータル、Azure AD PowerShell の使用、または同意プロンプト自体からテナント全体の管理者の同意を付与する手順については、「[アプリケーションに対してテナント全体の管理者の同意を付与する](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50eb1-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="50eb1-104">**特定のユーザーに代わって同意を付与する**: 管理者は、組織全体に同意を付与する代わりに、[Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) を使用して、単一のユーザーに代わって委任されたアクセス許可に同意を付与することもできます。</span><span class="sxs-lookup"><span data-stu-id="50eb1-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="50eb1-105">詳細については、「[ユーザーの代わりにアクセスを取得](https://docs.microsoft.com/graph/auth-v2-user)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="50eb1-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>