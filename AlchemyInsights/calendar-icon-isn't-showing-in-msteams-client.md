---
title: Microsoft Teams クライアントに予定表アイコンが表示されない
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584211"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="9ad30-102">Microsoft Teams クライアントに予定表アイコンが表示されない</span><span class="sxs-lookup"><span data-stu-id="9ad30-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="9ad30-103">Teams の **[予定表]** タブでは、Exchange Web サービスを使用して Exchange メールボックスにアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ad30-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="9ad30-104">Exchange メールボックスは、オンラインまたはオンプレミスである可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9ad30-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="9ad30-105">オンライン ユーザーで **[予定表]** タブが表示されない場合には、[Exchange Online メールボックスのライセンスがあり、メールボックスが有効になっている](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)ことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="9ad30-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="9ad30-106">ユーザーがオンプレミスに属している場合、ハイブリッド構成が正常であることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ad30-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="9ad30-107">[ハイブリッド構成ウィザード](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)を使用して、トラブルシューティングします。</span><span class="sxs-lookup"><span data-stu-id="9ad30-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="9ad30-108">[Teams では Exchange 2016 CU3 以上](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)が必要であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="9ad30-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="9ad30-109">詳細とトラブルシューティング手順の詳細については、「[Microsoft Teams と Exchange Server の相互作用の問題のトラブルシューティング](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ad30-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
