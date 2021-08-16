---
title: AAD Connect の通知
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
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097311"
---
# <a name="notification-aad-connect"></a>AAD Connect の通知

- 外科手術を行う権限があることを確認してください。 グローバル管理者は既定でアクセス権を持っています。 さらに、[ロール ベースのアクセス制御](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)を使用して、登録権限を共同作成者に委任できます。
- 必要なエンドポイントが有効になっていて、ファイアウォールが原因でブロックされていないことを確認してください。 詳細については、[要件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)を参照してください。
- ネットワーク レイヤーによる SSL 検査の対象となるアウトバウンド通信が原因で、登録が失敗する可能性があります。
- Azure AD Connect Health の通知設定を確認して、自分の設定をレビューしてください。 Azure AD Connect Health 通知の通知設定を構成する方法を理解するには、この[ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)が役立ちます。
- AAD Connect Health 同期レポートとそのダウンロード方法の詳細については、「[オブジェクト レベルの同期レポート](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)」を参照してください。

AAD Connect Health アラートのトラブルシューティングを行うには、「[AAD Connect Health データの鮮度アラートのトラブルシューティング ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)」に従ってください。よくある質問については、「[AAD Connect Health のインストールに関する一般的な質問](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)」を参照してください。
