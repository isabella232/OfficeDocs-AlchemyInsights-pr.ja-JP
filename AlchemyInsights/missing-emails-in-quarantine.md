---
title: 検疫に電子メールがない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569878"
---
# <a name="missing-emails-in-quarantine"></a>検疫に電子メールがない

管理者は[、これらのメッセージを表示、リリース、または削除できます。](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

セキュリティ & コンプライアンスセンターを開くには、に移動 [https://protection.office.com](https://protection.office.com/) します。 [検疫] ページを直接開くには、に移動 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) します。  

次の値に基づいて検索できます。  

- **[メッセージ ID]**: メッセージのグローバル一意識別子。 一覧でメッセージを選択すると、表示される [**詳細**] ポップアップウィンドウに、**メッセージ ID**の値が表示されます。 管理者は、[メッセージ追跡](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)を使用して、メッセージとそれに対応する [メッセージ ID] 値を検索できます。
- **[送信者のメール アドレス]**: 単一の送信者のメール アドレス。
- **[受信者のメール アドレス]**: 単一の受信者のメール アドレス。
- **[件名]**: メッセージの件名全体を使用します。 この検索では大文字と小文字は区別されません。

検索条件を入力した後、[ ![ 更新] ボタンの [ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **更新**] をクリックして結果をフィルター処理します。  

検疫内のメッセージおよびファイルを表示および管理するには、次のコマンドレットを使用します。
- [Get-quarantinemessage を削除します。](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): このコマンドレットは、メッセージのみを対象としています。このコマンドレットは、SharePoint Online、OneDrive for business、または TEAMS の ATP ファイルではなく、メッセージのみを対象としています。
- [Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)