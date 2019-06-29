---
title: OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354802"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング

この問題は、ユーザーを削除し、同じユーザープリンシパル名 (UPN) を使用して再作成した場合によく発生します。 新しいアカウントは、異なる PUID (Passport の一意の ID) 値を使用して作成されます。 ユーザーがサイトコレクションまたは OneDrive にアクセスしようとすると、ユーザーの誤った PUID が表示されます。 2番目のシナリオでは、Active Directory の組織単位 (OU) とのディレクトリ同期が必要になります。 ユーザーが既に SharePoint にサインインしていて、別の OU に移動して SharePoint と resynced した場合、この問題が発生する可能性があります。

この問題を解決するには、記事「[Office 365 でユーザーを復元](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)する」の手順に従って元の UPN を復元する必要があります。

この操作を実行すると、ユーザーの[onedrive の管理者を追加](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)する手順に従って、ユーザーに onedrive サイトへの管理者権限があることを確認できます。

アクセス許可レベルの詳細については、記事「 [SharePoint でのアクセス許可レベルについ](https://docs.microsoft.com/sharepoint/understanding-permission-levels)て」を参照してください。
