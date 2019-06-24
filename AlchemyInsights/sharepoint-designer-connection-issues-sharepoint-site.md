---
title: SharePoint Online のアクセス許可レベル
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35086087"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="2f772-102">SharePoint Designer の接続に関する問題</span><span class="sxs-lookup"><span data-stu-id="2f772-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="2f772-103">SharePoint Designer で SharePoint サイトへの接続に問題が発生した場合は、次の一般的な解決方法を試してください。</span><span class="sxs-lookup"><span data-stu-id="2f772-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="2f772-104">手順 1: SharePoint Designer が更新されていることを確認する。</span><span class="sxs-lookup"><span data-stu-id="2f772-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="2f772-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="2f772-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="2f772-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="2f772-106">SharePoint Server 2010 with Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="2f772-107">SharePoint Designer 2013 の更新プログラム (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="2f772-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="2f772-108">手順 2: ローカル キャッシュ ファイルをクリアする</span><span class="sxs-lookup"><span data-stu-id="2f772-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="2f772-109">SharePoint Designer 2013 を閉じます。</span><span class="sxs-lookup"><span data-stu-id="2f772-109">SharePoint Designer 2013</span></span>

- <span data-ttu-id="2f772-110">ローカル コンピューターで、次のフォルダーを参照してキャッシュされているファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="2f772-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="2f772-111">[スタート]、[実行] の順にクリックして、次の各場所にあるすべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="2f772-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="2f772-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="2f772-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="2f772-113">SharePoint Designer 2013 を開いて、動作を確認するために、もう一度アカウントを入力します。</span><span class="sxs-lookup"><span data-stu-id="2f772-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="2f772-114">手順 3: [Windows デバイスの Office 2013 の先進認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="2f772-114">[Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide) .</span></span>

<span data-ttu-id="2f772-115">手順 4: 管理者は SharePoint Designer の接続を可能にするカスタム スクリプトの実行を許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2f772-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="2f772-116">詳細な手順、例、および考慮事項については、「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f772-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


