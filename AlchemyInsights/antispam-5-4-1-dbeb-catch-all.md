---
title: AntiSpam 5.4.1 DBEB のまとめ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717366"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正

この問題は、Microsoft ネットワークに入る際の[バウンスバックを防ぐためにメール アドレスが有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。 以下の操作を試してください。

1. 問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。
    - ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。
    - 単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。
2. 問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。 一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。

さらにサポートが必要な場合には、サポート チケットを開いて、より良いサポートをご提供できるよう問題の範囲 (送信先のオブジェクト タイプを含む) を明記してください。