---
title: 送信したメール メッセージを取り消す、または置き換えます
ms.author: daeite
author: daeite
manager: joallard
ms.date: 05/15/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 170fbd632f0289a45d9497ac26fbe7f90cf88318
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35356602"
---
# <a name="recall-or-replace-an-email-message"></a>送信したメール メッセージを取り消す、または置き換えます

- あなたは**あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。 たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。
- **PC の Outlook 2016 から送信されたメッセージのみを取り消す**ことができます。 ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。
- 管理者である場合は、 **PowerShell を使用して、ユーザーの代わりにメッセージを呼び戻す**ことができます。 管理センターからメッセージを取り消すことはできません。 詳細については、「組織内の電子メールメッセージの検索と削除」の下にスクロールしてください。

***送信した電子メールメッセージを呼び戻すまたは置換する***

1. Outlook ウィンドウの左側にあるフォルダーウィンドウで、[送信済みアイテム] フォルダーを選択します。
2. 取り消したいメッセージを開きます。 メッセージを開くには、ダブルクリックする必要があります。 閲覧ウィンドウに表示されるようにメッセージを選択しても、メッセージを取り消すことはできません。
3. [メッセージ] タブで、[**アクション** > を**取り消す**] を選択します。
4. [**このメッセージの未開封のコピーを削除**する] または [**未開封のコピーを削除して新しいメッセージに置き換える**] を選択し、[ **OK]** を選択します。
5. 代替メッセージを送信している場合は、メッセージを作成し、[**送信**] を選択します。
6. メッセージの取り消しの成功または失敗は、Outlook の受信者の設定によって異なります。

取り消しの確認方法など、詳細については、「[送信した電子メールメッセージを呼び戻すか置き換える](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)」を参照してください。

***組織内の電子メールメッセージの検索と削除***組織内の電子メールメッセージを検索して削除するには、グローバル管理者であることが最も簡単です。グローバル管理者でない場合は、アカウントが電子情報開示マネージャーの役割グループまたはコンプライアンス検索管理役割に追加されている必要があります。 メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。 これらの役割へのアクセス許可は、[セキュリティ & コンプライアンスセンター](https://protection.office.com/)で割り当てられます。

1. [コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。
2. [セキュリティ & コンプライアンスセンター PowerShell に接続](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)します。 

MFA を使用している場合は、「 [Connect To Office 365 Security & 多要素認証を使用](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)した PowerShell」を参照してください。 
