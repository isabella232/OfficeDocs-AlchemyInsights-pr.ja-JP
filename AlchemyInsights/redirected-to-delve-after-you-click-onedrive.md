---
title: OneDrive for Business Web OneDrive が Delve にリダイレクトする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 8ba296c6986c767939ef51076551f95719d11aa2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752253"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="ae6c1-102">OneDrive をクリックした後に Delve にリダイレクトされる</span><span class="sxs-lookup"><span data-stu-id="ae6c1-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="ae6c1-103">この問題を解決するには、Office 365 管理者が個人用サイトを作成する権限をユーザーに付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-103">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="ae6c1-104">これは、個人用サイトに OneDrive for Business ページが作成されるためです。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-104">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="ae6c1-105">この権限を付与するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-105">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="ae6c1-106">SharePoint 管理センターで、[**ユーザープロファイル**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-106">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="ae6c1-107">[**人**] セクションで、[**ユーザー権限の管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-107">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="ae6c1-108">個人用サイトを作成するためのアクセス許可を必要とするユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-108">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="ae6c1-109">既定では、この設定は [**外部ユーザーを除くすべてのユーザー**] に設定されています。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-109">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="ae6c1-110">ユーザー、ユーザー、またはグループを追加した後で、追加したユーザー、ユーザー、またはグループが選択されていることを確認し、[**アクセス許可**] セクションまでスクロールして、[**個人用サイトの作成] (個人記憶域、ニュースフィード、およびフォロー対象のコンテンツ)**。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-110">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="ae6c1-111">[ **OK**] をクリックし、ユーザーが OneDrive ページを参照してサイトを作成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ae6c1-111">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
