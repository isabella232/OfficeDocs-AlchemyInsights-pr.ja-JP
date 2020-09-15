---
title: 検疫されたメールがなくなった場合
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673719"
---
# <a name="missing-emails-in-quarantine"></a>検疫されたメールがなくなった場合

管理者は、[これらのメッセージを表示、解放、または削除](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)できます。

セキュリティ/コンプライアンス センターを開くには、[https://protection.office.com](https://protection.office.com/) へ移動します。 検疫ページを直接開くには、[https://protection.office.com/quarantine](https://protection.office.com/quarantine) にアクセスします。  

次の値に基づいて検索できます。  

- **[メッセージ ID]**: メッセージのグローバル一意識別子。 一覧でメッセージを選択すると、表示される **[詳細]** ポップアップ ウィンドウに **[メッセージ ID]** 値が表示されます。 管理者は、[メッセージ追跡](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)を使用して、メッセージとそれに対応する [メッセージ ID] 値を検索できます。
- **[送信者のメール アドレス]**: 単一の送信者のメール アドレス。
- **[受信者のメール アドレス]**: 単一の受信者のメール アドレス。
- **[件名]**: メッセージの件名全体を使用します。 この検索では大文字と小文字は区別されません。

検索条件を入力したら、![[更新] ボタン](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **[更新]** をクリックすると、結果がフィルター処理されます。

検疫内のメッセージとファイルを表示および管理するコマンドレットは、次のとおりです。
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): このコマンドレットはメッセージ専用であり、SharePoint Online、OneDrive for Business、または Teams の ATP からのマルウェアファイルではないことに注意してください。
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)