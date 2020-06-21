---
title: 2419-unable-to-enable-auditing
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510433"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="4e812-102">統合監査を有効にできない</span><span class="sxs-lookup"><span data-stu-id="4e812-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="4e812-103">組織の統合監査を有効にしようとすると、次のようなエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e812-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="4e812-104">この問題を解決するには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="4e812-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="4e812-105">[Exchange Online PowerShell に接続します](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="4e812-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="4e812-106">次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="4e812-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="4e812-107">先の設定が有効になるまで 60 分間待ちます。</span><span class="sxs-lookup"><span data-stu-id="4e812-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="4e812-108">Exchange Online PowerShell で次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="4e812-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="4e812-109">詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e812-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="4e812-110">多要素認証を使用して Exchange Online PowerShell に接続する</span><span class="sxs-lookup"><span data-stu-id="4e812-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="4e812-111">監査ログ検索を有効または無効にする</span><span class="sxs-lookup"><span data-stu-id="4e812-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
