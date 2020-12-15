---
title: 送信したメール メッセージを取り消す、または置き換えます
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353511"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Microsoft 365 でメール メッセージを取り消す、または置き換える

- あなたは **あなたの組織内の人々に送られたメッセージだけを取り消すことができます**。 たとえば、Gmail アドレスに送信された場合は、メッセージを取り消すことはできません。
- **PC 版 Outlook から送信されたメッセージのみを取り消すことができます**。 ユーザーが、Outlook for Mac またはOutlook on the web を使用してメッセージを送信する場合、取り消すことができません。
- テナント管理者は、**PowerShell を使用してユーザーに代わってメッセージを取り消す** ことができます (詳細については、「[メール メッセージの検索と削除](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)」を参照してください)。
- 管理センターからメッセージを取り消すことはできません。 下にスクロールして、「Office 365 組織でメール メッセージの検索と削除を行う」を参照してください。

**送信したメール メッセージを取り消す、または置き換える**

1. Outlook ウィンドウの左側のフォルダー ペインで、[送信済みアイテム] フォルダーを選びます。
2. 取り消すメッセージを開きます。 メッセージを開くにはダブルクリックする必要があります。 閲覧ウィンドウに表示されるようにメッセージを選択しても、メッセージを取り消すことはできません。
3. [メッセージ] タブから、[**操作]、[** > **メッセージの取り消し**]を選択します。
4. [**未読のこのメッセージのコピーを削除する**]、または [**未読のコピーを削除して新しいメッセージに置き換える**] を選び、それから [**OK**] を選択します。
5. 代わりのメッセージを送信する場合、メッセージを作成し、**[送信]** を選択します。
6. メッセージ取り消しの成功または失敗は、受信者の Outlook の設定によって決まります。

取り消しを確認する方法など、詳細については、「[送信したメールメッセージを取り消す、または置き換える](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)」を参照してください。

**_組織内のメール メッセージを検索して削除するには_**、グローバル管理者であることが最も簡単です。グローバル管理者でない場合は、アカウントを電子情報開示マネージャーの役割グループ、またはコンプライアンス検索の管理の役割に追加する必要があります。 メッセージを削除するには、Organization Management ロールグループのメンバーであるか、検索と消去の管理ロールが割り当てられている必要があります。 これらのロールへの権限は、[セキュリティ/コンプライアンス センター](https://protection.office.com/)で付与されます。

1. [コンテンツ検索を作成し、](https://docs.microsoft.com/microsoft-365/compliance/content-search) 削除するメッセージを見つけます。
2. [セキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。

多要素認証 (MFA) を使用している場合、「[多要素認証を使用して Microsoft 365 セキュリティ/コンプライアンス センター PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)」を参照してください。
