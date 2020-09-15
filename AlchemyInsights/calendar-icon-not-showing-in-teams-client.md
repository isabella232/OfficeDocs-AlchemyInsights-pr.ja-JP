---
title: Teams クライアントに予定表アイコンが表示されない
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
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684703"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="a94d7-102">Teams クライアントに予定表アイコンが表示されない</span><span class="sxs-lookup"><span data-stu-id="a94d7-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="a94d7-103">Teams の [予定表] タブでは、Exchange Web サービスを使用して Exchange メールボックスにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a94d7-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="a94d7-104">Exchange メールボックスは、オンラインまたはオンプレミスである可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a94d7-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="a94d7-105">オンライン ユーザーで [予定表] タブが表示されない場合には、[Exchange Online メールボックスのライセンスがあり、メールボックスが有効になっている](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)ことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a94d7-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="a94d7-106">Exchange Online の有効なメールボックスがあるものの [予定表] タブが表示されない場合には、ネットワークの問題が発生している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a94d7-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="a94d7-107">関係するユーザーに対して [Microsoft リモート接続アナライザー](https://testconnectivity.microsoft.com/)を使用して、**Microsoft Exchange Web サービス接続テスト**を実行します。</span><span class="sxs-lookup"><span data-stu-id="a94d7-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="a94d7-108">最後に、[Teams のアプリ - アプリのセットアップ ポリシー](https://admin.teams.microsoft.com/policies/app-setup)を調べて、予定表アプリがユーザーに適用されているポリシー (多くの場合は **(組織全体の既定) グローバル)** から削除されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a94d7-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="a94d7-109">ユーザーがオンプレミスに属している場合、ハイブリッド構成の正常性を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a94d7-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="a94d7-110">[ハイブリッド構成ウィザード](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)を使用して、トラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="a94d7-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="a94d7-111">[Teams では Exchange 2016 CU3 以上](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)が必要であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a94d7-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
