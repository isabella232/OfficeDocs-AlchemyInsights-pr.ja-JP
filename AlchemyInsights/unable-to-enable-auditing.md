---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/19/2019
ms.locfileid: "35085989"
---
# <a name="unable-to-enable-unified-auditing"></a>統合監査を有効にできない

Office 365 組織の統合監査を有効にしようとすると、次のようなエラーが表示されることがあります。

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

この問題を解決するには、次の手順を実行します。

1. [Exchange Online PowerShell に接続します](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。

2. 次のコマンドレットを実行します。

   ```
   Enable-OrganizationCustomization
   ```

3. 先の設定が有効になるまで 60 分間待ちます。

4. Exchange Online PowerShell で次のコマンドを実行します。

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

詳細については、次の記事を参照してください。

- [多要素認証を使用して Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 監査ログの検索を有効または無効にする](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
