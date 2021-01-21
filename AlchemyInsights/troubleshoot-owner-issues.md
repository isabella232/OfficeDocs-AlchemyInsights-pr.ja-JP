---
title: 所有者の問題のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901717"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="12c4f-102">所有者の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="12c4f-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="12c4f-103">所有者関連の問題のトラブルシューティングを行うには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="12c4f-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="12c4f-104">[Azure サブスクリプション管理者を追加または変更する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) グループは、グループ所有者によって所有および管理されます。</span><span class="sxs-lookup"><span data-stu-id="12c4f-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="12c4f-105">グループ所有者は、ユーザーまたはサービス プリンシパルであり、メンバーシップを含めたグループを管理できます。</span><span class="sxs-lookup"><span data-stu-id="12c4f-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="12c4f-106">グループ所有者を割り当てることができるのは、既存のグループ所有者またはグループを管理する管理者のみです。</span><span class="sxs-lookup"><span data-stu-id="12c4f-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="12c4f-107">グループ所有者がグループのメンバーである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="12c4f-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="12c4f-108">[[Azure サブスクリプション管理者の追加または変更]](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): この記事では、サブスクリプションの範囲で Azure RBAC を使用するユーザーの管理者役割を追加または変更する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="12c4f-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="12c4f-109">PowerShell を使用して、グループ所有者またはアプリケーション所有者を追加します。</span><span class="sxs-lookup"><span data-stu-id="12c4f-109">Use PowerShell to add a group owner or an application owner.</span></span>
