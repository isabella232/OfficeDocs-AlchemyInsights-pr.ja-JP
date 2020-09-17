---
title: ファイル オンデマンド
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804419"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="1b9a8-102">ファイル オンデマンドを構成する</span><span class="sxs-lookup"><span data-stu-id="1b9a8-102">Configure Files On-Demand</span></span>

<span data-ttu-id="1b9a8-103">OneDrive ファイル オンデマンド機能を利用すれば、OneDrive のファイルをすべてダウンロードし、デバイス上の記憶域を使用することなく、すべてのファイルにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="1b9a8-104">PC でファイル オンデマンドを構成するには:</span><span class="sxs-lookup"><span data-stu-id="1b9a8-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="1b9a8-105">Windows タスク バーの通知領域で、白または青の **OneDrive** クラウドのアイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="1b9a8-106">[**ヘルプと設定**] の歯車アイコン、[**設定**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="1b9a8-107">[**設定**] タブで、[**容量を節約し、ファイルを使用するときにダウンロード**] ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="1b9a8-108">レジストリを使用してファイル オンデマンドを構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="1b9a8-109">この設定を無効にした場合は、Windows 10 ユーザーは、以前のバージョンの Windows ユーザーと同じ同期動作となり、ファイル オンデマンドを有効にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="1b9a8-110">この設定を構成しなかった場合、ユーザーは、ファイル オンデマンドをオンまたはオフにすることができます。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="1b9a8-111">このポリシーを有効にすると、次のレジストリ キー値が 1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="1b9a8-112">このポリシーを無効にすると、次のレジストリ キーの値が 0 にセットされます。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="1b9a8-113">[設定] に [ファイル オンデマンド] オプションが表示されない場合は、サービスの [Windows クラウドのファイル フィルター ドライバー] の開始の種類が 2 (AUTO_START) に設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="1b9a8-114">このポリシーを有効にすると、次のレジストリ キー値が 2 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1b9a8-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`