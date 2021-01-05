---
title: Microsoft Edge はプライバシー設定を構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680453"
---
# <a name="microsoft-edge-configure-privacy-settings"></a><span data-ttu-id="308ce-102">Microsoft Edge はプライバシー設定を構成する</span><span class="sxs-lookup"><span data-stu-id="308ce-102">Microsoft Edge configure privacy settings</span></span>

<span data-ttu-id="308ce-103">既定では、Microsoft Edge が Windows 以外のプラットフォームに展開されている場合、診断データとサイト情報は Microsoft に送信されません。</span><span class="sxs-lookup"><span data-stu-id="308ce-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information are not sent to Microsoft.</span></span> <span data-ttu-id="308ce-104">ただし、Microsoft Edge が Windows 10 に展開されている場合、診断データとサイト情報はユーザーの [Windows 診断データ設定](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)に従って送信されます。</span><span class="sxs-lookup"><span data-stu-id="308ce-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).</span></span>

<span data-ttu-id="308ce-105">Microsoft Edge で組織のデータ収集を処理する方法を設定するには、次のグループ ポリシーを使用します。</span><span class="sxs-lookup"><span data-stu-id="308ce-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="308ce-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): このポリシーは、使用状況およびクラッシュ関連データのレポートを有効にします。</span><span class="sxs-lookup"><span data-stu-id="308ce-106">[MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): This policy enables reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="308ce-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): このポリシーは、Microsoft サービスの改善に使用されるサイト情報を送信します。</span><span class="sxs-lookup"><span data-stu-id="308ce-107">[SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): This policy sends site information that is used to improve Microsoft services.</span></span>

<span data-ttu-id="308ce-108">詳細については、「[ポリシー設定の構成](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="308ce-108">To learn more, see [Configure policy settings](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).</span></span>