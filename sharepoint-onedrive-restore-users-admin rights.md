---
title: SharePoint と OneDrive へのアクセス権をユーザーに付与する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ae4d2c00be6387744bdc84e1d8a021530f80f8fa
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "35086039"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="41454-102">SharePoint と OneDrive へのアクセス権をユーザーに付与する</span><span class="sxs-lookup"><span data-stu-id="41454-102">Give users access to SharePoint and OneDrive</span></span>

<p><span data-ttu-id="41454-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">この問題は、多くの場合、ユーザーを削除してから同じユーザー プリンシパル名 (UPN) でユーザーを再作成したとき発生します。新しいアカウントは別の PUID (Passport 一意識別子) の値で作成されます。ユーザーがサイト コレクションまたは自分の OneDrive にアクセスしようとすると、ユーザーの PUID が間違ったものになります。もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。</span></span><span class="sxs-lookup"><span data-stu-id="41454-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN). The new account is created by using a different PUID (Passport Unique ID) value. When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID. A second scenario involves directory synchronization with an Active Directory organizational unit (OU). If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span></span></p> <p><span data-ttu-id="41454-104">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">この問題を解決するには、「<a href="https://docs.microsoft.com/ja-JP/office365/admin/add-users/restore-user?view=o365-worldwide">Office 365 でユーザーを復元する</a>」に記載された手順を実行して元の UPN を復元する必要があります。</span></span><span class="sxs-lookup"><span data-stu-id="41454-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">To resolve this issue you should restore the original UPN with the steps in the article, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">Restore a user in Office 365.</a></span></span></span></p> <p><span data-ttu-id="41454-105">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">この作業が完了したら、「<a href="https://docs.microsoft.com/ja-JP/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">ユーザーの OneDrive に管理者を追加する</a>」の手順に従って、OneDrive サイトに対する管理者権限がユーザーに付与されていることを確認してください。</span></span><span class="sxs-lookup"><span data-stu-id="41454-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to <a href="https://docs.microsoft.com/en-us/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive">Add admin's for a user's OneDrive.</a></span></span></span></p> <p><span data-ttu-id="41454-106">
  <span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">アクセス許可レベルの詳細については、「<a href="https://docs.microsoft.com/ja-JP/sharepoint/understanding-permission-levels">SharePoint のアクセス許可レベルについて</a>」を参照してください。&nbsp;</span></span><span class="sxs-lookup"><span data-stu-id="41454-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on permission levels, see the article, <a href="https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels">Understanding permission levels in SharePoint.</a>&nbsp;</span></span></span></p>
