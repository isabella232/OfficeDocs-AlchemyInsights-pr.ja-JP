---
title: 予定表のアクセス許可
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819913"
---
# <a name="calendar-permissions"></a>予定表のアクセス許可

ユーザーは Outlook on Web やその他のクライアントで自分の予定表のアクセス許可を変更することができますが、管理者として調査を行う必要がある場合もあります。  
Exchange PowerShell コマンドレットを使用すると、ユーザーの予定表のアクセス許可が表示されます。

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

詳細については、次のトピックを参照してください。

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

予定表のアクセス許可は、予定表の共有で使用されます。Outlook カレンダーの共有に関する詳細情報については、次の記事を参照してください。

- [他のユーザーと Outlook 予定表を共有する](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Outlook on the web の自分の予定表を仕事のために共有する](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

予定表のアクセス許可のトラブルシューティングを行うには、[サポート/回復アシスタント](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) ツールを使用することができます。