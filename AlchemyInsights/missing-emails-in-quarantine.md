---
title: 検疫されたメールがなくなった場合
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
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539829"
---
# <a name="missing-emails-in-quarantine"></a>検疫されたメールがなくなった場合

管理者は、[これらのメッセージを表示、解放、または削除](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)できます。

セキュリティ/コンプライアンス センターを開くには、[https://protection.office.com](https://protection.office.com/) へ移動します。 検疫ページを直接開くには、[https://protection.office.com/quarantine](https://protection.office.com/quarantine) にアクセスします。  

次の値に基づいて検索できます。  

- **[メッセージ ID]**: メッセージのグローバル一意識別子。 一覧でメッセージを選択すると、表示される **[詳細]** ポップアップ ウィンドウに **[メッセージ ID]** 値が表示されます。 管理者は、[メッセージ追跡](/microsoft-365/security/office-365-security/message-trace-scc)を使用して、メッセージとそれに対応する [メッセージ ID] 値を検索できます。
- **[送信者のメール アドレス]**: 単一の送信者のメール アドレス。
- **[受信者のメール アドレス]**: 単一の受信者のメール アドレス。
- **[件名]**: メッセージの件名全体を使用します。 この検索では大文字と小文字は区別されません。

検索条件を入力したら、![[更新] ボタン](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **[更新]** をクリックすると、結果がフィルター処理されます。

検疫内のメッセージとファイルを表示および管理するコマンドレットは、次のとおりです。
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): このコマンドレットはメッセージ専用であり、SharePoint Online、OneDrive for Business、Teams 用の Microsoft Defender for Office 365 からのマルウェア ファイルではないことに注意してください。
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)