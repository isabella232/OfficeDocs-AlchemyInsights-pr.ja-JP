---
title: ワークフローが開始されない
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36738094"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="28cb1-102">ワークフローが開始されない</span><span class="sxs-lookup"><span data-stu-id="28cb1-102">Workflow is not starting</span></span>

- <span data-ttu-id="28cb1-103">SharePoint 2010 および SharePoint 2013 のワークフローが開始されない。</span><span class="sxs-lookup"><span data-stu-id="28cb1-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="28cb1-104">ワークフローが開始されない場合は、サービスに一時的な問題が発生している可能性があります。この問題が発生すると、ワークフローの進行で断続的な遅延が発生します。</span><span class="sxs-lookup"><span data-stu-id="28cb1-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="28cb1-105">[サービスの正常性ダッシュボード](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。</span><span class="sxs-lookup"><span data-stu-id="28cb1-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="28cb1-106">この問題が発生してから 24 時間以上経過した場合は、サポート チケットを記録してください。</span><span class="sxs-lookup"><span data-stu-id="28cb1-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="28cb1-107">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="28cb1-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="28cb1-108">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="28cb1-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="28cb1-109">SharePoint 2010 のワークフローの開始時に遅延がありました。</span><span class="sxs-lookup"><span data-stu-id="28cb1-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="28cb1-110">これは、ワークフローが大きなバッチでトリガーされた場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="28cb1-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="28cb1-111">(たとえば、一度に複数のアイテムが追加された場合)。</span><span class="sxs-lookup"><span data-stu-id="28cb1-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="28cb1-112">ワークフローはリアルタイムで実行するように設計されていないため、遅延は想定通りの動作です。</span><span class="sxs-lookup"><span data-stu-id="28cb1-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="28cb1-113">ワークフローが複雑な拡張可能オブジェクト マークアップ 言語 (XMOL) である場合、コンパイルに時間がかかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="28cb1-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="28cb1-114">[こちら](https://support.microsoft.com//kb/3043697)の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28cb1-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="28cb1-115">ワークフローを簡素化するか、Microsoft SharePoint 2013 ワークフローのプラットフォームの種類を使って再設計してください。</span><span class="sxs-lookup"><span data-stu-id="28cb1-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="28cb1-116">ワークフローの履歴が大きくなった場合は、アイテムを削除するか、新しい履歴リストを作成できます。</span><span class="sxs-lookup"><span data-stu-id="28cb1-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="28cb1-117">詳細情報: [Purge Workflow History (ワークフロー履歴の消去)](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="28cb1-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="28cb1-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="28cb1-118">Related topics</span></span>
<span data-ttu-id="28cb1-119">SharePoint Online で Microsoft Flow を試す方法。</span><span class="sxs-lookup"><span data-stu-id="28cb1-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="28cb1-120">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="28cb1-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="28cb1-121">SharePoint and Flow (SharePoint と Flow)</span><span class="sxs-lookup"><span data-stu-id="28cb1-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


