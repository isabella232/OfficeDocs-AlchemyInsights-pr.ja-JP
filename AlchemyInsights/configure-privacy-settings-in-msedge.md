---
title: Microsoft Edge でプライバシー設定を構成する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090309"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Microsoft Edge でプライバシー設定を構成する

既定では、Microsoft Edge が Windows 以外のプラットフォームに展開されている場合、診断データとサイト情報は Microsoft に送信されません。 ただし、Microsoft Edge が Windows 10 に展開されている場合、診断データとサイト情報はユーザーの [Windows 診断データ設定](https://go.microsoft.com/fwlink/?linkid=2132472)に従って送信されます。

Microsoft Edge で組織のデータ収集を処理する方法を設定するには、次のグループ ポリシーを使用します。
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) は、使用状況およびクラッシュ関連データのレポートを有効にします。
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) は、Microsoft サービスの改善に使用されるサイト情報を送信します。

詳細については、「[ポリシー設定の構成](https://go.microsoft.com/fwlink/?linkid=2132577)」を参照してください。
