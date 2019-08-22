---
title: Access services の廃止
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495756"
---
# <a name="access-services-retirement"></a><span data-ttu-id="67446-102">Access services の廃止</span><span class="sxs-lookup"><span data-stu-id="67446-102">Access services retirement</span></span>

<span data-ttu-id="67446-103">MC97576 で最初に発表されたように、2017年3月、年3月に、過去1年間のアクセスサービスは Office 365 から廃止されました。</span><span class="sxs-lookup"><span data-stu-id="67446-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="67446-104">このプロセスの次のフェーズでは、基になるデータストレージとして SharePoint リストを使用する Access Web データベースを削除します。</span><span class="sxs-lookup"><span data-stu-id="67446-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="67446-105">**どのような影響がありますか?**</span><span class="sxs-lookup"><span data-stu-id="67446-105">**How does this affect me?**</span></span>

<span data-ttu-id="67446-106">2019年6月以降、SharePoint Online の新しい Access データベースの作成を停止し、サービスおよび残りのアプリを4月2020にシャットダウンします。</span><span class="sxs-lookup"><span data-stu-id="67446-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="67446-107">**この変更を準備するために必要な作業**</span><span class="sxs-lookup"><span data-stu-id="67446-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="67446-108">組織の Access web データベースの移行計画を作成することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="67446-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="67446-109">管理者は、 [SharePoint access アプリスキャナー](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)を使用して、サイトが使用している access アプリのインベントリを取得できます。</span><span class="sxs-lookup"><span data-stu-id="67446-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="67446-110">Access web データベースのデータを移行するには、いくつかの方法があります。</span><span class="sxs-lookup"><span data-stu-id="67446-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="67446-111">ローカル Access データベース (にインポートします。ACCDB) または Excel ファイルにします。</span><span class="sxs-lookup"><span data-stu-id="67446-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="67446-112">また、web およびモバイルデバイス用のコードなしのビジネスソリューションを作成するための代替プラットフォームとして Microsoft PowerApps を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="67446-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>