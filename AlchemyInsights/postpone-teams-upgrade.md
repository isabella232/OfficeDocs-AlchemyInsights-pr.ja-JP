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
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="3171c-102">Microsoft 主導の Teams アップグレードを延期する方法</span><span class="sxs-lookup"><span data-stu-id="3171c-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="3171c-103">Skype for Business から Microsoft Teams への Microsoft 主導の自動アップグレードに関する通知を受け取り、自動アップグレードを後日に延期したい場合、Office 365 グローバル管理者は [Teams 管理ポータル](https://admin.teams.microsoft.com/dashboard)にログインし、[**延期**] ボタンを選択できます。</span><span class="sxs-lookup"><span data-stu-id="3171c-103">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Office 365 Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and select the **Postpone** button.</span></span> <span data-ttu-id="3171c-104">テナントの Microsoft Teams への自動アップグレードの新しい日付を確認するには、Teams 管理ポータル ページを更新します。</span><span class="sxs-lookup"><span data-stu-id="3171c-104">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="3171c-105">**注:** [**延期**] ボタンは、自動アップグレードに関するメッセージ センターの通知を受け取った場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="3171c-105">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="3171c-106">Office 365 グローバル管理者は [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) を実行して、現在のアップグレード ステータスの詳細について確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="3171c-106">Office 365 Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span> 