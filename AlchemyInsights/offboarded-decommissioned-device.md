---
title: オフボードまたは廃止されたデバイスをデバイス インベントリから削除する場合の問題点
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564780"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="a37cd-102">オフボードまたは廃止されたデバイスをデバイス インベントリから削除する場合の問題点</span><span class="sxs-lookup"><span data-stu-id="a37cd-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="a37cd-103">Microsoft Defender for Endpoint では現在、オフボードまたは使用を停止したデバイスのデバイス レコードをデバイス インベントリから手動で削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="a37cd-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="a37cd-104">セキュリティ上の理由から、デバイスは最大 180 日間、履歴としてポータルに残ります。</span><span class="sxs-lookup"><span data-stu-id="a37cd-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="a37cd-105">ただし、デバイス データは、設定した保存期間に従って消去されます。</span><span class="sxs-lookup"><span data-stu-id="a37cd-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="a37cd-106">**注**: オフボードまたは使用を停止したデバイスは、7 日後に自動的に **非アクティブ** 状態に切り替わります。</span><span class="sxs-lookup"><span data-stu-id="a37cd-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="a37cd-107">また、過去 30 日間にアクティブでなかったデバイスは、組織の脅威と脆弱性管理の公開スコアやデバイス向けの Microsoft セキュリティ スコアを反映するデータには反映されません。</span><span class="sxs-lookup"><span data-stu-id="a37cd-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="a37cd-108">それでも特定のデバイスがデバイス インベントリ ビューに表示されない場合は、デバイス タグを配置して、デバイス インベントリ ビューから使用を停止したデバイスのフィルター処理をお試しください。</span><span class="sxs-lookup"><span data-stu-id="a37cd-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="a37cd-109">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a37cd-109">For more information, see:</span></span>

[<span data-ttu-id="a37cd-110">Microsoft Defender for Endpoint サービスのオフボード デバイス</span><span class="sxs-lookup"><span data-stu-id="a37cd-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="a37cd-111">脅威と脆弱性の管理における露出スコア</span><span class="sxs-lookup"><span data-stu-id="a37cd-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="a37cd-112">Microsoft Defender for Endpoint で問題が発生したセンサーの修正</span><span class="sxs-lookup"><span data-stu-id="a37cd-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="a37cd-113">タグの効果的な使用方法 (パート 1)</span><span class="sxs-lookup"><span data-stu-id="a37cd-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="a37cd-114">タグの効果的な使用方法 (パート 2)</span><span class="sxs-lookup"><span data-stu-id="a37cd-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="a37cd-115">タグの効果的な使用方法 (パート 3)</span><span class="sxs-lookup"><span data-stu-id="a37cd-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




