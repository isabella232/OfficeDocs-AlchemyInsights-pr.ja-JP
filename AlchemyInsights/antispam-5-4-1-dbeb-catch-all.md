---
title: AntiSpam 5.4.1 DBEB のまとめ
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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672438"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正

この問題は、Office 365 ネットワークに入る際の[バウンスバックを防ぐためにメール アドレスが有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。 以下の操作を試してください。

1. 問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。
    - ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。
    - 単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。
2. 問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。 一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。

さらにサポートが必要な場合には、サポート チケットを開いて、問題の範囲 (送信先のオブジェクト タイプを含む) を指定してください。そうすれば、より良いサポートを提供できます。