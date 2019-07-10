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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354802"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング

この問題は、ユーザーの削除後に同じユーザー プリンシパル名 (UPN) でユーザーを再作成するときに最も頻繁に発生します。 新しいアカウントは、別の PUID (Passport 一意識別子) 値を使用して作成されます。 そのユーザーがサイト コレクションや自分の OneDrive にアクセスしようとしたときに、ユーザーの PUID は間違ったものになります。 もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。 SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。

この問題を解決するには、「[Office 365 でユーザーを復元する](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)」に記載された手順を実行して元の UPN を復元する必要があります。

この作業が完了したら、「[ユーザーの OneDrive に管理者を追加する](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)」の手順に従って、OneDrive サイトに対する管理者権限がユーザーに付与されていることを確認してください。

アクセス許可レベルの詳細については、「[SharePoint のアクセス許可レベルについて](https://docs.microsoft.com/sharepoint/understanding-permission-levels)」を参照してください。
