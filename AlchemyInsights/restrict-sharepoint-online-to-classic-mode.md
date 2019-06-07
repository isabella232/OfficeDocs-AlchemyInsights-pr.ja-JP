---
title: SharePoint Online のクラシック モードへの制限
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761764"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="fb1e3-102">SharePoint Online のクラシック モードへの制限</span><span class="sxs-lookup"><span data-stu-id="fb1e3-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="fb1e3-103">いくつかの組織はまだクラシック モードのエクスペリエンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="fb1e3-104">詳細なレベルでクラシックモードを削除する計画はありませんが、組織全体 (テナント) をリストとライブラリのクラシックモードに制限することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="fb1e3-105">管理者には、次のレベルで提供される詳細なオプト アウト スイッチを使用して、クラシック モードで個々のリストとライブラリを管理する次のオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="fb1e3-106">サイト コレクション</span><span class="sxs-lookup"><span data-stu-id="fb1e3-106">site collection</span></span>
- <span data-ttu-id="fb1e3-107">サイト</span><span class="sxs-lookup"><span data-stu-id="fb1e3-107">site</span></span>
- <span data-ttu-id="fb1e3-108">リスト</span><span class="sxs-lookup"><span data-stu-id="fb1e3-108">list</span></span>
- <span data-ttu-id="fb1e3-109">ライブラリ</span><span class="sxs-lookup"><span data-stu-id="fb1e3-109">library</span></span>

<span data-ttu-id="fb1e3-110">さらに、modernでサポートされていない特定の機能やカスタマイズを使用しているリストは、自動的にクラシック モードに切り替わります。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="fb1e3-111">2019年4月1日から、モダンリストとライブラリからのテナントレベルの脱退を無効にするプロセスが開始され、2019年5月31日から始まります。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="fb1e3-112">テナント脱退の結果としてクラシックモードになっているリストとライブラリは、自動的にモダンに移行されます。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="fb1e3-113">クラシックモードが必要な場合は、クラシック[](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023)モードを使用するため[](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout)に現在使用できるオプションとツールについて説明している「詳細情報」および「PnP Powershell 命令」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb1e3-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
