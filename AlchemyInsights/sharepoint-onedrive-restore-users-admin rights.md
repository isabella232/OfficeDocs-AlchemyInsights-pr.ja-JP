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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957798"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>OneDrive for Business サイトへのアクセス拒否メッセージのトラブルシューティング

この問題は、多くの場合、ユーザーを削除してから同じユーザー プリンシパル名 (UPN) でユーザーを再作成したとき発生します。新しいアカウントは別の PUID (Passport 一意識別子) の値で作成されます。ユーザーがサイト コレクションまたは自分の OneDrive にアクセスしようとすると、ユーザーの PUID が間違ったものになります。もう 1 つのシナリオには、Active Directory 組織単位 (OU) とのディレクトリ同期が関連します。SharePoint にサインインしているユーザーが、別の OU に移動されて SharePoint と再同期されると、この問題が発生することがあります。

1. この問題を解決するには、「[Microsoft 365 でユーザーを復元する](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)」に記載されている手順を実行して元の UPN を復元する必要があります。
2. 元のユーザーを復元できない場合は、「[ユーザー情報リストからユーザーを削除する]()」の手順を使用して OneDrive サイトから古いユーザーを削除する必要があります。 
3. この作業が完了したら、「[ユーザーの OneDrive に管理者を追加する](https://docs.microsoft.com/sharepoint/manage-user-profiles)」の手順に従って、OneDrive サイトに対する管理者権限がユーザーに付与されていることを確認してください。

アクセス許可レベルの詳細については、「[SharePoint のアクセス許可レベルについて](https://docs.microsoft.com/sharepoint/understanding-permission-levels)」を参照してください。
