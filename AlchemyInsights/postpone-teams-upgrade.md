---
title: Teams のアップグレードを延期する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2737"
- "4000006"
ms.openlocfilehash: 893a01ae74f8aec9bb0079430188e3cd6881b3009818830ea5572cfa41cdf71f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923982"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>Microsoft 主導の Teams アップグレードを延期する方法

**重要**: これを修正するにはサポート診断ツールを利用できますが、お客様は新しい管理センターをご使用でないようです。 新しい管理センターを使用するには、右上の **[新しい管理センター]** と示されているトグルを右にスライドしてください。 新しい管理センターで **[ヘルプが必要な場合]** ウィジェットをクリックし、「Teams のアップグレードを延期する」と入力してから、画面の指示に従って診断を実行します。

Skype for Business から Microsoft Teams への Microsoft 主導の自動アップグレードに関する通知を受け取り、自動アップグレードを後日に延期したい場合は、グローバル管理者が [Teams 管理ポータル](https://admin.teams.microsoft.com/dashboard)にログインし、[Microsoft Teams アップグレード] で **[ステータスの更新]** ボタンを選択した後、**[延期]** ボタンを選択します。テナントの Microsoft Teams への自動アップグレードの新しい日付を確認するには、Teams 管理ポータル ページを更新します。

**注:** [**延期**] ボタンは、自動アップグレードに関するメッセージ センターの通知を受け取った場合にのみ使用できます。 

全体管理者は [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) を実行して、現在のアップグレード ステータスの詳細を確認することもできます。
