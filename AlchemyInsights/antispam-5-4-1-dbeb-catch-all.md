---
title: AntiSpam 5.4.1 DBEB のまとめ
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821452"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正

この問題は、Microsoft ネットワークに入る際の[バウンスバックを防ぐためにメール アドレスが有効かどうかを確認する](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)ときに発生します。 以下の操作を試してください。

1. 問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。
    - ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。
    - 単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。
2. 問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。 一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。

さらにサポートが必要な場合には、サポート チケットを開いて、より良いサポートをご提供できるよう問題の範囲 (送信先のオブジェクト タイプを含む) を明記してください。