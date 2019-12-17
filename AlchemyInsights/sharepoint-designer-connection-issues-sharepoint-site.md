---
title: SharePoint Designer の接続に関する問題
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051718"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="e5bb6-102">SharePoint Designer の接続に関する問題</span><span class="sxs-lookup"><span data-stu-id="e5bb6-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="e5bb6-103">SharePoint Designer で SharePoint サイトへの接続に問題が発生した場合は、次の一般的な解決方法を試してください。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="e5bb6-104">手順 1: [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) および [SharePoint Designer 2013 の 2016 年 8 月 2 日の更新プログラム](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)を使用して SharePoint Designer 2013 が更新済みであることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="e5bb6-105">手順 2: ローカル キャッシュ ファイルをクリアします。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="e5bb6-106">SharePoint Designer 2013 を閉じます。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="e5bb6-107">ローカル コンピューターで、次の各フォルダーに含まれるファイルをすべて削除します。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="e5bb6-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="e5bb6-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="e5bb6-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="e5bb6-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="e5bb6-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="e5bb6-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="e5bb6-111">SharePoint Designer 2013 を開いてもう一度アカウントにサインインし、動作を確認します。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="e5bb6-112">手順 3: [Windows デバイスの Office 2013 の先進認証を有効にします](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="e5bb6-113">手順 4: SharePoint Designer の接続を可能にするために、管理者は SharePoint 管理センターの設定で、**カスタム スクリプトの実行を許可**する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="e5bb6-114">詳細については、「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5bb6-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


