---
title: 'Teams のアップグレードを延期する '
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: 28c3a376170aba0ae43929865200fc85cd1c41f4
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/27/2019
ms.locfileid: "39626749"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Microsoft 主導の Teams アップグレードを延期する方法

Skype for Business から Microsoft Teams への Microsoft 主導の自動アップグレードに関する通知を受け取り、自動アップグレードを後日に延期したい場合、Office 365 グローバル管理者は [Teams 管理ポータル](https://admin.teams.microsoft.com/dashboard)にログインし、[**延期**] ボタンを選択できます。 テナントの Microsoft Teams への自動アップグレードの新しい日付を確認するには、Teams 管理ポータル ページを更新します。

**注:** [**延期**] ボタンは、自動アップグレードに関するメッセージ センターの通知を受け取った場合にのみ使用できます。 

Office 365 グローバル管理者は [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) を実行して、現在のアップグレード ステータスの詳細について確認することもできます。 