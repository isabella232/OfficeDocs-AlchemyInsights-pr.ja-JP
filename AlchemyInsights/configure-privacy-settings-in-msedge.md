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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405856"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>Microsoft Edge でプライバシー設定を構成する

既定では、Microsoft Edge が Windows 以外のプラットフォームに展開されている場合、診断データとサイト情報は Microsoft に送信されません。 ただし、Microsoft Edge が Windows 10 に展開されている場合、診断データとサイト情報はユーザーの [Windows 診断データ設定](https://go.microsoft.com/fwlink/?linkid=2132472)に従って送信されます。

Microsoft Edge で組織のデータ収集を処理する方法を設定するには、次のグループ ポリシーを使用します。
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) は、使用状況およびクラッシュ関連データのレポートを有効にします。
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) は、Microsoft サービスの改善に使用されるサイト情報を送信します。

詳細については、「[ポリシー設定の構成](https://go.microsoft.com/fwlink/?linkid=2132577)」を参照してください。
