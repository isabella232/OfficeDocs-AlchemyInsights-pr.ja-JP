---
title: Configuration Manager デバイスがポータルに表示されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817249"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Configuration Manager デバイスがポータルに表示されない

デバイスの同期を機能させるには、サービス接続ポイントの役割をホストするオンプレミス サーバーから[必要なインターネット エンドポイント](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)に到達できる必要があります。 デバイス同期のトラブルシューティングを行うには、サービス接続ポイントにある **CMGatewaySyncUploadWorker.log** を確認してください。

詳細については、「[Microsoft エンドポイント マネージャーでのテナント接続](https://docs.microsoft.com/configmgr/tenant-attach/)」を参照してください。
