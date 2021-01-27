---
title: 検疫状態のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/22/2021
ms.locfileid: "49950157"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="10c09-102">検疫状態のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="10c09-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="10c09-103">Azure Active Directory (AD) プロビジョニング サービスは、構成の正常性を監視します。</span><span class="sxs-lookup"><span data-stu-id="10c09-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="10c09-104">また、異常なアプリを **[検疫]** 状態にします。</span><span class="sxs-lookup"><span data-stu-id="10c09-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="10c09-105">ターゲット システムに対して行われた呼び出しのほとんどまたはすべてが一貫して失敗する場合、プロビジョニング ジョブは **[検疫]** としてマークされます。</span><span class="sxs-lookup"><span data-stu-id="10c09-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="10c09-106">失敗の例として、**無効な管理者の資格情報が原因でエラーが受信されました**。</span><span class="sxs-lookup"><span data-stu-id="10c09-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="10c09-107">詳細については、「[検疫状態のアプリケーションのプロビジョニング](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10c09-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="10c09-108">クラウド同期のトラブルシューティングについては、「[隔離された問題のプロビジョニング](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10c09-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
