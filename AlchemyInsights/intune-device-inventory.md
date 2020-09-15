---
title: Intune デバイス インベントリ
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667883"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="59777-102">Intune デバイス インベントリ</span><span class="sxs-lookup"><span data-stu-id="59777-102">Intune Device Inventory</span></span>

<span data-ttu-id="59777-103">デバイス ブレードは、デバイスごとに Intune で管理されているデバイスに対する管理者の分析情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="59777-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="59777-104">表示される情報には、ハードウェア、検出されたアプリケーション、デバイスのコンプライアンス状態、デバイスの構成状態が含まれます。</span><span class="sxs-lookup"><span data-stu-id="59777-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="59777-105">ハードウェアと検出されたアプリケーションのインベントリデータは、7日間のサイクルで収集されます。</span><span class="sxs-lookup"><span data-stu-id="59777-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="59777-106">報告されるハードウェアのアプリケーションと特定の要素は、デバイスのオペレーティングシステムとデバイスが個人所有か企業所有かによって異なります。</span><span class="sxs-lookup"><span data-stu-id="59777-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="59777-107">詳細については、「[Intuneでデバイスの詳細を確認する](https://docs.microsoft.com/intune/device-inventory)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59777-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="59777-108">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="59777-108">**FAQ**</span></span>

<span data-ttu-id="59777-109">Q: Intune に登録された Windows デバイスに存在するアプリケーションの完全なインベントリリストを受け取っていません。</span><span class="sxs-lookup"><span data-stu-id="59777-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="59777-110">どうしてでしょうか?</span><span class="sxs-lookup"><span data-stu-id="59777-110">Why not?</span></span>

<span data-ttu-id="59777-111">A: 現時点では、企業のデバイスとして識別される Windows 10 PC 用の最新アプリのみがリスト表示されます。</span><span class="sxs-lookup"><span data-stu-id="59777-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="59777-112">Intune は、これらのデバイスにインストールされているWin32 アプリに関する情報を収集しません。</span><span class="sxs-lookup"><span data-stu-id="59777-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="59777-113">Q: どのデバイスからも電話番号が収集されないのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="59777-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="59777-114">A: Intune で企業デバイスとして分類された電話は、モバイルデバイス インベントリレポートを実行したときなどは、完全な電話番号として識別されません。</span><span class="sxs-lookup"><span data-stu-id="59777-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="59777-115">持ち込まれたデバイスの電話番号は、部分的にアスタリスク (\*\*\*\*) で隠され、最後の4桁のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="59777-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>