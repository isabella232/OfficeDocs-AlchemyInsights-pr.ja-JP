---
title: PowerShell スクリプトを Exchange Online に接続する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: ac6aa835123cb7557016edbc0ab9ef98763f64b36dbd29c744318e67416d5a92
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53915376"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a>PowerShell スクリプトを Exchange Online に接続する

Exchange Online の基本認証は廃止されます。今後の方法は、スクリプトおよび無人タスクに証明書ベースの認証を使用して接続することです。 詳細については、[「EXO V2 モジュールの無人スクリプトのアプリ専用の認証」](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2) を参照してください。