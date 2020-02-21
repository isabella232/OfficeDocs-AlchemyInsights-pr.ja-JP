---
title: 従来の電子情報開示ツールの廃止
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158090"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>従来の電子情報開示ツールの廃止

Microsoft 365 コンプライアンスセンターの新機能と改善された電子情報開示機能の結果として、次の従来の電子情報開示ツールおよびコマンドレットを使用すると、今後数か月で廃止されることになります。

- Exchange 管理センターでは、[インプレース電子情報開示](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)と[インプレース保持](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)が行われます。

- インプレース電子情報開示とインプレース保持をサポートする Exchange Online の PowerShell コマンドレット。 (これらのコマンドレットは、Get-mailboxsearch コマンドレットと総称して識別されます。)これには、次のコマンドレットが含まれます。

    - [Get-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Get-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Get-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Get-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell の[検索-メールボックス](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)コマンドレット。
- Exchange Web サービス API の次の操作。
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery version 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**定年後のタイムライン**:
- 2020年4月1日: 新しい検索と保持を作成することはできませんが、既存の検索を自分のリスクで実行、編集、削除することはできます。 Microsoft サポートは、EAC でインプレース電子情報開示 & 保持をサポートしなくなります。

- 2020年7月1日: インプレース電子情報開示 & は、EAC の機能を読み取り専用モードで保持します。 これは、既存の検索と保持を削除できることを意味します。

**詳細については、以下を参照してください**。

 - [従来の電子情報開示検索と保持を Microsoft 365 コンプライアンスセンターに移行する](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [従来の電子情報開示ツールの廃止](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [インプレースの電子情報開示とインプレース保持に関する Faq](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



