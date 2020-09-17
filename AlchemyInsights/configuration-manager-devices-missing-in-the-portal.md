---
title: Configuration Manager デバイスがポータルに表示されない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812156"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="1914c-102">Configuration Manager デバイスがポータルに表示されない</span><span class="sxs-lookup"><span data-stu-id="1914c-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="1914c-103">デバイスの同期を機能させるには、サービス接続ポイントの役割をホストするオンプレミス サーバーから[必要なインターネット エンドポイント](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)に到達できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1914c-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="1914c-104">デバイス同期のトラブルシューティングを行うには、サービス接続ポイントにある **CMGatewaySyncUploadWorker.log** を確認してください。</span><span class="sxs-lookup"><span data-stu-id="1914c-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="1914c-105">詳細については、「[Microsoft エンドポイント マネージャーでのテナント接続](https://docs.microsoft.com/configmgr/tenant-attach/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1914c-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
