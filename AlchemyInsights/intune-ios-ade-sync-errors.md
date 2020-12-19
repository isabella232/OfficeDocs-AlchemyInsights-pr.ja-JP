---
title: Apple デバイスの自動登録同期エラー
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/17/2020
ms.locfileid: "49715069"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="2a2ce-102">Apple デバイスの自動登録同期エラー</span><span class="sxs-lookup"><span data-stu-id="2a2ce-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="2a2ce-103">「エラー状態にある 1 つまたは複数の ADE/DEP トークンがあることを検出しました。</span><span class="sxs-lookup"><span data-stu-id="2a2ce-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="2a2ce-104">影響を受ける各トークンについてエラーの状態が解決されるまで、ADE 機能は同様に使用できません。」</span><span class="sxs-lookup"><span data-stu-id="2a2ce-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="2a2ce-105">このエラーは、次のような場合に表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2a2ce-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="2a2ce-106">デバイスが ABM/ASM から Intune に同期されないことがある</span><span class="sxs-lookup"><span data-stu-id="2a2ce-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="2a2ce-107">登録プロファイルの割り当てが失敗した可能性がある</span><span class="sxs-lookup"><span data-stu-id="2a2ce-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="2a2ce-108">デバイスが ADE 登録を正常に完了しないことがある</span><span class="sxs-lookup"><span data-stu-id="2a2ce-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="2a2ce-109">**[デバイス]、 [デバイスの登録]、[ Apple の登録]、 [登録プログラムのトークン]** の順に Intune コンソールに報告された同期エラーがあるか確認して、可能性のある改善策を以下のドキュメントを参照し確認します。</span><span class="sxs-lookup"><span data-stu-id="2a2ce-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="2a2ce-110">IOS/iPadOS および macOS の自動デバイスの登録トークンの ABM/ASM 同期エラー</span><span class="sxs-lookup"><span data-stu-id="2a2ce-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
