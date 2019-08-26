---
title: SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620728"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="83702-102">SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合</span><span class="sxs-lookup"><span data-stu-id="83702-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="83702-103">ユーザーが SharePoint または OneDrive を次のシナリオで使用しようとすると、**メンテナンスのため読み取り専用**というメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="83702-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="83702-104">予定されていたまたは実行中のメンテナンス アクティビティ。</span><span class="sxs-lookup"><span data-stu-id="83702-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="83702-105">[メッセージ センター](https://portal.office.com/adminportal/home#/messagecenter)に移動して、これらについて確認してください。</span><span class="sxs-lookup"><span data-stu-id="83702-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="83702-106">発生中の可能性がある、優先度の高いアクティブなサービス インシデント。</span><span class="sxs-lookup"><span data-stu-id="83702-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="83702-107">[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)に移動して、アドバイザリおよびインシデントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="83702-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="83702-108">サーバー上での予期しないイベントが原因で発生中の可能性がある、継続時間が 30 分程度以内の軽微な自動復旧回復シナリオ。</span><span class="sxs-lookup"><span data-stu-id="83702-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="83702-109">これらの軽微な回復についてはメッセージ センターまたはサービス正常性に投稿されませんが、短時間で通常状態に回復します。</span><span class="sxs-lookup"><span data-stu-id="83702-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="83702-110">まれにですが、上記の 3 つのシナリオのいずれかが原因のケースで、サービスが回復したにも関わらずユーザーのブラウザーのキャッシュがクリアされないケースがあります。</span><span class="sxs-lookup"><span data-stu-id="83702-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="83702-111">ブラウザーのキャッシュをクリアしてから、サイトに移動してみてください。</span><span class="sxs-lookup"><span data-stu-id="83702-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="83702-112">Microsoft Edge ブラウザーで、[**設定**] を選択し、 [**プライバシーとセキュリティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="83702-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="83702-113">[**閲覧データの消去**] で、[**クリアするデータの選択**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="83702-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="83702-114">[**Cookies と保存済みの Web サイト データ**] を選択し、[**クリア**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="83702-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="83702-115">注: 他のブラウザー (Mozilla Firefox や Google Chrome など) を使用している場合は、この手順とは異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="83702-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="83702-116">別の方法としては、新しい InPrivate ウィンドウで SharePoint サイトまたは OneDrive を開くこともできます。</span><span class="sxs-lookup"><span data-stu-id="83702-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>