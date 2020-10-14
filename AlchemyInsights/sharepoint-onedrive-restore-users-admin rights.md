---
title: OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670621"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング

この問題は、ユーザーの削除後に同じユーザー プリンシパル名 (UPN) でユーザーを再作成するときに最も頻繁に発生します。 新しいアカウントは、別の PUID (Passport 一意識別子) 値を使用して作成されます。 そのユーザーがサイト コレクションや自分の OneDrive にアクセスしようとしたときに、ユーザーの PUID は間違ったものになります。 もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。 SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。

1. この問題を解決するには、「[Microsoft 365 でユーザーを復元する](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)」に記載されている手順を実行して元の UPN を復元する必要があります。
2. 元のユーザーを復元できない場合は、「[ユーザー情報リストからユーザーを削除する]()」の手順を使用して OneDrive サイトから古いユーザーを削除する必要があります。 
3. この作業が完了したら、「[ユーザーの OneDrive に管理者を追加する](https://docs.microsoft.com/sharepoint/manage-user-profiles)」の手順に従って、OneDrive サイトに対する管理者権限がユーザーに付与されていることを確認してください。

アクセス許可レベルの詳細については、「[SharePoint のアクセス許可レベルについて](https://docs.microsoft.com/sharepoint/understanding-permission-levels)」を参照してください。
