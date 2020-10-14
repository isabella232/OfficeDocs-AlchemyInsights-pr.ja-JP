---
title: 従来の電子情報開示ツールの廃止
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727788"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>従来の電子情報開示ツールの廃止

Microsoft 365 コンプライアンス センターの電子情報開示機能が刷新され、機能が向上したことにより、次に挙げる従来の電子情報開示ツールおよびコマンドレットは今後数か月間の間に廃止されます。

- Exchange 管理センターの[インプレース電子情報開示](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)および[インプレース ホールド](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。

- インプレース電子情報開示およびインプレース ホールドをサポートしている、Exchange Online の PowerShell コマンドレット。 (これらのコマンドレットは、まとめて *-MailboxSearch cmdlets と識別されます。) 次のコマンドレットが含まれます。

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell の [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) コマンドレット。
- Exchange Web Services API での次の操作。
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**廃止のタイムライン**:
- **2020 年 7 月 1 日**: 新しい検索と保留リストを作成できなくなりますが、ユーザーの自己責任において、既存の検索の実行、編集、および削除は行えます。 Microsoft サポートによる Exchange 管理センターのインプレース電子情報開示およびインプレース ホールドのサポートが終了します。
    
- **2020 年 10 月 1 日**: EAC のインプレース電子情報開示と保持機能は読み取り専用モードになるため、既存の検索と保持のみを削除できます。

**詳細については、以下を参照してください。**

 - [従来の電子情報開示検索と保持を Microsoft 365 コンプライアンス センターに移行する](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [従来の電子情報開示ツールの廃止](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [インプレース電子情報開示とインプレース ホールドに関するよくある質問](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



