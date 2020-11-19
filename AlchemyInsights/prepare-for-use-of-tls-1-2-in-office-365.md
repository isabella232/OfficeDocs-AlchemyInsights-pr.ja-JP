---
title: Microsoft 365 で TLS 1.2 を使用するための準備
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085909"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Microsoft 365 で TLS 1.2 を使用するための準備

2018 年 10 月 31 日の時点で、Microsoft 365 では TLS 1.2 への移行が継続されます。 2020 年 10 月 15 日以降、O365 のサービス全体で TLS1.0 および 1.1 が非推奨になります。 この変更の展開は今後数週間から数か月にわたって継続されますが、2020 年 10 月 15 日以降、O365 を使用する場合、TLS 1.0 /1.1 の通話が機能しなくなることを想定する必要があります。 以前に連絡 (2017 年 12 月の MC126199、2018 年 2 月の MC128929、2019 年 7 月の MC186827、2020 年 7 月の MC218794) したように、クラス最高の暗号化を提供し、既定でサービスの安全性を高めるために、すべてのオンラインサービスをトランスポート層セキュリティ (TLS) 1.2 以上に移行しています。 お客様は、サーバーとリソースに TLS 1.0 / 1.1 を使用することも選択できますが、O365 リソースとやり取りする場合は TLS1.2 以降のみが機能します。
  
これらの変更の詳細については、[こちら](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)と[こちら](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)をご覧ください。

  