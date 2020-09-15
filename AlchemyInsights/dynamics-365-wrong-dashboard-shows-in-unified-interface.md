---
title: Dynamics 365 - Dynamics 365 統合インターフェイスでの間違ったダッシュボードの表示
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711280"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="1323c-102">Dynamics 365 統合インターフェースで間違ったダッシュボードが表示される</span><span class="sxs-lookup"><span data-stu-id="1323c-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="1323c-103">想定と異なるダッシュボードが表示される理由はいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="1323c-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="1323c-104">ユーザーが自分のデフォルトのダッシュボードを設定した</span><span class="sxs-lookup"><span data-stu-id="1323c-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="1323c-105">通常、[**デフォルトに設定**] ボタンがダッシュボードのコマンド バーに表示されない場合は、ユーザーのデフォルト ダッシュボードが設定されていると認識できます。</span><span class="sxs-lookup"><span data-stu-id="1323c-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="1323c-106">ユーザーのデフォルト ダッシュボードが現在のアプリに含まれていない場合でも、ユーザーのデフォルト ダッシュボードは他のすべてのデフォルトのダッシュボードを上書きします。</span><span class="sxs-lookup"><span data-stu-id="1323c-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="1323c-107">デフォルトのダッシュボードの設定を解除するには、次の回避策を使用してください。</span><span class="sxs-lookup"><span data-stu-id="1323c-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="1323c-108">新しい個人用ダッシュボードを作成します。</span><span class="sxs-lookup"><span data-stu-id="1323c-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="1323c-109">新しいダッシュボードをユーザーのデフォルトとして設定します。</span><span class="sxs-lookup"><span data-stu-id="1323c-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="1323c-110">そのダッシュボードを削除します。</span><span class="sxs-lookup"><span data-stu-id="1323c-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="1323c-111">ダッシュボードがサイトマップに設定されている</span><span class="sxs-lookup"><span data-stu-id="1323c-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="1323c-112">ダッシュボードを選択し、 [システムのカスタマイズ] の下にある [デフォルトに設定] を選んで、組織のデフォルト ダッシュボードを設定したでしょうか。</span><span class="sxs-lookup"><span data-stu-id="1323c-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="1323c-113">ですが、ユーザーがアクセス権を持っている場合、サイトマップデザイナーで定義されているダッシュボードがこのダッシュボードよりも優先されます。</span><span class="sxs-lookup"><span data-stu-id="1323c-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="1323c-114">組織のデフォルトとして設定したダッシュボードをユーザーに表示させるには、次のいずれかの操作を行います。</span><span class="sxs-lookup"><span data-stu-id="1323c-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="1323c-115">そのダッシュボードをサイトマップに設定する</span><span class="sxs-lookup"><span data-stu-id="1323c-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="1323c-116">それらのユーザーのサイトマップ定義ダッシュボードへのアクセス権を削除する</span><span class="sxs-lookup"><span data-stu-id="1323c-116">Remove access to the sitemap defined dashboard for those users</span></span>
