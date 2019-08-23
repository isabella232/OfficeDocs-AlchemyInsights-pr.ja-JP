---
title: ワークフロー電子メールが送信されていません
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530884"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>ワークフロー電子メールが SharePoint リストまたはライブラリに送信されていません

1. ワークフローからの電子メールは、すべてのユーザーまたは特定のユーザーのみに送信されることはありません。また、電子メールメッセージを送信できないというエラーが表示され**ます。電子メールの受信者が有効であることを確認**します。

    そのサイトコレクションの [**すべて**のユーザー] アクセス許可グループ (ユーザー情報リスト) にユーザーが存在するかどうかを確認します。  サンプルの直接 URL:<tenant>https://sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?メンバーシップ Groupid = 0

    - ユーザーが存在しない場合は、ユーザーがページにサインインしていることを確認します。 
    - 外部ユーザーの場合は、招待状が承諾されていることを確認してください。
    - ユーザーがアクセス許可グループに存在する場合は、電子メールアドレスが正しいことを確認してください。
    - ユーザーの電子メールアドレスがここで設定されていない場合は、そのユーザーのためのサンプル通知を作成します。これにより、そのユーザーアカウントを SharePoint のユーザープロファイルからこのサイトコレクションに強制的に同期させることができます。
 
2. ワークフローからの電子メールは、サイトコレクションの管理者に送信されますが、他のユーザーに送信されることはありません。エラーは、 ** <span>https が Https</span>で禁止**されています://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail。
 

    [SharePoint グループに電子メールを送信する場合](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)は、「アクセス拒否」を参照してください。

    また、 **"制限付きアクセス" ユーザーアクセス許可のロックダウンモード**サイトコレクション機能がアクティブではないことを確認します。


## <a name="related-topics"></a>関連項目
SharePoint Online で Microsoft Flow を試す場合
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint およびフロー](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


