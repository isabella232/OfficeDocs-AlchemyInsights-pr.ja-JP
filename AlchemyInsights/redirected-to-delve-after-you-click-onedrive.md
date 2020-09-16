---
title: OneDrive for Business Web OneDrive を Delve にリダイレクトする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776384"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="187c6-102">[OneDrive] をクリックした後、Delve にリダイレクトされる</span><span class="sxs-lookup"><span data-stu-id="187c6-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="187c6-103">詳細については、「[トラブルシューティング ガイド](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="187c6-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="187c6-104">この問題を解決するには、管理者は、ユーザーに [個人用サイト] サイトを作成する権限を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="187c6-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="187c6-105">これは、OneDrive for Business ページが個人用サイトに作成されているためです。</span><span class="sxs-lookup"><span data-stu-id="187c6-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="187c6-106">この権限を付与するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="187c6-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="187c6-107">SharePoint 管理センターで、[**ユーザー プロファイル**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="187c6-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="187c6-108">[**ひと**] セクションで、 [**ユーザー権限の管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="187c6-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="187c6-109">[個人用サイト] サイトを作成する権限を必要とするユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="187c6-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="187c6-110">既定では、この設定は [**外部ユーザー以外のすべてのユーザー**] に設定されます。</span><span class="sxs-lookup"><span data-stu-id="187c6-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="187c6-111">ユーザー、複数のユーザー、またはグループを追加したら、追加したユーザー、複数のユーザー、またはグループが選択されていることを確認して、[**アクセス許可**] セクションまでスクロールして、[**個人用サイトの作成 (個人用ストレージ、ニュースフィード、およびフォローしたコンテンツ)**] の隣のチェック ボックスを選択します。</span><span class="sxs-lookup"><span data-stu-id="187c6-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="187c6-112">[**OK**] をクリックし、ユーザーに OneDrive ページに移動してサイトを作成してもらいます。</span><span class="sxs-lookup"><span data-stu-id="187c6-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
