---
title: コマンドレットで削除済みアイテムを復元する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741308"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="9b254-102">コマンドレットで削除済みアイテムを復元する</span><span class="sxs-lookup"><span data-stu-id="9b254-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="9b254-103">[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) コマンドレットを使用して、メールボックス内の削除済みアイテムを表示します。</span><span class="sxs-lookup"><span data-stu-id="9b254-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="9b254-104">削除済みアイテムを見つけたら、[Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) コマンドレットを使用してそれらを復元します。</span><span class="sxs-lookup"><span data-stu-id="9b254-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="9b254-105">詳細については、「[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9b254-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="9b254-106">このコマンドレットを実行する前に、メールボックス インポート エクスポートの役割を割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b254-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="9b254-107">詳細については、「[Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9b254-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
