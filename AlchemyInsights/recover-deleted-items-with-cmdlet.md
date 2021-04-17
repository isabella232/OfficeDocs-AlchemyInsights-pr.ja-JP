---
title: コマンドレットで削除済みアイテムを復元する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835816"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="81ecb-102">コマンドレットで削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="81ecb-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="81ecb-103">[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) コマンドレットを使用して、メールボックス内の削除済みアイテムを表示します。</span><span class="sxs-lookup"><span data-stu-id="81ecb-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="81ecb-104">削除済みアイテムを見つけたら、[Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) コマンドレットを使用してそれらを復元します。</span><span class="sxs-lookup"><span data-stu-id="81ecb-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="81ecb-105">詳細については、「[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="81ecb-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="81ecb-106">このコマンドレットを実行する前に、メールボックス インポート エクスポートの役割を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="81ecb-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="81ecb-107">詳細については、「[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="81ecb-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
