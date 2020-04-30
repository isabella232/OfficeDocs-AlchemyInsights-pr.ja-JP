---
title: Teams のアップグレードを延期する
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
ms.openlocfilehash: fcf724e335bd6a7cb4801d9b2789447befc06ff7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912516"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="58ac7-102">Microsoft 主導の Teams アップグレードを延期する方法</span><span class="sxs-lookup"><span data-stu-id="58ac7-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="58ac7-103">**重要**: これを修正するにはサポート診断ツールを利用できますが、お客様は新しい管理センターをご使用でないようです。</span><span class="sxs-lookup"><span data-stu-id="58ac7-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="58ac7-104">新しい管理センターを使用するには、右上の **[新しい管理センター]** と示されているトグルを右にスライドしてください。</span><span class="sxs-lookup"><span data-stu-id="58ac7-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="58ac7-105">新しい管理センターで **[ヘルプが必要な場合]** ウィジェットをクリックし、「Teams のアップグレードを延期する」と入力してから、画面の指示に従って診断を実行します。</span><span class="sxs-lookup"><span data-stu-id="58ac7-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="58ac7-106">Skype for Business から Microsoft Teams への Microsoft 主導の自動アップグレードに関する通知を受け取り、自動アップグレードを後日に延期したい場合は、全体管理者が [Teams 管理ポータル](https://admin.teams.microsoft.com/dashboard)にログインし、[Microsoft Teams アップグレード] で **[ステータスの更新]** ボタンを選択した後、**[延期]** ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="58ac7-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="58ac7-107">テナントの Microsoft Teams への自動アップグレードの新しい日付を確認するには、Teams 管理ポータル ページを更新します。</span><span class="sxs-lookup"><span data-stu-id="58ac7-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="58ac7-108">**注:** [**延期**] ボタンは、自動アップグレードに関するメッセージ センターの通知を受け取った場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="58ac7-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="58ac7-109">全体管理者は [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) を実行して、現在のアップグレード ステータスの詳細を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="58ac7-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
