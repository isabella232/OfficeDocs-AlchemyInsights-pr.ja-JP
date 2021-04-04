---
title: ドメインに参加しているデバイスの既定のブラウザーとして Microsoft Edge を設定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2021
ms.locfileid: "51492343"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="289db-102">ドメインに参加しているデバイスの既定のブラウザーとして Microsoft Edge を設定する</span><span class="sxs-lookup"><span data-stu-id="289db-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="289db-103">以下の手順で、Microsoft Edge を既定のブラウザーとして設定します。</span><span class="sxs-lookup"><span data-stu-id="289db-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="289db-104">[既定のアソシエーション構成ファイルを作成](https://go.microsoft.com/fwlink/?linkid=2132437)し、ローカルまたはネットワーク共有に保存します。</span><span class="sxs-lookup"><span data-stu-id="289db-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="289db-105">グループ ポリシー エディターを開き、**[コンピューターの構成]** > **[管理用テンプレート]** > **[Windows コンポーネント]** > **[ファイル エクスプローラー]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="289db-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="289db-106">[**既定の関連付け構成ファイルを設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="289db-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="289db-107">**[ポリシー設定]** を選択し、**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="289db-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="289db-108">**[オプション]** で、デフォルトの関連付け構成ファイルの場所を入力し、**[OK]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="289db-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
