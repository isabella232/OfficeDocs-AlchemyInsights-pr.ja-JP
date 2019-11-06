---
title: スパム対策 5.4.1 DBEB キャッチオール
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2019
ms.locfileid: "37973184"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>エラーコード 550 5.4.1 Relay アクセスが拒否された場合の配信に関する問題の修正

この問題は、Office 365 ネットワークへの入力時に[電子メールアドレスが有効であるかどうかを確認するために、bouncebacks が有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。 次の方法を試します。

1. 問題がドメイン全体に特有なものか、単一の電子メールアドレスであるかを判別します。
    - ドメイン全体: ドメインを同期する必要がある場合があります。[ドメインを内部に設定してから、権限のあるものに戻し](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)てください。
     - 単一の電子メールアドレス: 場合によっては、アドレスを同期する必要があります。smtp プロキシアドレスを変更した後、それを再度変更することができます。
2. 問題がグループまたはパブリックフォルダーに固有かどうかを判断します。 オブジェクトの種類によっては、Azure Active Directory にオブジェクトを手動で作成する必要がある場合があります。

追加のヘルプが必要な場合は、サポートチケットを開いて、問題の範囲 (「送信するオブジェクトの種類」) を指定してください。これにより、より良いお手伝いができます。