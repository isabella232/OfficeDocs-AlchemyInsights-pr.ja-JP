---
title: 1 日のメールの制限を超えました。 ワークフローは中断されています。
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 5ae06919fde3c30b27975700fe17ecfd1bc2f675
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36818290"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="90807-103">1 日のメールの制限を超えました。</span><span class="sxs-lookup"><span data-stu-id="90807-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="90807-104">ワークフローは中断されています。</span><span class="sxs-lookup"><span data-stu-id="90807-104">Workflow is suspended.</span></span>

<span data-ttu-id="90807-105">このエラーは、次のシナリオに該当する場合に受信する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="90807-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="90807-106">SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。</span><span class="sxs-lookup"><span data-stu-id="90807-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="90807-107">ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。</span><span class="sxs-lookup"><span data-stu-id="90807-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="90807-108">ワークフローを実行すると、メール メッセージは送信されず、ユーザーは次のような動作に気付くはずです。</span><span class="sxs-lookup"><span data-stu-id="90807-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="90807-109">プラットフォームの種類に SharePoint 2013 を使用するワークフローでは、[**ワークフローの状態**] ページを参照します。</span><span class="sxs-lookup"><span data-stu-id="90807-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="90807-110">[ワークフローの状態] ページで、[**内部の状態**] は [**開始済み**] に設定され、情報の吹き出しには "**受信者に送信できません**" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="90807-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="90807-111">この問題を回避するには、[Exchange Online の送信者制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)を超過せずにメール メッセージを送信するようにワークフローを構成します。</span><span class="sxs-lookup"><span data-stu-id="90807-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="90807-112">たとえば、ワークフロー内で一時停止を使用したり、メールを Office 365 グループ、配布グループ、またはメールが有効なセキュリティ グループに送信したり、一度にメッセージを送信する相手を 200 人未満の受信者にしたりします。</span><span class="sxs-lookup"><span data-stu-id="90807-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="90807-113">詳細については、以下の[記事](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90807-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="90807-114">関連項目</span><span class="sxs-lookup"><span data-stu-id="90807-114">Related topics</span></span>
- [<span data-ttu-id="90807-115">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="90807-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="90807-116">SharePoint and Flow (SharePoint と Flow)</span><span class="sxs-lookup"><span data-stu-id="90807-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 