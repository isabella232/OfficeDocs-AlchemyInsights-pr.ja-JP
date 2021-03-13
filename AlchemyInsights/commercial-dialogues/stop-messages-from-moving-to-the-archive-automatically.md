---
title: メッセージのアーカイブへの移動を自動的に停止する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751357"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="49b77-102">メッセージのアーカイブへの移動を自動的に停止する</span><span class="sxs-lookup"><span data-stu-id="49b77-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="49b77-103">アイテム保持ポリシーを使用している場合は、そのポリシーの保持の有効期限を変更して、メッセージが自動的にアーカイブされないようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="49b77-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="49b77-104">次の操作を実行してください。</span><span class="sxs-lookup"><span data-stu-id="49b77-104">Here's how:</span></span>

1. <span data-ttu-id="49b77-105">[Exchange 管理センター](https://go.microsoft.com/fwlink/?linkid=2059104)で、**[コンプライアンス管理]**、 > **[保持タグ]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="49b77-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="49b77-106">[アーカイブ保持タグに移動する] を検索します。</span><span class="sxs-lookup"><span data-stu-id="49b77-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="49b77-107">保持タグで、保持期間 (アーカイブ期間) を **[なし]** に変更して、アイテム保持ポリシーにアイテムが自動的にアーカイブされないようにします。</span><span class="sxs-lookup"><span data-stu-id="49b77-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="49b77-108">これにより、この保持タグが適用されているすべてのメールボックスのアーカイブ設定が変更されます。</span><span class="sxs-lookup"><span data-stu-id="49b77-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
