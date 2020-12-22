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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724159"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="b0818-102">リスト アイテムへのコメント</span><span class="sxs-lookup"><span data-stu-id="b0818-102">Comments on List items</span></span>

<span data-ttu-id="b0818-103">ユーザーは、リスト アイテムのすべてのコメントを表示し、アイテムに関連するコメントまたはアクティビティを表示するビューをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="b0818-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="b0818-104">ユーザーは、コメントを追加および削除する前に、次の点に注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0818-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="b0818-105">コメントは、SharePoint 固有の権限設定に従います。</span><span class="sxs-lookup"><span data-stu-id="b0818-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="b0818-106">タスク リストのように、最新のユーザー インターフェイスに表示されるようにまだ構築されていない従来のリストには、このコメント機能はありません。</span><span class="sxs-lookup"><span data-stu-id="b0818-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="b0818-107">このリリースでは、Teams 内のリストにコメントすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b0818-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="b0818-108">コメントは検索によってインデックス化されません。</span><span class="sxs-lookup"><span data-stu-id="b0818-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="b0818-109">管理者は、**Set-SPOTenant** PowerShell コマンドレットの **CommentsOnListItemsDisabled** パラメータを変更して、組織レベルでこの機能を無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b0818-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="b0818-110">現在、サイト レベルまたはリスト レベルでコメントを無効にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b0818-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="b0818-111">これらのコントロールは、おそらく 2021 年第 1 四半期に更新される予定です。</span><span class="sxs-lookup"><span data-stu-id="b0818-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
