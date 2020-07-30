---
title: 紛失した iOS デバイスを Intune で見つける
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440606"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="98892-102">紛失した iOS デバイスを Intune で見つける</span><span class="sxs-lookup"><span data-stu-id="98892-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="98892-103">iOS デバイスで紛失モードを有効にすると、管理者はロック画面にメッセージと連絡先の電話番号を表示できます。</span><span class="sxs-lookup"><span data-stu-id="98892-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="98892-104">紛失モードを有効にした後、管理者は [デバイスの検索] アクションを使用して、デバイスの物理的な場所を特定できます。</span><span class="sxs-lookup"><span data-stu-id="98892-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="98892-105">Intuneのデバイス検索アクションは iOS デバイス上で、特定のデバイスの場所を地図上に表示します。</span><span class="sxs-lookup"><span data-stu-id="98892-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="98892-106">このアクションを使用するには、iOS デバイスが次のいずれかの状態である必要があります。</span><span class="sxs-lookup"><span data-stu-id="98892-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="98892-107">監視モード</span><span class="sxs-lookup"><span data-stu-id="98892-107">Supervised mode</span></span>
- <span data-ttu-id="98892-108">紛失モード</span><span class="sxs-lookup"><span data-stu-id="98892-108">Lost mode</span></span>

<span data-ttu-id="98892-109">詳細については、[「 Intune で iOS / iPadOS デバイスで紛失モードを有効にする」](https://docs.microsoft.com/intune/device-lost-mode)および[「Intuneで紛失または盗難された iOS / iPadOS デバイスを特定する」](https://docs.microsoft.com/intune/device-locate)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98892-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="98892-110">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="98892-110">**FAQ**</span></span>

<span data-ttu-id="98892-111">Q：会社のデータをデバイスから削除するためのリモート アクションを発行しましたが、保留状態のままになっています。</span><span class="sxs-lookup"><span data-stu-id="98892-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="98892-112">A: リモート アクションを正常に完了するには、対象のデバイスがオンラインで正常である必要があります。</span><span class="sxs-lookup"><span data-stu-id="98892-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="98892-113">次のような状況では、リモート アクションは30日間、またはデバイスがコマンドを確認するまで保留状態になります。</span><span class="sxs-lookup"><span data-stu-id="98892-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="98892-114">デバイスが接続できない場合</span><span class="sxs-lookup"><span data-stu-id="98892-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="98892-115">デバイスで Intune の管理状態が解除された場合</span><span class="sxs-lookup"><span data-stu-id="98892-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="98892-116">デバイスがチェックインしておらず、会社のデータを削除できない場合は、[削除]を選択します。</span><span class="sxs-lookup"><span data-stu-id="98892-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="98892-117">削除すると、デバイスのレコードが削除され、デバイスの Intune リストに表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="98892-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="98892-118">デバイスが再びアクティブになった場合、そのユーザーはデバイスを再登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98892-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="98892-119">Q: 特定のリモート アクションを使用できないのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="98892-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="98892-120">A: すべてのプラットフォームがすべてのリモート デバイス アクションをサポートしているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="98892-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="98892-121">以下のリモートアクションはプラットフォーム固有であるため、記載されているプラットフォームでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="98892-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="98892-122">アクティベーション ロックのバイパス (iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="98892-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="98892-123">新たに開始 (Windows のみ)</span><span class="sxs-lookup"><span data-stu-id="98892-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="98892-124">ロスト モード (iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="98892-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="98892-125">デバイスの検索 (iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="98892-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="98892-126">再起動 (Windows のみ)</span><span class="sxs-lookup"><span data-stu-id="98892-126">Restart (Windows only)</span></span>

<span data-ttu-id="98892-127">各アクションの詳細については、[「使用可能なデバイス アクション」](https://docs.microsoft.com/intune/device-management#available-device-actions) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98892-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>