---
title: エンドポイント マネージャー - セキュリティベースライン
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440889"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="693e7-102">エンドポイント マネージャー - セキュリティベースライン</span><span class="sxs-lookup"><span data-stu-id="693e7-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="693e7-103">セキュリティ ベースラインは、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するのに役立つ、事前に構成された Windows 設定のグループです。</span><span class="sxs-lookup"><span data-stu-id="693e7-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="693e7-104">これらのベースラインは、目的の設定と値のみを提供するためにカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="693e7-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="693e7-105">セキュリティ ベースラインの詳細については、「[セキュリティ ベースラインを使用して、Intune で Windows 10 デバイスを構成する](https://docs.microsoft.com/mem/intune/protect/security-baselines)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="693e7-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="693e7-106">現在、これらの製品のベースラインがあります。</span><span class="sxs-lookup"><span data-stu-id="693e7-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="693e7-107">Windows MDM セキュリティ設定</span><span class="sxs-lookup"><span data-stu-id="693e7-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="693e7-108">Microsoft Defender for Endpoint セキュリティ</span><span class="sxs-lookup"><span data-stu-id="693e7-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="693e7-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="693e7-109">Microsoft Edge</span></span>

<span data-ttu-id="693e7-110">各ベースラインは定期的に更新され、増分バージョンでリリースされます。</span><span class="sxs-lookup"><span data-stu-id="693e7-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="693e7-111">各バージョンは、ベースラインが現在のガイダンスを満たしていることを確認するために、以前のバージョンの設定を追加または削除します。</span><span class="sxs-lookup"><span data-stu-id="693e7-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="693e7-112">エンドポイント セキュリティ のセキュリティ ベースライン コンソールでは、バージョン間の変更を表示することで、異なるバージョン同士を比較することができます。</span><span class="sxs-lookup"><span data-stu-id="693e7-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="693e7-113">展開するベースラインのバージョンを最も効果的に変更する方法については、「[Microsoft Intune でセキュリティ ベースライン プロファイルを管理する](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="693e7-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="693e7-114">セキュリティ ベースラインを展開した後は、展開の状態を監視し、デバイス別に設定を確認できます。</span><span class="sxs-lookup"><span data-stu-id="693e7-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="693e7-115">**注:** ベースラインのレポート データがデバイスへの初期展開から表示されるまでに最大で 24 時間、さらに更新されるまでに最大 6 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="693e7-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="693e7-116">ベースライン設定が適用されない最も一般的な原因は、同じ設定が別のプロファイルで使用されているためです。</span><span class="sxs-lookup"><span data-stu-id="693e7-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="693e7-117">このシナリオは、セキュリティ ベースライン プロファイルの [デバイスの状態] ノードからそのデバイスを選択することで、特定のデバイスを調査できます。</span><span class="sxs-lookup"><span data-stu-id="693e7-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="693e7-118">詳細については、「[セキュリティ ベースラインの競合を解決する](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="693e7-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>