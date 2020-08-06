---
title: スケジュール済みの更新の一時停止
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2020
ms.locfileid: "46556250"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="f97af-102">スケジュール済みの更新の一時停止</span><span class="sxs-lookup"><span data-stu-id="f97af-102">Pausing scheduled updates</span></span>

<span data-ttu-id="f97af-103">[一時停止] コマンドが発行されると、デバイスは次回 Intune にチェックインするまでコマンドを処理しません。</span><span class="sxs-lookup"><span data-stu-id="f97af-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="f97af-104">このため、デバイスは次のことを行う、または状態にある可能性があります:</span><span class="sxs-lookup"><span data-stu-id="f97af-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="f97af-105">チェックイン前にスケジュール済みの更新をインストールしている。</span><span class="sxs-lookup"><span data-stu-id="f97af-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="f97af-106">[一時停止] コマンドを発行したときに電源がオフになる。</span><span class="sxs-lookup"><span data-stu-id="f97af-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="f97af-107">この場合、デバイスの電源を入れたときに、チェックイン前からスケジュール済みの更新をダウンロードしてインストールした可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f97af-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>