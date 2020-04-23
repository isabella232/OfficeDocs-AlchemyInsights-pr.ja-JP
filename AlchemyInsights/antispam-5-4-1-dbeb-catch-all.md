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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707916"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>エラー コード 550 5.4.1リレー アクセスの拒否に関する配信の問題を修正

この問題は、Microsoft ネットワークへの入力時に[電子メールアドレスが有効であるかどうか](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)を確認するために、bouncebacks を確認するときに発生します。 以下の操作を試してください。

1. 問題がドメイン全体に見られるものか、それとも単一のメールアドレスに特有のものかを判断します。
    - ドメイン全体: 時折ドメインを同期する必要があります。[ドメインを Internal に設定してから Authoritative に戻して](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)みてください。
    - 単一のメールアドレス: 時折アドレスを同期する必要があります。SMTP プロキシ アドレスを変更してから元に戻すと良いかもしれません。
2. 問題がグループまたはパブリック フォルダーに特有のものかどうかを判断します。 一部のオブジェクト タイプでは Azure Active Directory でオブジェクトを手動で作成する必要がある場合があります。

追加のヘルプが必要な場合は、サポートチケットを開いて、問題の範囲 (送信元のオブジェクトの種類を含む) を指定してください。これにより、より良いお手伝いができます。