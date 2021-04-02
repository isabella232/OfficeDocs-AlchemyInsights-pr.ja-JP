---
title: エンドポイント マネージャー - セキュリティベースライン
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440889"
---
# <a name="endpoint-manager---security-baselines"></a>エンドポイント マネージャー - セキュリティベースライン

セキュリティ ベースラインは、関連するセキュリティ チームが推奨する一連の設定と既定値を適用するのに役立つ、事前に構成された Windows 設定のグループです。 これらのベースラインは、目的の設定と値のみを提供するためにカスタマイズできます。 セキュリティ ベースラインの詳細については、「[セキュリティ ベースラインを使用して、Intune で Windows 10 デバイスを構成する](https://docs.microsoft.com/mem/intune/protect/security-baselines)」を参照してください。

現在、これらの製品のベースラインがあります。

- Windows MDM セキュリティ設定
- Microsoft Defender for Endpoint セキュリティ
- Microsoft Edge

各ベースラインは定期的に更新され、増分バージョンでリリースされます。 各バージョンは、ベースラインが現在のガイダンスを満たしていることを確認するために、以前のバージョンの設定を追加または削除します。 エンドポイント セキュリティ のセキュリティ ベースライン コンソールでは、バージョン間の変更を表示することで、異なるバージョン同士を比較することができます。

展開するベースラインのバージョンを最も効果的に変更する方法については、「[Microsoft Intune でセキュリティ ベースライン プロファイルを管理する](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)」を参照してください。

セキュリティ ベースラインを展開した後は、展開の状態を監視し、デバイス別に設定を確認できます。

**注:** ベースラインのレポート データがデバイスへの初期展開から表示されるまでに最大で 24 時間、さらに更新されるまでに最大 6 時間かかる場合があります。 

ベースライン設定が適用されない最も一般的な原因は、同じ設定が別のプロファイルで使用されているためです。 このシナリオは、セキュリティ ベースライン プロファイルの [デバイスの状態] ノードからそのデバイスを選択することで、特定のデバイスを調査できます。 詳細については、「[セキュリティ ベースラインの競合を解決する](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)」を参照してください。