---
title: ワークフローが開始されない
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766102"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="99c8a-102">ワークフローが開始されない</span><span class="sxs-lookup"><span data-stu-id="99c8a-102">Workflow is not starting</span></span>

- <span data-ttu-id="99c8a-103">SharePoint 2010 および SharePoint 2013 のワークフローが開始されない。</span><span class="sxs-lookup"><span data-stu-id="99c8a-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="99c8a-104">ワークフローが開始されない場合は、サービスに一時的な問題が発生している可能性があります。この問題が発生すると、ワークフローの進行で断続的な遅延が発生します。</span><span class="sxs-lookup"><span data-stu-id="99c8a-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="99c8a-105">[サービスの正常性ダッシュボード](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。</span><span class="sxs-lookup"><span data-stu-id="99c8a-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="99c8a-106">この問題が発生してから 24 時間以上経過した場合は、サポート チケットを記録してください。</span><span class="sxs-lookup"><span data-stu-id="99c8a-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="99c8a-107">多くの場合、すでに解決策に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="99c8a-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="99c8a-108">解決策を完成させるために少なくとも 24 時間を与えてください。</span><span class="sxs-lookup"><span data-stu-id="99c8a-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="99c8a-109">SharePoint 2010 のワークフローの開始時に遅延がありました。</span><span class="sxs-lookup"><span data-stu-id="99c8a-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="99c8a-110">これは、ワークフローが大きなバッチでトリガーされた場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="99c8a-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="99c8a-111">(たとえば、一度に複数のアイテムが追加された場合)。</span><span class="sxs-lookup"><span data-stu-id="99c8a-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="99c8a-112">ワークフローはリアルタイムで実行するように設計されていないため、遅延は想定通りの動作です。</span><span class="sxs-lookup"><span data-stu-id="99c8a-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="99c8a-113">ワークフローが複雑な拡張可能オブジェクト マークアップ 言語 (XMOL) である場合、コンパイルに時間がかかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="99c8a-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="99c8a-114">[こちら](https://support.microsoft.com//kb/3043697)の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99c8a-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="99c8a-115">ワークフローを簡素化するか、Microsoft SharePoint 2013 ワークフローのプラットフォームの種類を使って再設計してください。</span><span class="sxs-lookup"><span data-stu-id="99c8a-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="99c8a-116">ワークフローの履歴が大きくなった場合は、アイテムを削除するか、新しい履歴リストを作成できます。</span><span class="sxs-lookup"><span data-stu-id="99c8a-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="99c8a-117">詳細情報: [Purge Workflow History (ワークフロー履歴の消去)](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="99c8a-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="99c8a-118">関連項目</span><span class="sxs-lookup"><span data-stu-id="99c8a-118">Related topics</span></span>
<span data-ttu-id="99c8a-119">SharePoint Online で Microsoft Flow を試す方法。</span><span class="sxs-lookup"><span data-stu-id="99c8a-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="99c8a-120">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="99c8a-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="99c8a-121">SharePoint and Flow (SharePoint と Flow)</span><span class="sxs-lookup"><span data-stu-id="99c8a-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


