---
title: 電子情報開示で発生するエラーのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 2a7372c7b20b87c8c774eae4ca4540a3bd19709596405da041eeaa24db310fa7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105393"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>電子情報開示で発生するエラーのトラブルシューティング

電子情報開示で問題が発生していますか? こちらに、推奨されるベスト プラクティスの一部を示します。

- 保持している配布状態を確認します。  状態が **オン (保留中)** または **オフ (保留中)** である場合は、配布の保持を待機して完了します。
- 電子情報開示の更新の保持を、トランザクションごとに繰り返しポリシーを更新するのではなく、1 つの一括要求に結合します。
- Set-CaseHoldPolicy <policyname> の実行 - RetryDistribution を セキュリティ/コンプライアンス センター Powershell で実行します。 詳細については、「[セキュリティ/コンプライアンス センターの PowerShell に接続する](/powershell/exchange/connect-to-scc-powershell)」を参照してください。

これらの設定を確認する手順や、電子情報開示の保持の問題を解決するためのその他のベスト プラクティスについては、「[電子情報開示の保持エラーのトラブルシューティング](/microsoft-365/compliance/hold-distribution-errors)」を参照してください。
その他の一般的な電子情報開示の問題のトラブルシューティングについては、[電子情報開示に共通する問題の調査、トラブルシューティング、問題解決](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)」をご参照ください。
