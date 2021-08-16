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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046757"
---
# <a name="your-archive-mailbox-is-almost-full"></a>アーカイブ メールボックスがほぼいっぱいです

ユーザーが **[アーカイブ メールボックスがほぼいっぱいです]**、または [アーカイブ メールボックスのサイズを増やす必要があります] という警告を受け取った場合は、次のヒントを参考にしてください。

1. ユーザーに Exchange Online プラン 1 が割り当てられている場合は、**Exchange Online プラン 2** ライセンスにアップグレードして、サイズを 50 GB から 100 GB に増やします。
1. ユーザーに **Exchange Online プラン 2** または Exchange Online Archiving アドオンを備えた Exchange Online プラン 1 のいずれかが既に割り当てられている場合は、以下の手順を使用して自動拡張アーカイブを有効にします。
 
    1. [Exchange Online PowerShell に接続します](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。
    2. ユーザーに対して次のコマンドレットを実行します。  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. 次のコマンドレットを実行して、ユーザーに対して有効になっていることを確認します。  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

詳細については、次のトピックを参照してください。

- [ 無制限のアーカイブを有効にする - 管理者ヘルプ - Microsoft 365 コンプライアンス | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [ ExchangeOnline の制限 - サービスの説明 | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [ 別のビジネス プランにアップグレードする | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

