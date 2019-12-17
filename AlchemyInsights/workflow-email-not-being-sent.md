---
title: ワークフロー メールが送信されない
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049378"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>SharePoint リストまたはライブラリのワークフロー メールが送信されない

1. ワークフローからのメールがすべてのユーザーまたは特定のユーザーにのみ送信されない、または "**電子メールを送信できません。電子メールの宛先が正しいか確認してください。**" というエラーが表示される場合。

    ユーザーがそのサイトコレクションの [**すべてのユーザー**] アクセス許可グループ (ユーザー情報リスト) に存在するかどうかを確認します。  直接 URL のサンプル: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0

    - ユーザーが存在しない場合は、ユーザーがページにサインインしていることを確認します。 
    - 外部ユーザーの場合は、招待が承諾されていることを確認します。
    - ユーザーがアクセス許可グループに存在する場合は、メール アドレスが正しいことを確認します。
    - ユーザーのメール アドレスがアクセス許可グループで設定されていない場合は、そのユーザー用にサンプル アラートを作成します。これにより、ユーザー アカウントは SharePoint のユーザー プロファイルからこのサイト コレクションに強制的に同期されます。
 
2. ワークフローからのメールは、サイト コレクション管理者に送信されます。他のユーザーに送信されることはなく、**HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail** エラーが表示されます。
 

    詳細については、「[SharePoint グループに電子メールを送信するとアクセスが拒否される](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)」を参照してください。

    また、サイト コレクションの機能である**制限付きアクセス ユーザーのアクセス許可ロックダウン モード**がアクティブになっていないことを確認します。


## <a name="related-topics"></a>関連項目
SharePoint Online で Microsoft Flow を試す方法。
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint and Flow (SharePoint と Flow)](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


