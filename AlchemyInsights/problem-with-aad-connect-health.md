---
title: AAD Connect Health の問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484087"
---
# <a name="problem-with-aad-connect-health"></a>AAD Connect Health の問題

- 外科手術を行う権限があることを確認してください。 グローバル管理者は既定でアクセス権を持っています。 さらに、[ロール ベースのアクセス制御](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)を使用して、登録権限を共同作成者に委任できます。
- 必要なエンドポイントが有効になっていて、ファイアウォールが原因でブロックされていないことを確認してください。 詳細については、[要件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)を参照してください。
- ネットワーク レイヤーによる SSL 検査の対象となるアウトバウンド通信が原因で、登録が失敗する可能性があります。
- Azure AD Connect Health の通知設定を確認したことを確認してください。 設定を確認してください。 この[ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)は、Azure AD Connect Health 通知の通知設定を構成する方法を理解するのに役立ちます。
- AAD Connect Health 同期レポートとそのダウンロード方法の詳細については、「[オブジェクト レベルの同期レポート](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)」を参照してください。

AAD Connect Health アラートのトラブルシューティングを行うには、「[AAD Connect Health データの鮮度アラートのトラブルシューティング ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)」従ってください。よくある質問については、「[AAD Connect Health のインストールに関する一般的な質問](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)」を参照してください。
