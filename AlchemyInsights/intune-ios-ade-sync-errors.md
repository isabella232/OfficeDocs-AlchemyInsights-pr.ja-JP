---
title: Apple デバイスの自動登録同期エラー
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448927"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="e82ac-102">Apple デバイスの自動登録同期エラー</span><span class="sxs-lookup"><span data-stu-id="e82ac-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="e82ac-103">「エラー状態にある 1 つまたは複数の ADE/DEP トークンがあることを検出しました。</span><span class="sxs-lookup"><span data-stu-id="e82ac-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="e82ac-104">影響を受ける各トークンについてエラーの状態が解決されるまで、ADE 機能は期待どおりに使用できません。」</span><span class="sxs-lookup"><span data-stu-id="e82ac-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="e82ac-105">このエラーは、次のような場合に表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e82ac-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="e82ac-106">デバイスが ABM/ASM から Intune に同期されないことがある</span><span class="sxs-lookup"><span data-stu-id="e82ac-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="e82ac-107">登録プロファイルの割り当てが失敗した可能性がある</span><span class="sxs-lookup"><span data-stu-id="e82ac-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="e82ac-108">デバイスが ADE 登録を正常に完了しないことがある</span><span class="sxs-lookup"><span data-stu-id="e82ac-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="e82ac-109">**[デバイス]、[デバイスの登録]、[Apple の登録]、[登録プログラムのトークン]** の順に Intune コンソールに報告された同期エラーがあるか確認します。</span><span class="sxs-lookup"><span data-stu-id="e82ac-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="e82ac-110">同期エラーの最も一般的な原因の 1 つは、現在のトークンの有効期限です。</span><span class="sxs-lookup"><span data-stu-id="e82ac-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="e82ac-111">多くの場合、影響を受けるトークンを更新すると問題が解決します。</span><span class="sxs-lookup"><span data-stu-id="e82ac-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="e82ac-112">1 つ以上のトークンの有効期限が切れている場合は、次のドキュメントを参照して必要に応じてトークンを更新します。</span><span class="sxs-lookup"><span data-stu-id="e82ac-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="e82ac-113">自動デバイス登録トークンを更新する</span><span class="sxs-lookup"><span data-stu-id="e82ac-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="e82ac-114">さらに、次のドキュメントを参照して、トークンの同期エラーの原因となる他のエラーの潜在的な修正を確認できます。</span><span class="sxs-lookup"><span data-stu-id="e82ac-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="e82ac-115">IOS/iPadOS および macOS の自動デバイスの登録トークンの ABM/ASM 同期エラー</span><span class="sxs-lookup"><span data-stu-id="e82ac-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="e82ac-116">IOS/iPadOS および macOS の自動デバイスの登録トークンの ABM/ASM 同期エラー</span><span class="sxs-lookup"><span data-stu-id="e82ac-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
