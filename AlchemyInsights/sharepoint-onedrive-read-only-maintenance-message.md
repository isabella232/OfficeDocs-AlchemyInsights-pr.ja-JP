---
title: 127 メールにアクセスしようとしたときに TenantAccessBlockedException エラーが表示される場合
ms.author: kirks
author: Techwriter40
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
ms.openlocfilehash: 5613138e7613deb264a7ab2c966f8b9c4a24763d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "35174432"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="3f125-102">SharePoint または OneDrive を使用しようとした場合に、メンテナンスメッセージの読み取り専用にする</span><span class="sxs-lookup"><span data-stu-id="3f125-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="3f125-103">ユーザーが SharePoint または OneDrive を使用しようとすると、メンテナンスメッセージの読み取り専用のメッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f125-103">Users may receive a Read-Only for Maintenance message when attempting to use SharePoint or OneDrive.</span></span>

<span data-ttu-id="3f125-104">[メッセージセンター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブなメンテナンスが発生しているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="3f125-104">Check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="3f125-105">最後に、[[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)] ページにアクセスして、発生している可能性があるすべてのアドバイザリ/インシデントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="3f125-105">Finally, ensure you visit the[Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="3f125-106">メッセージセンターまたはサービス正常性ダッシュボードで、テナントの現在のメンテナンスについての情報がない場合は、ブラウザーのキャッシュの問題である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3f125-106">If neither the Message Center or Service Health Dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="3f125-107">サイトに移動する前に、ブラウザーのキャッシュをクリアしてください。</span><span class="sxs-lookup"><span data-stu-id="3f125-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

- <span data-ttu-id="3f125-108">Microsoft Edge ブラウザーで、[詳細設定] に移動します。</span><span class="sxs-lookup"><span data-stu-id="3f125-108">In the Microsoft Edge browser, go to More  Settings</span></span>

- <span data-ttu-id="3f125-109">[ブラウズをクリアする] で、[削除対象を選択する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3f125-109">Under Clear browsing, select Choose what to clear.</span></span>
- <span data-ttu-id="3f125-110">[Cookie と保存された web サイトデータ] チェックボックスをオンにして、[クリア] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3f125-110">Select the Cookies and saved website data check box and select Clear.</span></span>

<span data-ttu-id="3f125-111">**注**: Firefox や Chrome などの他のブラウザーを使用する場合、これらの手順は異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="3f125-111">**Note**: These steps may differ when using other browsers such as Firefox or Chrome.</span></span>

