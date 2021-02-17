---
title: レプリカ セット
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
- "9004400"
- "8265"
ms.openlocfilehash: 7b6d614fddfcb5722e426b520f1c0d6c539c7f33
ms.sourcegitcommit: 9400cd853b7a5a81f6f5a1ad9601fef37c18bcae
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50254941"
---
# <a name="replica-set"></a><span data-ttu-id="80516-102">レプリカ セット</span><span class="sxs-lookup"><span data-stu-id="80516-102">Replica set</span></span>

<span data-ttu-id="80516-103">AADDS は管理対象ドメインとも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="80516-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="80516-104">実際には、バックエンドによって実行および保守される 2 つのドメイン コントローラーです。</span><span class="sxs-lookup"><span data-stu-id="80516-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="80516-105">2 つの DC には、メイン DC とレプリケーション DC が 1 つずつ含まれます。</span><span class="sxs-lookup"><span data-stu-id="80516-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="80516-106">AADDS (管理対象ドメイン) でのバックアップは、Azure プラットフォームによって管理される自動プロセスです。</span><span class="sxs-lookup"><span data-stu-id="80516-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="80516-107">管理対象ドメインに問題が発生した場合は、Azure サポートがバックアップからの復元を支援します。</span><span class="sxs-lookup"><span data-stu-id="80516-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="80516-108">仮想ネットワーク内で各レプリカ セットを作成します。</span><span class="sxs-lookup"><span data-stu-id="80516-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="80516-109">各仮想ネットワークは、管理対象ドメインのレプリカセットをホストする他のすべての仮想ネットワークとピアリングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="80516-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="80516-110">この構成では、ディレクトリ レプリケーションをサポートするメッシュ ネットワーク トポロジが作成されます。</span><span class="sxs-lookup"><span data-stu-id="80516-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="80516-111">各レプリカ セットが異なる仮想サブネット内にある場合、仮想ネットワークは複数のレプリカ セットをサポートできます。</span><span class="sxs-lookup"><span data-stu-id="80516-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="80516-112">レプリカ セットの詳細については、「[レプリカ セットの概念](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80516-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
