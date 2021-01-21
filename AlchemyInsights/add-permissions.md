---
title: アクセス許可を追加する
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
- "7783"
ms.openlocfilehash: b749278dc8e532ca723da5e6d8e4affc9a9266c7
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901740"
---
# <a name="add-permissions"></a><span data-ttu-id="ceb11-102">アクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="ceb11-102">Add permissions</span></span>

1. <span data-ttu-id="ceb11-103">管理者同意エンドポイントを使用して、[アプリケーションに対して静的に要求されたアクセス許可のリストを構成します](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#to-configure-the-list-of-statically-requested-permissions-for-an-application)。</span><span class="sxs-lookup"><span data-stu-id="ceb11-103">Use the admin consent endpoint to [configure the list of statically requested permissions for an application](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#to-configure-the-list-of-statically-requested-permissions-for-an-application).</span></span>
1. <span data-ttu-id="ceb11-104">アプリケーション登録を作成する機能を付与するために使用できる 2 つの権限があり、それぞれ動作が異なります。</span><span class="sxs-lookup"><span data-stu-id="ceb11-104">There are two permissions available for granting the ability to create application registrations, each with different behavior.</span></span> <span data-ttu-id="ceb11-105">詳細については、「[Azure Active Directory でのカスタム ロールのアプリケーション登録アクセス許可](https://docs.microsoft.com/azure/active-directory/roles/custom-available-permissions)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ceb11-105">For more information, see [Application registration permissions for custom roles in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/custom-available-permissions).</span></span>
1. <span data-ttu-id="ceb11-106">[ロール アクセス許可](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference#role-permissions): 各ロールに付与された Azure Active Directory の特定のアクセス許可を説明するテーブル。</span><span class="sxs-lookup"><span data-stu-id="ceb11-106">[Role Permissions](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference#role-permissions): tables that describe the specific permissions in Azure Active Directory given to each role.</span></span> <span data-ttu-id="ceb11-107">一部のロールには、Azure Active Directory 以外の Microsoft サービスで追加のアクセス許可がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="ceb11-107">Some roles may have additional permissions in Microsoft services outside of Azure Active Directory.</span></span>