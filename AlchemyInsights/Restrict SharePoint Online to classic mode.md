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
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "31754854"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="4cef3-102">SharePoint Online のクラシック モードへの制限</span><span class="sxs-lookup"><span data-stu-id="4cef3-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="4cef3-103">いくつかの組織はまだクラシック モードのエクスペリエンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="4cef3-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="4cef3-104">クラシック モードを詳細なレベルで削除する計画はありませんが、2019 年 4 月 1 日からリストやライブラリに対して組織全体 (テナント) をクラシック モードに制限することはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="4cef3-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="4cef3-105">管理者には、次のレベルで提供される詳細なオプト アウト スイッチを使用して、クラシック モードで個々のリストとライブラリを管理する次のオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="4cef3-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="4cef3-106">-- サイト コレクション -- サイト -- リスト -- ライブラリ</span><span class="sxs-lookup"><span data-stu-id="4cef3-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="4cef3-107">さらに、modernでサポートされていない特定の機能やカスタマイズを使用しているリストは、自動的にクラシック モードに切り替わります。</span><span class="sxs-lookup"><span data-stu-id="4cef3-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="4cef3-108">4 月 1 日以降、テナントのオプト アウトの結果としてクラシック モードになっているリストとライブラリは、サイト レベルとリスト レベルで自動的に管理されます。</span><span class="sxs-lookup"><span data-stu-id="4cef3-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="4cef3-109">クラシック モードが必要な場合は、こちらの詳細情報と、4 月 1 日にテナント レベルのオプト アウト削除の準備をするために今日使用できるオプションとツールを説明している PnP Powershell の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4cef3-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
