---
title: DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353182"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="27a73-102">DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する</span><span class="sxs-lookup"><span data-stu-id="27a73-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="27a73-103">[ [ドメイン](https://portal.office.com/adminportal/home#/Domains) ] ページで、ドメインの一覧から、Web サイトで使用しているドメインを選択し、管理ウィンドウで [ **DNS 設定** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27a73-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="27a73-104">[**+ 新しいカスタム レコード**] を選択し、次を入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="27a73-105">[ **DNS の種類** ] には、「 **A (アドレス)** 」と入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="27a73-106">[ **ホスト名またはエイリアス** ] には、「 **@** 」と入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="27a73-107">[ **IP アドレス** ] には、Web サイトが現在ホストされている場所の静的 IP アドレス (たとえば、172.16.140.1) を入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="27a73-p101">これは、Web サイトの *動的*  IP アドレスではなく、  *静的*  IP アドレスでなければなりません。 Web サイトがホストされているサイトで、一般向け Web サイトの静的 IP アドレスを取得できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="27a73-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="27a73-110">[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27a73-110">Select **Save**.</span></span>

<span data-ttu-id="27a73-111">さらに、CNAME レコードを作成して、Web サイトを顧客が簡単に見つけることができるようにすることもできます。</span><span class="sxs-lookup"><span data-stu-id="27a73-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="27a73-112">[ **+ 新しいカスタム レコード** ] を選択し、次の項目を入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="27a73-113">[ **DNS の種類** ] には、「 **CNAME (エイリアス)** 」と入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="27a73-114">[ **ホスト名またはエイリアス** ] には、「 **www** 」と入力します。</span><span class="sxs-lookup"><span data-stu-id="27a73-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="27a73-115">[ **ポイント先のアドレス** ] には、Web サイトの完全修飾ドメイン名 (FQDN) を入力します (例: contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="27a73-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="27a73-116">[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27a73-116">Select **Save**.</span></span>
