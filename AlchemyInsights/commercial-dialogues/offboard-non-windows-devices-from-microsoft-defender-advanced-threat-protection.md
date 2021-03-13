---
title: Microsoft Defender Advanced Threat Protection (ATP) から Windows 以外のデバイスをオフボードする
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751254"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="db964-102">Microsoft Defender Advanced Threat Protection (ATP) から Windows 以外のデバイスをオフボードする</span><span class="sxs-lookup"><span data-stu-id="db964-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="db964-103">次の操作を実行してください。</span><span class="sxs-lookup"><span data-stu-id="db964-103">Here's how:</span></span>

1. <span data-ttu-id="db964-104">サードパーティのソリューションを Microsoft Defender ATP から切断するには、サードパーティのドキュメントに従ってください。</span><span class="sxs-lookup"><span data-stu-id="db964-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="db964-105">Azure Active Directory テナントから、サードパーティのソリューションのアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="db964-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="db964-106">[Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="db964-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="db964-107">**[すべてのサービス]** > **[Azure Active Directory]** > **[エンタープライズ アプリケーション]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="db964-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="db964-108">オフボードするアプリケーションを選択します。</span><span class="sxs-lookup"><span data-stu-id="db964-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="db964-109">**[削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="db964-109">Select **Delete**.</span></span>

<span data-ttu-id="db964-110">詳細については、「[Windows 以外のデバイスをオフボードする](https://go.microsoft.com/fwlink/?linkid=2143630)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db964-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
