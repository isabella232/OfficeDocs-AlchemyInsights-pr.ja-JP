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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701288"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="8f708-102">Intune からのデータの削除とデバイスのワイプ</span><span class="sxs-lookup"><span data-stu-id="8f708-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="8f708-103">Device Retire およびDevice Wipe リモートアクションを使用して、Intune が管理する会社データを削除したり、デバイスを出荷時設定にリセットして既定の設定に戻すことができます。</span><span class="sxs-lookup"><span data-stu-id="8f708-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="8f708-104">Microsoft 365 Device Management にサインインし、**デバイス**の > **すべてのデバイス**に移動します。</span><span class="sxs-lookup"><span data-stu-id="8f708-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="8f708-105">ワイプを実行するデバイスを選びます。</span><span class="sxs-lookup"><span data-stu-id="8f708-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="8f708-106">実行するリモートワイプのタイプを選択します。</span><span class="sxs-lookup"><span data-stu-id="8f708-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="8f708-107">破棄を行うと組織情報のみが削除されますが、フルワイプを実行すると、デバイスは工場出荷時の設定に戻ります。</span><span class="sxs-lookup"><span data-stu-id="8f708-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="8f708-108">[**はい**] を選択して確認します。</span><span class="sxs-lookup"><span data-stu-id="8f708-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="8f708-109">ワイプが完了するまで、デバイスのアクションステータスは [破棄の保留中] と表示されます。</span><span class="sxs-lookup"><span data-stu-id="8f708-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="8f708-110">アクションが完了すると、管理対象デバイスのリストにモバイルデバイスが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="8f708-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="8f708-111">**注:** 会社のデータを Azure AD に結合されたデバイスから削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="8f708-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="8f708-112">何が保持され何が削除されるかなど、破棄およびワイプ アクションの効果の詳細については、「[ワイプを使用してデバイスを削除、破棄、または手動でデバイスの登録を解除する](https://docs.microsoft.com/intune/devices-wipe)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f708-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="8f708-113">MacOS デバイスのすべてのデータを消去する場合は、「[MacOS デバイスからすべてのデータを削除する](https://docs.microsoft.com/intune/device-erase)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f708-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>