---
title: アーカイブ メールボックスがほぼいっぱいです
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975085"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="e0030-102">アーカイブ メールボックスがほぼいっぱいです</span><span class="sxs-lookup"><span data-stu-id="e0030-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="e0030-103">ユーザーが **[アーカイブ メールボックスがほぼいっぱいです]**、または [アーカイブ メールボックスのサイズを増やす必要があります] という警告を受け取った場合は、次のヒントを参考にしてください。</span><span class="sxs-lookup"><span data-stu-id="e0030-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="e0030-104">ユーザーに Exchange Online プラン 1 が割り当てられている場合は、**Exchange Online プラン 2** ライセンスにアップグレードして、サイズを 50 GB から 100 GB に増やします。</span><span class="sxs-lookup"><span data-stu-id="e0030-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="e0030-105">ユーザーに **Exchange Online プラン 2** または Exchange Online Archiving アドオンを備えた Exchange Online プラン 1 のいずれかが既に割り当てられている場合は、以下の手順を使用して自動拡張アーカイブを有効にします。</span><span class="sxs-lookup"><span data-stu-id="e0030-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="e0030-106">[Exchange Online PowerShell に接続します](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="e0030-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="e0030-107">ユーザーに対して次のコマンドレットを実行します。  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="e0030-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="e0030-108">次のコマンドレットを実行して、ユーザーに対して有効になっていることを確認します。  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="e0030-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="e0030-109">詳細については、次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0030-109">For more information see:</span></span>

- [<span data-ttu-id="e0030-110"> 無制限のアーカイブを有効にする - 管理者ヘルプ - Microsoft 365 コンプライアンス | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="e0030-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="e0030-111"> ExchangeOnline の制限 - サービスの説明 | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="e0030-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="e0030-112"> 別のビジネス プランにアップグレードする | Microsoft Docs</span><span class="sxs-lookup"><span data-stu-id="e0030-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

