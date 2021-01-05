---
title: Microsoft Edge で Azure 機能が正常に機能しない場合の対処方法
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584200"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="3315c-102">Microsoft Edge で Azure 機能が正常に機能しない場合の対処方法</span><span class="sxs-lookup"><span data-stu-id="3315c-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="3315c-103">Microsoft Edge には、セキュリティ ゾーンに関連する[既知の問題](https://go.microsoft.com/fwlink/?linkid=2140608)があり、Azure ユーザーが Windows Admin Center にログインする方法に影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3315c-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="3315c-104">Microsoft Edge で Azure 機能を使用する際に問題が発生した場合は、次の手順を試してください。</span><span class="sxs-lookup"><span data-stu-id="3315c-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="3315c-105">**[スタート]** メニューで、**[インターネット オプション]** を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="3315c-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="3315c-106">**[プロパティ]** ダイアログ ボックスで **[セキュリティ]** タブに移動します。</span><span class="sxs-lookup"><span data-stu-id="3315c-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="3315c-107">**[信頼済みサイト]** ゾーンを選択してから、**[サイト]** ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="3315c-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="3315c-108">**[信頼済みサイト]** ダイアログ ボックスで、ゲートウェイ URL と [https://login.microsoftonline.com](https://login.microsoftonline.com) および [https://login.live.com](https://login.live.com) を追加し、**[閉じる]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3315c-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="3315c-109">**[インターネット プロパティ]** ダイアログ ボックスで、**[プライバシー]** タブをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3315c-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="3315c-110">**[ポップアップ ブロック]** セクションで、**[設定]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3315c-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="3315c-111">表示されたダイアログ ボックスで、ゲートウェイ URL と [https://login.microsoftonline.com](https://login.microsoftonline.com) および [https://login.live.com](https://login.live.com) を追加し、**[閉じる]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3315c-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
