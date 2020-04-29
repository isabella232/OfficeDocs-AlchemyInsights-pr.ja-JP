---
title: SharePoint の大きなリスト
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767290"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="1dbea-102">SharePoint で大きなリストおよびライブラリを使用する</span><span class="sxs-lookup"><span data-stu-id="1dbea-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="1dbea-p101">SharePoint のリストおよびライブラリには、最大 3,000 万個のアイテムを含めることができます。ただし、5,000 個を超えるアイテムが含まれる場合、それらを使用しようとすると、リスト ビューのしきい値エラーが表示されることがあります。このしきい値は、サービスのパフォーマンスを維持するために設定されており、変更することはできません。このしきい値に達しないようにするには、次を実行します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-p101">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them. This threshold is in place to maintain performance of the service. It can't be changed. To avoid hitting this threshold:</span></span>

<span data-ttu-id="1dbea-107">**モダンを使用する**</span><span class="sxs-lookup"><span data-stu-id="1dbea-107">**Use modern**</span></span>

<span data-ttu-id="1dbea-108">表示アイテムが多いビューの場合、モダン環境で最適に動作します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="1dbea-109">[モダン環境を使用](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)すると、クラシック環境で発生する可能性があるエラーを回避できます。</span><span class="sxs-lookup"><span data-stu-id="1dbea-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="1dbea-110">**インデックスを追加する**</span><span class="sxs-lookup"><span data-stu-id="1dbea-110">**Add indexes**</span></span>

<span data-ttu-id="1dbea-111">インデックスが作成されていない列によるフィルター処理または並べ替えを実行すると、エラー メッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1dbea-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="1dbea-112">[設定] メニューの [**リストの設定**] から手動で[インデックスを追加](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)してから、**インデックス付きの列**を追加します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="1dbea-113">**リスト ビューを編集する**</span><span class="sxs-lookup"><span data-stu-id="1dbea-113">**Edit the list view**</span></span>

<span data-ttu-id="1dbea-114">大規模なリストでの作業でエラーが発生する場合は、[リスト ビューを編集します](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。</span><span class="sxs-lookup"><span data-stu-id="1dbea-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="1dbea-115">次の 4 つの変更により、リスト ビューのしきい値エラーが削除されます。</span><span class="sxs-lookup"><span data-stu-id="1dbea-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="1dbea-116">4 つの変更をすべて行って、すべてのエラーを削除します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="1dbea-117">それでもエラーが発生する場合は、「[大規模なリストとライブラリ](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="1dbea-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="1dbea-118">[**最優先する列**] と [**2 番目に優先する列**] の両方から [**なし**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="1dbea-119">[**最優先する列**] と [**2 番目に優先する列**] の両方から [**なし**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="1dbea-120">[**合計**] セクションのすべての列で [**なし**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="1dbea-121">[**列**] セクションから表示する 1 列を除くすべての選択を解除します。</span><span class="sxs-lookup"><span data-stu-id="1dbea-121">Deselect all but one column for display from the **Columns** section.</span></span>

