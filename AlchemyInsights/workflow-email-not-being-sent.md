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
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36180404"
---
# <a name="workflow-email-is-not-being-sent"></a>ワークフロー電子メールが送信されていません

1. ワークフローからの電子メールは、すべてのユーザーまたは特定のユーザーのみに送信されることはありません。また、電子メールメッセージを送信できないというエラーが表示され**ます。電子メールの受信者が有効であることを確認**します。

そのサイトコレクションの [**すべて**のユーザー] アクセス許可グループ (ユーザー情報リスト) にユーザーが存在するかどうかを確認します。  サンプルの直接 URL:<tenant>https://sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?メンバーシップ Groupid = 0

- ユーザーが存在しない場合は、ユーザーがページにサインインしていることを確認します。 
- 外部ユーザーの場合は、招待状が承諾されていることを確認してください。
- ユーザーがアクセス許可グループに存在する場合は、電子メールアドレスが正しいことを確認してください。
- ユーザーの電子メールアドレスがここで設定されていない場合は、そのユーザーのためのサンプル通知を作成します。これにより、そのユーザーアカウントを SharePoint のユーザープロファイルからこのサイトコレクションに強制的に同期させることができます。
 
2. ワークフローからの電子メールは、サイトコレクション管理者に送信されますが、他のユーザーに送信されることはありません。また、 **HTTP 禁止<spam> <spam>** のエラーを<spam> <spam>参照してください。
 

[グループに電子メールを送信する場合は、アクセス拒否](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)を参照してください。

また、 **"制限付きアクセス" ユーザーアクセス許可のロックダウンモード**サイトコレクション機能がアクティブではないことを確認します。

## <a name="related-topics"></a>関連項目
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint およびフロー](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


