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
ms.openlocfilehash: c51e48fe5694f964aef74c2973f774b44415ebb8
ms.sourcegitcommit: 21cfb213183188d32a3743f66db10a8463019965
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2019
ms.locfileid: "31754856"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="c123b-102">SharePoint Online のクラシック モードへの制限</span><span class="sxs-lookup"><span data-stu-id="c123b-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="c123b-103">いくつかの組織はまだクラシック モードのエクスペリエンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="c123b-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="c123b-104">クラシック モードを詳細なレベルで削除する計画はありませんが、2019 年 4 月 1 日からリストやライブラリに対して組織全体 (テナント) をクラシック モードに制限することはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="c123b-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="c123b-105">管理者には、次のレベルで提供される詳細なオプト アウト スイッチを使用して、クラシック モードで個々のリストとライブラリを管理する次のオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="c123b-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="c123b-106">サイト コレクション</span><span class="sxs-lookup"><span data-stu-id="c123b-106">site collection</span></span>
- <span data-ttu-id="c123b-107">サイト</span><span class="sxs-lookup"><span data-stu-id="c123b-107">Site</span></span>
- <span data-ttu-id="c123b-108">リスト</span><span class="sxs-lookup"><span data-stu-id="c123b-108">list</span></span>
- <span data-ttu-id="c123b-109">ライブラリ</span><span class="sxs-lookup"><span data-stu-id="c123b-109">Library</span></span>

<span data-ttu-id="c123b-110">さらに、modernでサポートされていない特定の機能やカスタマイズを使用しているリストは、自動的にクラシック モードに切り替わります。</span><span class="sxs-lookup"><span data-stu-id="c123b-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="c123b-111">4 月 1 日以降、テナントのオプト アウトの結果としてクラシック モードになっているリストとライブラリは、サイト レベルとリスト レベルで自動的に管理されます。</span><span class="sxs-lookup"><span data-stu-id="c123b-111">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="c123b-112">クラシック モードが必要な場合は、こちらの詳細情報と、4 月 1 日にテナント レベルのオプト アウト削除の準備をするために今日使用できるオプションとツールを説明している PnP Powershell の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c123b-112">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
