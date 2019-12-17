---
title: Outlook デスクトップでメール メッセージを取り消す、または置き換える
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496116"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Outlook メール メッセージを取り消す、または置き換える

- 管理者は、**PowerShell を使用してユーザーの代理のメッセージを取り消すことが**できます。 管理センターからメッセージを取り消すことはできません。
- あなたは**あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。 たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。
- あなたは **PC の Outlook 2016 から送信されたメッセージだけを取り消すことができます**。 ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。

送信したメール メッセージを取り消す、または置き換えるには：

1. Outlook ウィンドウの左側のフォルダー ペインで、[送信済みアイテム] フォルダーを選択します。
1. 取り消したいメッセージをクリックして開きます。
1. **メッセージ**タブを選択、それから**Actions** > **Recall This Message**を選択。
1. [**未読のこのメッセージのコピーを削除する**]を選択、または [**未読のコピーを削除して新しいメッセージに置き換える**] 、そして[**OK**] を選択します。
1. 代わりのメッセージを送信する場合、メッセージを作成し、[**送信**] を選択します。
1. メッセージ取り消しの成功または失敗は、受信者のOutlookの設定によって決まります。 取り消しの状況をチェックするステップについては、[こちらの記事](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)を参照してください。

組織内の電子メールメッセージを検索して削除します

- グローバル管理者ではない場合、メッセージを検索するには、自分のアカウントをeDiscovery ManagerロールまたはCompliance Search管理ロールに追加する必要があります。 メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。 これらのロールの権限は、[セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/?linkid=2083731)で付与されます。
- [コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。
- [セキュリティ/コンプライアンス センターのPowerShellに接続します](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。

多要素認証を使用している場合、以下を参照してください [多要素認証を使用してOffice 365のセキュリティ/コンプライアンス センターのPowerShellに接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。