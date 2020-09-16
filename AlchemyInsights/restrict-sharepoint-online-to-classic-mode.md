---
title: SharePoint Online のクラシック モードへの制限
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751427"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="6f396-102">SharePoint Online のクラシック モードへの制限</span><span class="sxs-lookup"><span data-stu-id="6f396-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="6f396-103">いくつかの組織はまだクラシック モードのエクスペリエンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="6f396-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="6f396-104">クラシック モードを詳細なレベルで削除する計画はありませんが、リストやライブラリに対して組織全体 (テナント) をクラシック モードに制限することはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="6f396-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="6f396-105">管理者には、次のレベルで提供される詳細なオプト アウト スイッチを使用して、クラシック モードで個々のリストとライブラリを管理する次のオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="6f396-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="6f396-106">サイト コレクション</span><span class="sxs-lookup"><span data-stu-id="6f396-106">site collection</span></span>
- <span data-ttu-id="6f396-107">サイト</span><span class="sxs-lookup"><span data-stu-id="6f396-107">site</span></span>
- <span data-ttu-id="6f396-108">リスト</span><span class="sxs-lookup"><span data-stu-id="6f396-108">list</span></span>
- <span data-ttu-id="6f396-109">ライブラリ</span><span class="sxs-lookup"><span data-stu-id="6f396-109">library</span></span>

<span data-ttu-id="6f396-110">さらに、modernでサポートされていない特定の機能やカスタマイズを使用しているリストは、自動的にクラシック モードに切り替わります。</span><span class="sxs-lookup"><span data-stu-id="6f396-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="6f396-111">2019 年 4 月 1 日から、モダン リストおよびライブラリからオプトアウトするテナント レベルを無効にするプロセスが開始し、2019 年 5 月 31 日まで継続されます。</span><span class="sxs-lookup"><span data-stu-id="6f396-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="6f396-112">テナントのオプト アウトの結果としてクラシック モードのリストとライブラリは、自動的にモダンにシフトします。</span><span class="sxs-lookup"><span data-stu-id="6f396-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="6f396-113">クラシック モードが必要な場合は、クラシック モード エクスペリエンスの使用に今日用いることができるオプションとツールを説明する、「[こちら](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)」の詳細情報および「[こちら](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)」の PnP Powershell の手順をご参照ください。</span><span class="sxs-lookup"><span data-stu-id="6f396-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
