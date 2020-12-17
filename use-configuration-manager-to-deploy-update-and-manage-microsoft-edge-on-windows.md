---
title: Configuration Manager を使用して Windows 上の Microsoft Edge を展開、更新、および管理する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004030"
- "7100"
ms.openlocfilehash: 8987a37a1e756001c45e9407337543d70560e314
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680463"
---
# <a name="use-configuration-manager-to-deploy-update-and-manage-microsoft-edge-on-windows"></a><span data-ttu-id="d5d6d-102">Configuration Manager を使用して Windows 上の Microsoft Edge を展開、更新、および管理する</span><span class="sxs-lookup"><span data-stu-id="d5d6d-102">Use Configuration Manager to deploy, update, and manage Microsoft Edge on Windows</span></span>

<span data-ttu-id="d5d6d-103">Configuration Manager バージョン1910の場合、PowerShell スクリプトを使用して、Microsoft Edge (バージョン77以降) を展開できます。</span><span class="sxs-lookup"><span data-stu-id="d5d6d-103">As of Configuration Manager version 1910, you can deploy Microsoft Edge (versions 77 and later) through a PowerShell script.</span></span> <span data-ttu-id="d5d6d-104">スクリプトは自動更新をオフにします。これにより、Configuration Manager で更新プログラムを管理できます。</span><span class="sxs-lookup"><span data-stu-id="d5d6d-104">The script turns off automatic updates, and this lets you manage the updates through Configuration Manager.</span></span> <span data-ttu-id="d5d6d-105">この機能や Configuration Manager を使用したその他の利点の詳細情報は、[Microsoft Edge 管理](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge??) を参照します。</span><span class="sxs-lookup"><span data-stu-id="d5d6d-105">To learn more about this and other benefits of using Configuration Manager, see [Microsoft Edge Management](https://docs.microsoft.com/mem/configmgr/apps/deploy-use/deploy-edge??).</span></span>