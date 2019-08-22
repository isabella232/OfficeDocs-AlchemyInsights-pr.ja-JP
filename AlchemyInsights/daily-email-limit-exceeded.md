---
title: 毎日のメールの制限を超えました。 ワークフローは中断されます。
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514462"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="1895a-103">毎日のメールの制限を超えました。</span><span class="sxs-lookup"><span data-stu-id="1895a-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="1895a-104">ワークフローは中断されます。</span><span class="sxs-lookup"><span data-stu-id="1895a-104">Workflow is suspended.</span></span>

<span data-ttu-id="1895a-105">このエラーは、次のシナリオで受け取ることがあります。</span><span class="sxs-lookup"><span data-stu-id="1895a-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="1895a-106">SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。</span><span class="sxs-lookup"><span data-stu-id="1895a-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="1895a-107">ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。</span><span class="sxs-lookup"><span data-stu-id="1895a-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="1895a-108">ワークフローを実行すると、電子メールメッセージは送信されず、次のような現象が発生します。</span><span class="sxs-lookup"><span data-stu-id="1895a-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="1895a-109">SharePoint 2013 プラットフォームの種類を使用するワークフローの場合は、[**ワークフローの状態**] ページを参照します。</span><span class="sxs-lookup"><span data-stu-id="1895a-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="1895a-110">[ワークフローの状態] ページで、[**内部の状態**] が [**開始**] に設定されており、情報のバルーンが**受信者に送信できない**ように表示されます。</span><span class="sxs-lookup"><span data-stu-id="1895a-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="1895a-111">この問題を回避するには、 [Exchange Online の送信者の制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)を超えずに電子メールメッセージを送信するようにワークフローを構成します。</span><span class="sxs-lookup"><span data-stu-id="1895a-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="1895a-112">たとえば、ワークフローで一時停止を使用するか、Office 365 グループ、配布グループまたはメールが有効なセキュリティグループに電子メールを送信するか、またはメッセージを1度に200人より少ない受信者に送信します。</span><span class="sxs-lookup"><span data-stu-id="1895a-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="1895a-113">詳細については、次の[記事](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1895a-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="1895a-114">関連項目</span><span class="sxs-lookup"><span data-stu-id="1895a-114">Related topics</span></span>
- [<span data-ttu-id="1895a-115">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="1895a-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="1895a-116">SharePoint およびフロー</span><span class="sxs-lookup"><span data-stu-id="1895a-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 