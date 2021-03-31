---
title: 夜間モードの表示設定を支援する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405801"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="77f28-102">夜間モードの表示設定を支援する</span><span class="sxs-lookup"><span data-stu-id="77f28-102">Help with the night light display setting</span></span>

<span data-ttu-id="77f28-103">夜間ディスプレイ設定の詳細については、「[Windows 10 でディスプレイを夜間用に設定する](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77f28-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="77f28-104">[設定] で夜間モードのオプションがグレー表示されている場合は、ディスプレイ ドライバを確認してください。</span><span class="sxs-lookup"><span data-stu-id="77f28-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="77f28-105">タスク バーの検索ボックスに「**デバイス マネージャー**」と入力し、検索結果のリストから [**デバイス マネージャー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="77f28-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="77f28-106">[**ディスプレイ アダプタ**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="77f28-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="77f28-107">残念ながら、デバイスが DisplayLink ドライバーまたは Basic Display ドライバーを使用している場合、夜間モード機能は使用できません。</span><span class="sxs-lookup"><span data-stu-id="77f28-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="77f28-108">夜間モード機能は最新のグラフィック テクノロジーを利用しているため、ディスプレイ ドライバーを更新する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="77f28-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="77f28-109">**[スタート]** > **[設定]** > **[更新とセキュリティ]** > **[Windows Update]** > **[更新の確認]** に移動して、更新を確認します。</span><span class="sxs-lookup"><span data-stu-id="77f28-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="77f28-110">または</span><span class="sxs-lookup"><span data-stu-id="77f28-110">OR</span></span>

- <span data-ttu-id="77f28-111">ハードウェア メーカーのサポート Web サイトにアクセスして、最新のディスプレイ ドライバーを手動でダウンロードしてインストールします。</span><span class="sxs-lookup"><span data-stu-id="77f28-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="77f28-112">レジストリの夜間モードをリセットする</span><span class="sxs-lookup"><span data-stu-id="77f28-112">Reset night light in the registry</span></span>

<span data-ttu-id="77f28-113">ディスプレイ ドライバの更新が機能しなかった場合は、レジストリの夜間モードをリセットする必要があるかもしれません。</span><span class="sxs-lookup"><span data-stu-id="77f28-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="77f28-114">**注意:** このトラブルシューティング手順は、上級ユーザーにのみお勧めします。</span><span class="sxs-lookup"><span data-stu-id="77f28-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="77f28-115">レジストリを誤って変更すると、重大な問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="77f28-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="77f28-116">保護を強化するには、レジストリを変更する前にバックアップして、問題が発生した場合にレジストリを復元できるようにします。</span><span class="sxs-lookup"><span data-stu-id="77f28-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="77f28-117">検索ボックスに「**regedit**」と入力し、検索結果で [**レジストリ エディタ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="77f28-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="77f28-118">次のレジストリ キーに移動します。</span><span class="sxs-lookup"><span data-stu-id="77f28-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="77f28-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="77f28-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="77f28-120">次のサブキーをエクスポートしてから削除します: $$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="77f28-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="77f28-121">次のサブキーをエクスポートしてから削除します：$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="77f28-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="77f28-122">Windows を再起動し、常夜灯のオプションが利用可能かどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="77f28-122">Restart Windows and verify if the night light options are available.</span></span>


