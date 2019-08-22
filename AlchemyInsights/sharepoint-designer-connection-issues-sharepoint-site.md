---
title: SharePoint Designer の接続の問題
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508428"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="ffb67-102">SharePoint Designer の接続の問題</span><span class="sxs-lookup"><span data-stu-id="ffb67-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="ffb67-103">Sharepoint Designer で SharePoint サイトへの接続に関する問題が発生している場合は、次の一般的なソリューションを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="ffb67-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="ffb67-104">手順 1: sharepoint designer 2013 が sharepoint designer [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)に更新されていること、および sharepoint [Designer 2013 の更新プログラム (2016 年8月2日)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)を更新していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ffb67-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="ffb67-105">手順 2: ローカルキャッシュファイルを消去します。</span><span class="sxs-lookup"><span data-stu-id="ffb67-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="ffb67-106">SharePoint Designer 2013 を閉じます。</span><span class="sxs-lookup"><span data-stu-id="ffb67-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="ffb67-107">ローカルコンピューターで、次の各フォルダーにあるすべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="ffb67-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="ffb67-108">%APPDATA%\Microsoft\Web サーバーの Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="ffb67-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="ffb67-109">%APPDATA%\Microsoft\SharePoint デザイナ \ proxyassemblycache</span><span class="sxs-lookup"><span data-stu-id="ffb67-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="ffb67-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="ffb67-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="ffb67-111">SharePoint Designer 2013 を開き、もう一度アカウントを入力して、正常に動作するかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="ffb67-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="ffb67-112">手順 3: [Windows デバイスで Office 2013 の先進認証を有効に](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)します。</span><span class="sxs-lookup"><span data-stu-id="ffb67-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="ffb67-113">手順 4: 管理者は、sharepoint 管理センターの設定で**カスタムスクリプトを許可**して、sharepoint Designer 接続を許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffb67-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="ffb67-114">詳細について[は、「カスタムスクリプトを許可または禁止](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffb67-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


