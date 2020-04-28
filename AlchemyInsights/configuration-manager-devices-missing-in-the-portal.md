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
# <a name="configuration-manager-devices-missing-in-the-portal"></a>Configuration Manager デバイスがポータルに表示されない

デバイスの同期を機能させるには、サービス接続ポイントの役割をホストするオンプレミス サーバーから[必要なインターネット エンドポイント](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)に到達できる必要があります。 デバイス同期のトラブルシューティングを行うには、サービス接続ポイントにある **CMGatewaySyncUploadWorker.log** を確認してください。

詳細については、「[Microsoft エンドポイント マネージャーでのテナント接続](https://docs.microsoft.com/configmgr/tenant-attach/)」を参照してください。
