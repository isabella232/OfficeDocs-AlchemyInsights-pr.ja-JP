---
title: リスト アイテムへのコメント
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982625"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="38fc8-102">リスト アイテムへのコメント</span><span class="sxs-lookup"><span data-stu-id="38fc8-102">Comments on List items</span></span>

<span data-ttu-id="38fc8-103">ユーザーはまもなくリスト アイテムへのコメントを追加したり削除したりできるようになります。</span><span class="sxs-lookup"><span data-stu-id="38fc8-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="38fc8-104">ユーザーは、リスト アイテムのすべてのコメントを表示し、アイテムに関連するコメントまたはアクティビティを表示するビューをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="38fc8-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="38fc8-105">**時期**:</span><span class="sxs-lookup"><span data-stu-id="38fc8-105">**Timing**:</span></span>

<span data-ttu-id="38fc8-106">**対象指定リリース**: 10 月中旬に段階的に展開し、11 月中旬までに完了する予定</span><span class="sxs-lookup"><span data-stu-id="38fc8-106">**Targeted release**: Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="38fc8-107">**標準リリース**: 11 月中旬に段階的に展開し、12 月上旬までに完了する予定</span><span class="sxs-lookup"><span data-stu-id="38fc8-107">**Standard release**: Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="38fc8-108">**展開**: 組織全体の対象指定リリース</span><span class="sxs-lookup"><span data-stu-id="38fc8-108">**Rollout**: Targeted release for the entire organization</span></span>

<span data-ttu-id="38fc8-109">ユーザーは、コメントを追加および削除する前に、次の点に注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="38fc8-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="38fc8-110">コメントは、SharePoint 固有の権限設定に従います。</span><span class="sxs-lookup"><span data-stu-id="38fc8-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="38fc8-111">タスク リストのように、最新のユーザー インターフェイスに表示されるようにまだ構築されていない従来のリストには、このコメント機能はありません。</span><span class="sxs-lookup"><span data-stu-id="38fc8-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="38fc8-112">このリリースでは、Teams 内のリストにコメントすることはできません。</span><span class="sxs-lookup"><span data-stu-id="38fc8-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="38fc8-113">コメントは検索によってインデックス化されません。</span><span class="sxs-lookup"><span data-stu-id="38fc8-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="38fc8-114">管理者は、**Set-SPOTenant** PowerShell コマンドレットの **CommentsOnListItemsDisabled** パラメータを変更して、組織レベルでこの機能を無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="38fc8-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="38fc8-115">現在、サイト レベルまたはリスト レベルでコメントを無効にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="38fc8-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="38fc8-116">これらのコントロールは、おそらく 2021 年第 1 四半期に更新される予定です。</span><span class="sxs-lookup"><span data-stu-id="38fc8-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
