---
title: データの場所
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207266"
---
# <a name="data-location"></a><span data-ttu-id="7eac3-102">データの場所</span><span class="sxs-lookup"><span data-stu-id="7eac3-102">Data location</span></span>

<span data-ttu-id="7eac3-103">Office 365 テナントの場所は管理センターで表示することも、PowerShell を使用して Exchange Online に接続して表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="7eac3-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="7eac3-104">**管理センター:**</span><span class="sxs-lookup"><span data-stu-id="7eac3-104">**Admin center**</span></span>
1. <span data-ttu-id="7eac3-105">[管理センター](https://admin.microsoft.com/Adminportal/Home)にログインします。</span><span class="sxs-lookup"><span data-stu-id="7eac3-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="7eac3-106">[**設定**]  >  [**組織プロファイル**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="7eac3-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="7eac3-107">[**データの場所**] で、[**詳細の表示**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7eac3-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="7eac3-108">**PowerShell:**</span><span class="sxs-lookup"><span data-stu-id="7eac3-108">**PowerShell**</span></span>
1. <span data-ttu-id="7eac3-109">Windows PowerShell を使用して Exchange Online に接続します。</span><span class="sxs-lookup"><span data-stu-id="7eac3-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="7eac3-110">[Get-OrganizationalUnit](https://docs.microsoft.com/ja-JP/powershell/module/exchange/active-directory/get-organizationalunit) コマンドレットを実行してテナントのプロパティの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="7eac3-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/ja-JP/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="7eac3-111">"OrganizationId" プロパティを確認します。</span><span class="sxs-lookup"><span data-stu-id="7eac3-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="7eac3-112">EXO および SPO のデータの場所がわかれば、[データが格納されている場所](https://products.office.com/where-is-your-data-located)から使用する他のサービスのデータの場所を特定できます。</span><span class="sxs-lookup"><span data-stu-id="7eac3-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>