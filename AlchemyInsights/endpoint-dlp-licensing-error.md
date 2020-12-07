---
title: エンドポイント DLP ライセンス エラー
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/30/2020
ms.locfileid: "49565238"
---
# <a name="endpoint-dlp-licensing-error"></a>エンドポイント DLP ライセンス エラー

エンドポイント DLP を設定しようとしたときに、次のエラーが発生した場合:

`Your organization is missing the licenses required to manage these devices`

次のいずれかのサブスクリプションまたはアドオンがあることを確認します。

- Microsoft 365 E5
- Microsoft 365 A5 (EDU) 
- Microsoft 365 E5 コンプライアンス
- Microsoft 365 A5 コンプライアンス
- Microsoft 365 E5 の情報保護とガバナンス
- Microsoft 365 A5 の情報保護とガバナンス

> [!NOTE]
> これは、次のようなライセンスの組み合わせでは動作しません: Win E5 + O365 E5 + EMS E5。 この機能を設定するには、純粋な M365 E5 ライセンスが必要です。

エンドポイント DLP ライセンスの詳細については、「[エンドポイント DLP ライセンス](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)」を参照してください。
