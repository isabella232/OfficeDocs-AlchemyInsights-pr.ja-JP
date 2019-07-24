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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840520"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="0a80b-102">SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合</span><span class="sxs-lookup"><span data-stu-id="0a80b-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="0a80b-103">ユーザーが SharePoint または OneDrive を使用しようとすると、**メンテナンスのため読み取り専用**というメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="0a80b-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="0a80b-104">これが表示された場合、[[メッセージ センター](https://portal.office.com/adminportal/home#/MessageCenter)] に移動して、テナントで進行中のメンテナンスがあるかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="0a80b-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="0a80b-105">また、[[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)] ダッシュボードを確認して、公開中のアドバイザリや発生中のインシデントがないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="0a80b-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="0a80b-106">[メッセージセンター] と [サービス正常性] ダッシュボードのどちらにも進行中のテナントのメンテナンスに関する情報がない場合、ブラウザー キャッシュの問題である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0a80b-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="0a80b-107">ブラウザーのキャッシュをクリアしてから、サイトに移動してみてください。</span><span class="sxs-lookup"><span data-stu-id="0a80b-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="0a80b-108">Microsoft Edge ブラウザーで、[**設定**] を選択し、 [**プライバシーとセキュリティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0a80b-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="0a80b-109">[**閲覧データの消去**] で、[**クリアするデータの選択**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0a80b-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="0a80b-110">[**Cookies と保存済みの Web サイト データ**] を選択し、[**クリア**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0a80b-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="0a80b-111">注: 他のブラウザー (Mozilla Firefox や Google Chrome など) を使用している場合は、この手順とは異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="0a80b-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="0a80b-112">別の方法としては、新しい InPrivate ウィンドウで SharePoint サイトまたは OneDrive を開くこともできます。</span><span class="sxs-lookup"><span data-stu-id="0a80b-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>