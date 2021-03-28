---
title: Yammer 管理者について
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038355"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="9eacd-102">Yammer 管理者について</span><span class="sxs-lookup"><span data-stu-id="9eacd-102">About Yammer admins</span></span>

<span data-ttu-id="9eacd-103">**ネットワーク管理者**</span><span class="sxs-lookup"><span data-stu-id="9eacd-103">**Network admins**</span></span>

<span data-ttu-id="9eacd-104">グローバル管理者は Yammer ネットワークの認証管理者の役割に自動的に昇格します。</span><span class="sxs-lookup"><span data-stu-id="9eacd-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="9eacd-105">次の場合、この昇格が正しく行われません。</span><span class="sxs-lookup"><span data-stu-id="9eacd-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="9eacd-106">複数の Yammer ネットワークが存在し、管理者が間違ったネットワークにサインインしている。</span><span class="sxs-lookup"><span data-stu-id="9eacd-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="9eacd-107">1 つの Yammer ネットワークに到達するには、[ネットワークの統合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9eacd-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="9eacd-108">Azure PIM が使用されています。</span><span class="sxs-lookup"><span data-stu-id="9eacd-108">Azure PIM is being used.</span></span> <span data-ttu-id="9eacd-109">ユーザーがグローバル管理者に昇格するまでに、長く時間が必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="9eacd-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="9eacd-110">Yammer の今後の更新でこの問題が解決される場合がありますが、ユーザーのグローバル管理者への昇格は手動で行うのが最善です。</span><span class="sxs-lookup"><span data-stu-id="9eacd-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="9eacd-111">Yammer ネットワークに同期の問題があります。</span><span class="sxs-lookup"><span data-stu-id="9eacd-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="9eacd-112">この場合、さらに調査するためにはサポートの依頼が必要になります。</span><span class="sxs-lookup"><span data-stu-id="9eacd-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="9eacd-113">Yammer 管理者の役割の詳細については、「[Yammer の管理者の役割を管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9eacd-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="9eacd-114">**グループ管理者**</span><span class="sxs-lookup"><span data-stu-id="9eacd-114">**Group admins**</span></span>

<span data-ttu-id="9eacd-115">Microsoft 365 に接続されているグループのグループ管理者は、Azure AD のグループ メンバーシップと同期されます。</span><span class="sxs-lookup"><span data-stu-id="9eacd-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="9eacd-116">大規模なグループの場合、この同期が長期間におよぶ場合があります。</span><span class="sxs-lookup"><span data-stu-id="9eacd-116">For large groups, this sync can take an extended period.</span></span>
