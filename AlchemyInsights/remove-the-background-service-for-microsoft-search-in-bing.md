---
title: Bing での Microsoft Search のバックグラウンド サービスを削除する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816526"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="20534-102">Bing での Microsoft Search のバックグラウンド サービスを削除する</span><span class="sxs-lookup"><span data-stu-id="20534-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="20534-103">Bing での Microsoft Search のバックグラウンド サービスを削除するには、次の対処法を試すことができます。</span><span class="sxs-lookup"><span data-stu-id="20534-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="20534-104">検索エンジンの設定を元に戻すには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="20534-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="20534-105">a.</span><span class="sxs-lookup"><span data-stu-id="20534-105">a.</span></span> <span data-ttu-id="20534-106">**Bing を既定の検索エンジンとして使用する[トグルを](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)オフ** に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="20534-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="20534-107">b.</span><span class="sxs-lookup"><span data-stu-id="20534-107">b.</span></span> <span data-ttu-id="20534-108">[Microsoft 365 管理センターに移動](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)し、組織内の全ユーザーに影響する設定を解除します。</span><span class="sxs-lookup"><span data-stu-id="20534-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="20534-109">個人のデバイスからバックグラウンド サービスを削除するには、次のタスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="20534-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="20534-110">a.</span><span class="sxs-lookup"><span data-stu-id="20534-110">a.</span></span> <span data-ttu-id="20534-111">**[コントロール パネル] > [プログラム] > [プログラムと機能]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="20534-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="20534-112">b.</span><span class="sxs-lookup"><span data-stu-id="20534-112">b.</span></span> <span data-ttu-id="20534-113">現在インストールされているプログラムのリストで、**[Bing での Microsoft Search]**] を右クリックし、**[アンインストール]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="20534-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="20534-114">組織内の複数のデバイスからバックグラウンド サービスを削除するには、管理者としてログインし、スクリプトで次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="20534-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
