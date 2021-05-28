---
title: 攻撃面の減少ルール
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676607"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="5dc60-102">攻撃面の減少ルール</span><span class="sxs-lookup"><span data-stu-id="5dc60-102">Attack surface reduction rules</span></span>

<span data-ttu-id="5dc60-103">ファイルやフォルダーを除外すると、攻撃面の減少ルールで指定された保護機能が著しく低下します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="5dc60-104">ルールでブロックされたはずのファイルは実行が許可され、レポートやイベントは記録されません。</span><span class="sxs-lookup"><span data-stu-id="5dc60-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="5dc60-105">除外は、除外を許可するすべてのルールに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5dc60-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="5dc60-106">ASR の除外項目は、Microsoft Defender ウイルス対策の除外項目と同じ構文を使用します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="5dc60-107">詳細については、「[Windows Defender ウイルス対策のスキャンの除外項目の構成と検証](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="5dc60-108">問題を回避するには、「[除外を定義する際に避ける必要のある一般的な間違い](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="5dc60-109">すべての ASR ルールが除外項目をサポートしているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="5dc60-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="5dc60-110">ルールが除外項目をサポートしているかどうかを検証するには、テーブル「[攻撃面の減少ルール](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="5dc60-111">攻撃面の減少ルール</span><span class="sxs-lookup"><span data-stu-id="5dc60-111">Attack surface reduction rules</span></span>

<span data-ttu-id="5dc60-112">組織の攻撃面とは、攻撃者が組織のデバイスやネットワークを侵害する可能性のあるすべての場所を指します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="5dc60-113">攻撃対象を削減するということは、組織のデバイスやネットワークを保護し、攻撃者が攻撃を実行する手段を減らすことを意味します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="5dc60-114">Microsoft Defender for Endpoint で攻撃面の減少ルールを構成することが役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5dc60-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="5dc60-115">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-115">For more information, see:</span></span>

- [<span data-ttu-id="5dc60-116">ASR ルール GUID をマッピングして名前をつける</span><span class="sxs-lookup"><span data-stu-id="5dc60-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="5dc60-117">ASR ルールの要件は、以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5dc60-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="5dc60-118">Windows 10 バージョン 1709 以降</span><span class="sxs-lookup"><span data-stu-id="5dc60-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="5dc60-119">Windows 10 Enterprise バージョン 1709 以降</span><span class="sxs-lookup"><span data-stu-id="5dc60-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="5dc60-120">Windows Server バージョン 1803 (半期チャネル) 以降</span><span class="sxs-lookup"><span data-stu-id="5dc60-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="5dc60-121">適用する適切な除外項目を特定する</span><span class="sxs-lookup"><span data-stu-id="5dc60-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="5dc60-122">Microsoft - Windows - Windows Defender/Operational のログで eventID 1121 または 1122 であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="5dc60-123">ブロック シナリオとコンテキストを評価し、このシナリオはブロックを解除する必要があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="5dc60-124">イベントの詳細にある、除外を定義する値である Path の値を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5dc60-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="5dc60-125">除外項目はできるだけ厳密にしてください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="5dc60-126">必要に応じてワイルドカードを適用します (User 変数の置き換えなど)。</span><span class="sxs-lookup"><span data-stu-id="5dc60-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="5dc60-127">展開の必要性に応じて、除外事項を適用します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="5dc60-128">詳細については、「[攻撃面の減少ルールをカスタマイズする](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="5dc60-129">除外事項が受け入れられない</span><span class="sxs-lookup"><span data-stu-id="5dc60-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="5dc60-130">ルールが除外事項をサポートしているかどうか判断します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="5dc60-131">詳細については、「[攻撃面の減少ルール](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="5dc60-132">適用された除外項目を確認し、タイプミスや誤って解釈されたワイルドカードがないか、イベント データで検証します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="5dc60-133">詳細については、「[サポートされる除外タイプ](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)」を参照してください</span><span class="sxs-lookup"><span data-stu-id="5dc60-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="5dc60-134">ルールの影響が大きすぎる場合は、ルールを監査モードに戻してさらに検証を行うことを検討します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="5dc60-135">詳細については、「[Microsoft Defender for Endpoint 機能が監査モードで動作する方法を確認する](/microsoft-365/security/defender-endpoint/audit-windows-defender)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="5dc60-136">このコマンドを使用してサポート ケースを開くためのサポートデータを収集します。</span><span class="sxs-lookup"><span data-stu-id="5dc60-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="5dc60-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="5dc60-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="5dc60-138">詳細については、「[Microsoft Defender for Endpoints へのマシンのオンボードに関する問題](issues-with-onboarding-machines.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5dc60-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
