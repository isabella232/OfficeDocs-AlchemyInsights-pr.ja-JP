---
title: 共同管理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1556"
- "9000080"
ms.openlocfilehash: fe7dcebf847fbd7d91632e93e2253bf62ac659aa
ms.sourcegitcommit: 4ed431b2e1aed26d07bd7eba282531537d29ad0e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923565"
---
# <a name="co-management"></a><span data-ttu-id="9740d-102">共同管理</span><span class="sxs-lookup"><span data-stu-id="9740d-102">Co-management</span></span>

<span data-ttu-id="9740d-103">**構成マネージャーハイブリッドから Intune に移行するための前提条件**</span><span class="sxs-lookup"><span data-stu-id="9740d-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="9740d-104">[この記事](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="9740d-104">Review [this article](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa).</span></span>
- <span data-ttu-id="9740d-105">[ユーザーに Intune ライセンスを追加](https://docs.microsoft.com/intune/licenses-assign)します。</span><span class="sxs-lookup"><span data-stu-id="9740d-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="9740d-106">共同管理を構成する場合は、[エッジブラウザー](https://www.microsoft.com/windows/microsoft-edge)を使用します。</span><span class="sxs-lookup"><span data-stu-id="9740d-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="9740d-107">**Intune で管理されているデバイスに Config Manager クライアントをインストールする方法**</span><span class="sxs-lookup"><span data-stu-id="9740d-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="9740d-108">「 [INTUNE MDM 管理 Windows デバイス](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9740d-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="9740d-109">**MDM 機関を変更するだけの場合はどうすればよいですか?**</span><span class="sxs-lookup"><span data-stu-id="9740d-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="9740d-110">MDM 機関は、サポートケースを開かずに変更することができます。</span><span class="sxs-lookup"><span data-stu-id="9740d-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="9740d-111">MDM 機関を変更するには、次のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="9740d-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="9740d-112">MDM 機関を構成マネージャーから Intune スタンドアロンに変更する</span><span class="sxs-lookup"><span data-stu-id="9740d-112">Change MDM Authority from Config Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="9740d-113">MDM 機関を Intune スタンドアロンから構成マネージャーに変更する</span><span class="sxs-lookup"><span data-stu-id="9740d-113">Change MDM Authority from Intune standalone to Config Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)