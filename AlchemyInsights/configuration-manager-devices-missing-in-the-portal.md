---
title: Configuration Manager デバイスがポータルに表示されない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "43791320"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="7a9de-102">Configuration Manager デバイスがポータルに表示されない</span><span class="sxs-lookup"><span data-stu-id="7a9de-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="7a9de-103">デバイスの同期を機能させるには、サービス接続ポイントの役割をホストするオンプレミス サーバーから[必要なインターネット エンドポイント](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)に到達できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a9de-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="7a9de-104">デバイス同期のトラブルシューティングを行うには、サービス接続ポイントにある **CMGatewaySyncUploadWorker.log** を確認してください。</span><span class="sxs-lookup"><span data-stu-id="7a9de-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="7a9de-105">詳細については、「[Microsoft エンドポイント マネージャーでのテナント接続](https://docs.microsoft.com/configmgr/tenant-attach/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a9de-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
