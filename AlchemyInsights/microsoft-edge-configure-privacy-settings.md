---
title: Microsoft Edge はプライバシー設定を構成する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114177"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge はプライバシー設定を構成する

既定では、Microsoft Edge が Windows 以外のプラットフォームに展開されている場合、診断データとサイト情報は Microsoft に送信されません。 ただし、Microsoft Edge が Windows 10 に展開されている場合、診断データとサイト情報はユーザーの [Windows 診断データ設定](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)に従って送信されます。

Microsoft Edge で組織のデータ収集を処理する方法を設定するには、次のグループ ポリシーを使用します。
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): このポリシーは、使用状況およびクラッシュ関連データのレポートを有効にします。
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): このポリシーは、Microsoft サービスの改善に使用されるサイト情報を送信します。

詳細については、「[ポリシー設定の構成](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)」を参照してください。