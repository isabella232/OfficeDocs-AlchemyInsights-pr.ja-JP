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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923565"
---
# <a name="co-management"></a><span data-ttu-id="a5d64-102">共同管理</span><span class="sxs-lookup"><span data-stu-id="a5d64-102">Co-management</span></span>

<span data-ttu-id="a5d64-103">**構成マネージャー ハイブリッドから Intune に移行するための前提条件**</span><span class="sxs-lookup"><span data-stu-id="a5d64-103">**Prerequisites for migrating from Config Manager Hybrid to Intune**</span></span>

- <span data-ttu-id="a5d64-104">[この記事](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-hybridmdm-to-intunesa)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="a5d64-104">Review this article</span></span>
- <span data-ttu-id="a5d64-105">[ユーザーに Intune ライセンスを追加する](https://docs.microsoft.com/intune/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="a5d64-105">[Add an Intune license to your users](https://docs.microsoft.com/intune/licenses-assign).</span></span>
- <span data-ttu-id="a5d64-106">共同管理を構成する場合は、[Edge ブラウザー](https://www.microsoft.com/windows/microsoft-edge)を使用します。</span><span class="sxs-lookup"><span data-stu-id="a5d64-106">Use the [Edge browser](https://www.microsoft.com/windows/microsoft-edge) when configuring Co-management.</span></span>

<span data-ttu-id="a5d64-107">**Intune によって管理されるデバイスに構成マネージャー クライアントをインストールする方法**</span><span class="sxs-lookup"><span data-stu-id="a5d64-107">**How to I install the Config Manager client on Intune-managed devices**</span></span>

<span data-ttu-id="a5d64-108">詳細については、「[Intune MDM によって管理される Windows デバイス](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5d64-108">See [Intune MDM-managed Windows devices](https://docs.microsoft.com/sccm/core/clients/deploy/deploy-clients-to-windows-computers#bkmk_mdm).</span></span>

<span data-ttu-id="a5d64-109">**MDM 機関のみを変更したい場合**</span><span class="sxs-lookup"><span data-stu-id="a5d64-109">**What if I just want to change MDM authority?**</span></span>

<span data-ttu-id="a5d64-110">MDM 機関は、サポート ケースを開かずに変更できます。</span><span class="sxs-lookup"><span data-stu-id="a5d64-110">MDM Authority can be changed without opening a support case.</span></span> <span data-ttu-id="a5d64-111">次のドキュメントを参照して、MDM 機関を変更してください。</span><span class="sxs-lookup"><span data-stu-id="a5d64-111">Please review the following documentation to assist in changing your MDM authority:</span></span>
- [<span data-ttu-id="a5d64-112">MDM 機関を構成マネージャーから Intune スタンドアロンに変更する</span><span class="sxs-lookup"><span data-stu-id="a5d64-112">Change MDM authority from the Configuration Manager to Intune standalone</span></span>](https://docs.microsoft.com/sccm/mdm/deploy-use/migrate-change-mdm-authority)
- [<span data-ttu-id="a5d64-113">MDM 機関を Intune スタンドアロンから構成マネージャーに変更する</span><span class="sxs-lookup"><span data-stu-id="a5d64-113">Change MDM authority from Intune standalone to Configuration Manager</span></span>](https://docs.microsoft.com/intune-classic/deploy-use/prerequisites-for-enrollment#what-to-do-if-you-choose-the-wrong-mdm-authority-setting)