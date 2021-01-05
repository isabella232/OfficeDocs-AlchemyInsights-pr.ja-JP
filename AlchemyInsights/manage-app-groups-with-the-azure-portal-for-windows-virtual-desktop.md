---
title: Windows Virtual Desktop 用の Azure portal を使用してアプリ グループを管理する
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722211"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="2cbb2-102">Windows Virtual Desktop 用の Azure portal を使用してアプリ グループを管理する</span><span class="sxs-lookup"><span data-stu-id="2cbb2-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="2cbb2-103">Windows Virtual Desktop の新しいホスト プール向けに作成される既定のアプリ グループには、完全なデスクトップも公開されています。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="2cbb2-104">さらに、Azure portal を使用して、ホスト プールに 1 つ以上の RemoteApp アプリ グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="2cbb2-105">展開プロセストにより、以下の処理が実行されます。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="2cbb2-106">RemoteApp アプリ グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="2cbb2-107">選択したアプリをアプリ グループに追加します。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="2cbb2-108">個々のユーザーまたはユーザー グループをアプリ グループに公開します。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="2cbb2-109">必要に応じて、アプリ グループを登録します。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="2cbb2-110">構成に応じて Azure Resource Manager テンプレートへのリンクを作成します。これにより、テンプレートをダウンロードして保存できます。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="2cbb2-111">Windows Virtual Desktop 用の RemoteApp グループを作成するには、「[Azure portal を使用してアプリ グループを管理する](https://go.microsoft.com/fwlink/?linkid=2129550)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="2cbb2-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
