---
title: ターミナル サーバーの Office 2019 または RDS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3487"
- "9001419"
ms.openlocfilehash: 3b61f0396c4698aaa54df74d6612d1a35d37f652
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790985"
---
# <a name="deploying-office-2019-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="bd9d1-102">RDS、ターミナル サーバー、または VDI で共有するための Office 2019 の導入</span><span class="sxs-lookup"><span data-stu-id="bd9d1-102">Deploying Office 2019 for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="bd9d1-103">他の Office プランを使用して Office が RDS サーバーに既にインストールされている場合には、アンインストールします。</span><span class="sxs-lookup"><span data-stu-id="bd9d1-103">If Office is already installed on the RDS server using any other Office plans, uninstall it.</span></span> <span data-ttu-id="bd9d1-104">たとえば、[**コントロール パネル**] >  [**プログラムのアンインストール**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="bd9d1-104">For example, go to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="bd9d1-105">問題が発生した場合には、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="bd9d1-105">If you're experiencing issues, uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy).</span></span> 

<span data-ttu-id="bd9d1-106">Office 展開ツール (ODT) を使用して Office をインストールします。</span><span class="sxs-lookup"><span data-stu-id="bd9d1-106">Use the Office Deployment Tool (ODT) to install Office.</span></span> <span data-ttu-id="bd9d1-107">詳細な手順については、「[Office 2019 を展開する](https://docs.microsoft.com/deployoffice/office2019/deploy)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd9d1-107">For detailed steps, see [Deploy Office 2019](https://docs.microsoft.com/deployoffice/office2019/deploy).</span></span>

<span data-ttu-id="bd9d1-108">ライセンス認証の詳細については、「[Office のボリューム ライセンス認証の概要](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd9d1-108">For activation, see [Overview of volume activation of Office](https://docs.microsoft.com/deployoffice/vlactivation/plan-volume-activation-of-office).</span></span>