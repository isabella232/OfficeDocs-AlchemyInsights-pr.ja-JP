---
title: Dynamics 365-Dynamics 365 の統合インターフェイスに正しくないダッシュボードが表示される
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528556"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="7f315-102">Dynamics 365 の統合インターフェイスに正しくないダッシュボードが表示される</span><span class="sxs-lookup"><span data-stu-id="7f315-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="7f315-103">必要なダッシュボードとは異なるダッシュボードが表示される理由はいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="7f315-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="7f315-104">ユーザーがユーザーの既定のダッシュボードを設定した</span><span class="sxs-lookup"><span data-stu-id="7f315-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="7f315-105">通常、ユーザーの既定のダッシュボードは、[既定の**設定**] ボタンがダッシュボードのコマンドバーに表示されない場合に設定できます。</span><span class="sxs-lookup"><span data-stu-id="7f315-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="7f315-106">ユーザーの既定のダッシュボードが現在のアプリにない場合でも、ユーザーの既定のダッシュボードは他のすべての既定のダッシュボードを上書きします。</span><span class="sxs-lookup"><span data-stu-id="7f315-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="7f315-107">次の回避策を使用して、既定のダッシュボードを未設定にします。</span><span class="sxs-lookup"><span data-stu-id="7f315-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="7f315-108">新しい個人ダッシュボードを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f315-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="7f315-109">新しいダッシュボードをユーザーの既定として設定します。</span><span class="sxs-lookup"><span data-stu-id="7f315-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="7f315-110">そのダッシュボードを削除します。</span><span class="sxs-lookup"><span data-stu-id="7f315-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="7f315-111">ダッシュボードは sitemap で設定されています。</span><span class="sxs-lookup"><span data-stu-id="7f315-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="7f315-112">ダッシュボードを選択し、[システムのカスタマイズ] の [既定として設定] を選択することにより、組織の既定のダッシュボードを設定した可能性があります。</span><span class="sxs-lookup"><span data-stu-id="7f315-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="7f315-113">しかし、ユーザーがアクセス権を持っている場合は、sitemap designer で定義されたダッシュボードがこのダッシュボードより優先されます。</span><span class="sxs-lookup"><span data-stu-id="7f315-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="7f315-114">組織の既定値として設定したダッシュボードがユーザーに表示されるようにするには、次のいずれかの方法を使用できます。</span><span class="sxs-lookup"><span data-stu-id="7f315-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="7f315-115">Sitemap でそのダッシュボードを設定する</span><span class="sxs-lookup"><span data-stu-id="7f315-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="7f315-116">これらのユーザーの sitemap 定義済みダッシュボードへのアクセスを削除する</span><span class="sxs-lookup"><span data-stu-id="7f315-116">Remove access to the sitemap defined dashboard for those users</span></span>
