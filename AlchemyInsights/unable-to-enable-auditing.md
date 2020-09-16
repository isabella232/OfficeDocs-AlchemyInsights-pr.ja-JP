---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767604"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="5128c-102">統合監査を有効にできない</span><span class="sxs-lookup"><span data-stu-id="5128c-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="5128c-103">組織の統合監査を有効にしようとすると、次のようなエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5128c-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="5128c-104">この問題を解決するには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="5128c-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="5128c-105">[Exchange Online PowerShell に接続します](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="5128c-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="5128c-106">次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="5128c-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="5128c-107">先の設定が有効になるまで 60 分間待ちます。</span><span class="sxs-lookup"><span data-stu-id="5128c-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="5128c-108">Exchange Online PowerShell で次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="5128c-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="5128c-109">詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5128c-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="5128c-110">多要素認証を使用して Exchange Online PowerShell に接続する</span><span class="sxs-lookup"><span data-stu-id="5128c-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="5128c-111">監査ログ検索を有効または無効にする</span><span class="sxs-lookup"><span data-stu-id="5128c-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
