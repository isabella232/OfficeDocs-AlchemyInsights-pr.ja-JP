---
title: メールボックスの自動返信を設定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046613"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>ユーザーのメールボックスの自動返信を設定する

**方法 1**

1. Microsoft 365 ポータルにサインインします。

2. **[ユーザー]、[アクティブ ユーザー]** (またはこれを共有メールボックスに設定した場合は、**[グループ]、[共有メールボックス]**) の順に移動します。

3. Microsoft Exchange メールボックスを持つユーザーを選択します。

4. 右側のフライアウト メニューで、**[メールの設定]、[自動返信]** の順に移動します (共有メールボックスの場合は、フライアウトで **[自動返信]** をクリックします)。

**方法 2**

1. 管理者の資格情報を使用して Microsoft 365 管理ポータルにサインインします。

2. **[管理センター]** を展開し、**[Exchange]** をクリックします。

3. 右上隅の画像をクリックし、**[別のユーザー]** をクリックして、変更するユーザーのメールボックスを選択します。

4. 左側で、**[オプション]** を選択し、**[メールの整理]**、**[自動返信]** の順にクリックします。

**方法 3**

Exchange Online PowerShell で次のコマンドレットを実行します。

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

このコマンドレットの詳細については、「[Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)」を参照してください。
