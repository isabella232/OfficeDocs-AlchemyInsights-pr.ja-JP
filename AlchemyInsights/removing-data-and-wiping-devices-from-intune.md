---
title: Intune からのデータの削除とデバイスのワイプ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416318"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="bd8ee-102">Intune からのデータの削除とデバイスのワイプ</span><span class="sxs-lookup"><span data-stu-id="bd8ee-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="bd8ee-103">Device Retire およびDevice Wipe リモートアクションを使用して、Intune が管理する会社データを削除したり、デバイスを出荷時設定にリセットして既定の設定に戻すことができます。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="bd8ee-104">Microsoft 365 Device Management にサインインし、**デバイス** の > **すべてのデバイス** に移動します。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="bd8ee-105">ワイプを実行するデバイスを選びます。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="bd8ee-106">実行するリモートワイプのタイプを選択します。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="bd8ee-107">破棄を行うと組織情報のみが削除されますが、フルワイプを実行すると、デバイスは工場出荷時の設定に戻ります。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="bd8ee-108">[**はい**] を選択して確認します。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="bd8ee-109">ワイプが完了するまで、デバイスのアクションステータスは *[破棄の保留中]* と表示されます。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="bd8ee-110">アクションが完了すると、管理対象デバイスのリストにモバイルデバイスが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="bd8ee-111">会社のデータを Azure AD に結合されたデバイスから削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="bd8ee-112">何が保持され何が削除されるかなど、破棄およびワイプ アクションの効果の詳細については、以下のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="bd8ee-113">[ワイプ、インベントリからの削除、デバイス登録の手動解除を使用し、デバイスを削除する](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="bd8ee-114">Intune で管理されているアプリから会社のデータをワイプする方法</span><span class="sxs-lookup"><span data-stu-id="bd8ee-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="bd8ee-115">[MacOS デバイスからすべてのデータを削除する](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)。</span><span class="sxs-lookup"><span data-stu-id="bd8ee-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>