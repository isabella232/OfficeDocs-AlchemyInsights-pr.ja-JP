---
title: OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 39f9b9b1ca22f6e5959e2b431fb373b0002c0a92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507816"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="e313b-102">OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="e313b-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="e313b-103">この問題は、ユーザーを削除し、同じユーザープリンシパル名 (UPN) を使用して再作成した場合によく発生します。</span><span class="sxs-lookup"><span data-stu-id="e313b-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e313b-104">新しいアカウントは、異なる PUID (Passport の一意の ID) 値を使用して作成されます。</span><span class="sxs-lookup"><span data-stu-id="e313b-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e313b-105">ユーザーがサイトコレクションまたは OneDrive にアクセスしようとすると、ユーザーの誤った PUID が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e313b-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e313b-106">2番目のシナリオでは、Active Directory の組織単位 (OU) とのディレクトリ同期が必要になります。</span><span class="sxs-lookup"><span data-stu-id="e313b-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e313b-107">ユーザーが既に SharePoint にサインインしていて、別の OU に移動して SharePoint と resynced した場合、この問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e313b-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="e313b-108">この問題を解決するには、記事「[Office 365 でユーザーを復元](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)する」の手順に従って元の UPN を復元する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e313b-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="e313b-109">元のユーザーを復元できない場合は、次の手順を使用して OneDrive サイトから古いユーザーを削除する必要があります。ユーザー[情報リストからユーザーを削除]()します。</span><span class="sxs-lookup"><span data-stu-id="e313b-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="e313b-110">この操作を実行すると、ユーザーの[onedrive の管理者を追加](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)する手順に従って、ユーザーに onedrive サイトへの管理者権限があることを確認できます。</span><span class="sxs-lookup"><span data-stu-id="e313b-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="e313b-111">アクセス許可レベルの詳細については、記事「 [SharePoint でのアクセス許可レベルについ](https://docs.microsoft.com/sharepoint/understanding-permission-levels)て」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e313b-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
