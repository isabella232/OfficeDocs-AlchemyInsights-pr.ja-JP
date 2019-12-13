---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 621504f5b7170ff36ad093330b8a662e7222d1e7
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36754485"
---
# <a name="internal-server-error-when-navigating-to-sharepoint-or-onedrive-sites"></a><span data-ttu-id="a5e47-102">SharePoint サイトまたは OneDrive サイトへの移動時の内部サーバー エラー</span><span class="sxs-lookup"><span data-stu-id="a5e47-102">Internal server error when navigating to Sharepoint or OneDrive sites</span></span>

<span data-ttu-id="a5e47-103">ユーザーが SharePoint または OneDrive のサイトに移動しようとしたときに 500 内部サーバー エラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="a5e47-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="a5e47-104">ブラウザーのキャッシュをクリアしてから、サイトに移動してみてください。</span><span class="sxs-lookup"><span data-stu-id="a5e47-104">Please attempt to clear the browser cache before navigating to the site.</span></span>


1. <span data-ttu-id="a5e47-105">Microsoft Edge ブラウザーで、[その他...] > [設定] に移動します</span><span class="sxs-lookup"><span data-stu-id="a5e47-105">In the Microsoft Edge browser, go to More...> Settings</span></span>

2. <span data-ttu-id="a5e47-106">[閲覧データのクリア] で、**[クリアするデータの選択]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a5e47-106">Under Clear browsing, select Choose what to clear.</span></span>

3. <span data-ttu-id="a5e47-107">[Cookie と保存済みの Web サイト データ] チェック ボックスをオンにして、**[クリア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a5e47-107">Select Cookies and saved website data, and select Clear.</span></span>

<span data-ttu-id="a5e47-108">注: 別のブラウザー (Firefox や Chrome など) を使用している場合は、この手順とは異なることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5e47-108">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

<span data-ttu-id="a5e47-109">この方法で問題が解決しない場合は、[[メッセージ センター]](https://portal.office.com/adminportal/home#/MessageCenter) に移動して、テナントでアクティブ メンテナンスが実施されているかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a5e47-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

<span data-ttu-id="a5e47-110">最後に、[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)ページにアクセスして、発生している可能性のあるインシデント/アドバイザリを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a5e47-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

