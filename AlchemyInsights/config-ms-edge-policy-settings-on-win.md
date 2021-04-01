---
title: Windows で Microsoft Edge ポリシー設定を構成する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "9004632"
- "6894"
- "8358"
ms.openlocfilehash: e9bb489b4d8ecd76fd777ade9fb740ecad542900
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402380"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="e8668-102">Windows で Microsoft Edge ポリシー設定を構成する</span><span class="sxs-lookup"><span data-stu-id="e8668-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="e8668-103">Microsoft Edge のポリシー設定と管理された更新を構成するには、グループ ポリシー オブジェクト (GPO) を使用します。</span><span class="sxs-lookup"><span data-stu-id="e8668-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="e8668-104">レジストリを通してポリシーをプロビジョニングすることもできます。 これは、(1) Microsoft Active Directory ドメインに参加している Windows デバイス、および (2) Microsoft Intune のデバイス管理用に登録されている Windows10 Pro および Enterprise インスタンスに適しています。</span><span class="sxs-lookup"><span data-stu-id="e8668-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="e8668-105">GPO を使用して Microsoft Edge を構成するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e8668-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="e8668-106">Active Directory ドメインのグループ ポリシー セントラル ストア、または個々のコンピューターのポリシー定義テンプレート フォルダーに、Microsoft Edge のルールと設定を追加するすべての管理用テンプレートをインストールします。</span><span class="sxs-lookup"><span data-stu-id="e8668-106">Go to the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="e8668-107">設定する特定のポリシーを構成します。</span><span class="sxs-lookup"><span data-stu-id="e8668-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="e8668-108">詳細については、「[Windows で Microsoft Edge ポリシー設定を構成する](https://go.microsoft.com/fwlink/?linkid=2135024)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8668-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
