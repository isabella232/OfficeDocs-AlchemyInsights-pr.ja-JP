---
title: Microsoft Planner のコメント
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001717"
- "3810"
ms.openlocfilehash: 98246b52e21c7a24d04e18ce77d96b28c65e7909
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911225"
---
# <a name="comments-in-microsoft-planner"></a>Microsoft Planner のコメント

プラン内のタスクに関するコメントは、プランに関連付けられている Microsoft 365 グループの Exchange Online メールボックスに保存されます。  タスクにコメントを投稿すると、メール通知がグループの受信トレイに送信され、そのタスクに対して以降に行われたコメントごとに電子メールが送信されます。

コメントに関連する一般的な問題に対する回答を次に示します。

- **ユーザーはメールを受信していません** - プランが属するグループのグループ受信トレイにコメントが送信されます。 ユーザーがグループ メールを受信するには、グループの会話をメンバーの受信トレイに送信するようにグループを構成する必要があります。

- **コメントは保存されていません** - コメントを追加したユーザーには、Microsoft 365 グループにメールを送信するアクセス権限がありません。 このシナリオの詳細については、「[Microsoft Planner のしくみ](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)」を参照してください。

- **アクセス権がありません**というエラー メッセージが表示される、または**ゲスト ユーザーがコメントを追加できません** - グループの受信トレイにメールを送信できないゲスト ユーザーに対して、このメッセージが表示されることがあります。 解決するには、ゲスト ユーザーのメールアドレスが有効であることを確認します。

- **削除されたユーザーがメールを受け取っています** - プランから削除される前にユーザーがタスクに対してコメントした場合、メールのスレッドにはそのユーザーがタスクに対するコメントごとに含められます。

Microsoft Planner のコメントの詳細については、「[Microsoft Planner のしくみ](https://techcommunity.microsoft.com/t5/planner-blog/how-microsoft-planner-works/ba-p/1214736)」および「[Microsoft Planner のタスクにコメントする](https://support.microsoft.com/office/comment-on-tasks-in-microsoft-planner-fd4aedde-7785-4cd0-96ee-122fbc9140e1)」を参照してください。
