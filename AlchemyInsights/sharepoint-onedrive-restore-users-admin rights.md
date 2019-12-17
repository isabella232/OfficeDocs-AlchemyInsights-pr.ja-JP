---
title: OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051610"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="ee3da-102">OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ee3da-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="ee3da-103">この問題は、ユーザーの削除後に同じユーザー プリンシパル名 (UPN) でユーザーを再作成するときに最も頻繁に発生します。</span><span class="sxs-lookup"><span data-stu-id="ee3da-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ee3da-104">新しいアカウントは、別の PUID (Passport 一意識別子) 値を使用して作成されます。</span><span class="sxs-lookup"><span data-stu-id="ee3da-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ee3da-105">そのユーザーがサイト コレクションや自分の OneDrive にアクセスしようとしたときに、ユーザーの PUID は間違ったものになります。</span><span class="sxs-lookup"><span data-stu-id="ee3da-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ee3da-106">もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。</span><span class="sxs-lookup"><span data-stu-id="ee3da-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ee3da-107">SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="ee3da-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="ee3da-108">この問題を解決するには、「[Office 365 でユーザーを復元する](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)」に記載された手順を実行して元の UPN を復元する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee3da-108">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="ee3da-109">元のユーザーを復元できない場合は、「[ユーザー情報リストからユーザーを削除する]()」の手順を使用して OneDrive サイトから古いユーザーを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee3da-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="ee3da-110">この作業が完了したら、「[ユーザーの OneDrive に管理者を追加する](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)」の手順に従って、OneDrive サイトに対する管理者権限がユーザーに付与されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ee3da-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="ee3da-111">アクセス許可レベルの詳細については、「[SharePoint のアクセス許可レベルについて](https://docs.microsoft.com/sharepoint/understanding-permission-levels)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee3da-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
