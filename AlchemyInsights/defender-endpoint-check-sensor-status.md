---
title: Defender Endpoint でセンサーの状態をチェックする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676598"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="0b71e-102">Defender Endpoint でセンサーの状態をチェックする</span><span class="sxs-lookup"><span data-stu-id="0b71e-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="0b71e-103">**センサーに問題のあるデバイス** タイルはセキュリティ運用ダッシュボードにあります。</span><span class="sxs-lookup"><span data-stu-id="0b71e-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="0b71e-104">このタイルは、センサー データを提供し、Defender for Endpoint サービスと通信する個々のデバイスの能力に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0b71e-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="0b71e-105">注意が必要なデバイスの数が報告され、問題のあるデバイスを特定し、既知の問題を修正するためのアクションを取るのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="0b71e-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="0b71e-106">タイル上の 2 つの状態インジケーターは、サービスに正しく報告していないデバイスの数に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0b71e-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="0b71e-107">**間違った構成** Defender for Endpoint サービスにセンサー データを部分的に報告している可能性があるデバイスに、修正が必要な構成エラーがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0b71e-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="0b71e-108">**非アクティブ** 過去 1 か月間で 7 日以上、Defender for Endpoint サービスへの報告が停止したデバイス。</span><span class="sxs-lookup"><span data-stu-id="0b71e-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="0b71e-109">いずれかのグループをクリックすると、選択した内容に応じてフィルター処理されたデバイスの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0b71e-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="0b71e-110">デバイス リストでは、以下の状態で正常性状態の一覧をいるター処理できます。</span><span class="sxs-lookup"><span data-stu-id="0b71e-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="0b71e-111">**アクティブ** Defender for Endpoint サービスにアクティブに報告しているデバイス。</span><span class="sxs-lookup"><span data-stu-id="0b71e-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="0b71e-112">**間違った構成** デバイスが Defender for Endpoint サービスにセンサー データを部分的に報告している場合でも、修正が必要な構成エラーがある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0b71e-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="0b71e-113">間違って構成されたデバイスには、次のような問題のいずれかまたは組み合わせがあります。</span><span class="sxs-lookup"><span data-stu-id="0b71e-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="0b71e-114">センサー データなし - デバイスがセンサー データの送信を停止しました。</span><span class="sxs-lookup"><span data-stu-id="0b71e-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="0b71e-115">制限のあるアラートをデバイスでトリガーすることができます。</span><span class="sxs-lookup"><span data-stu-id="0b71e-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="0b71e-116">障害のある通信 - デバイスとの通信機能に障害が発生しています。</span><span class="sxs-lookup"><span data-stu-id="0b71e-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="0b71e-117">詳細分析のためのファイルの送信、ファイルのブロック、ネットワークからのデバイスの分離など、デバイスとの通信を必要とするアクションが機能しない場合があります。</span><span class="sxs-lookup"><span data-stu-id="0b71e-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="0b71e-118">**アクティブ** Defender for Endpoint サービスへの報告を停止しているデバイス。</span><span class="sxs-lookup"><span data-stu-id="0b71e-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="0b71e-119">エクスポート機能を使用して、すべてのリストを CSV 形式でダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="0b71e-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="0b71e-120">詳細については、「[Microsoft Defender for Endpoint のセンサーの正常性状態をチェックする](/microsoft-365/security/defender-endpoint/check-sensor-status)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b71e-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="0b71e-121">デバイスが非アクティブまたは間違った設定になった原因の詳細については、「[Microsoft Defender for Endpoint で問題が発生したセンサーの修正](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b71e-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
