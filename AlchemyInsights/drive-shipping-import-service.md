---
title: Microsoft 365 インポート サービスのドライブ配送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2021
ms.locfileid: "52732086"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="1d84d-102">Microsoft 365 インポート サービスのドライブ配送</span><span class="sxs-lookup"><span data-stu-id="1d84d-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="1d84d-103">ドライブ配送を使用するには、PST をハード ドライブにコピーしてから、ハード ドライブを Microsoft に配送します。</span><span class="sxs-lookup"><span data-stu-id="1d84d-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="1d84d-104">ジョブを開始するには:</span><span class="sxs-lookup"><span data-stu-id="1d84d-104">To start the job:</span></span>

1. <span data-ttu-id="1d84d-105">Microsoft 365 コンプライアンス センターの **[情報ガバナンス]** で、**[インポート]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1d84d-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="1d84d-106">**[インポート ジョブの種類の選択]** を選択し、**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1d84d-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="1d84d-107">このインポート オプションの手順を確認するには、**[Microsoft の物理的な場所のいずれかにハード ドライブを送付する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1d84d-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="1d84d-108">覚えておきたい点がいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="1d84d-108">Here are some things to remember:</span></span>

- <span data-ttu-id="1d84d-109">PST ファイルを Microsoft 365 メールボックスにインポートするには、Exchange Online で Mailbox Import Export の役割が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d84d-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="1d84d-110">20 GB を超える PST の場合、パフォーマンスに影響する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1d84d-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="1d84d-111">2.5 インチのソリッドステート ドライブ (SSD) または 2.5 インチまたは 3.5 インチの SATA II/III 内部ハード ドライブのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1d84d-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="1d84d-112">PST ファイルを含むハード ドライブは、BitLocker で暗号化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d84d-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="1d84d-113">ドライブ送付で PST ファイルを Microsoft 365 メールボックスにインポートする費用は、データ 1 GB 当たり $2 USD です。</span><span class="sxs-lookup"><span data-stu-id="1d84d-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="1d84d-114">PST のインポートにドライブ配送方法を使用する際の詳細については、「[ドライブ配送を使用して組織の PST ファイルをインポートする](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d84d-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>