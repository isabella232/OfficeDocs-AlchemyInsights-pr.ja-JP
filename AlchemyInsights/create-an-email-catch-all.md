---
title: Catch All メールを作成する
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816205"
---
# <a name="create-an-email-catch-all"></a>Catch All メールを作成する

Catch All の使用は避けることを強く推奨します。 送信者が処置をとることができるように、送信者に返信し、送信者のメッセージが送信先に配信されなかったことを通知することをお勧めします。 以前の有効なメール アドレスのみをキャッチするように監視するメールボックスを限定することもできます。 

Catch All メールボックスは大量の迷惑メールを受信するため、厳重に監視されていない場合、最終的にはいっぱいになってしまいます。 (受信数には制限があります。) 

続行する場合は、次の手順を実行します。

1. "すべての種類の受信者を含める" という動的配布グループを作成する。

2. catchall@domain.com などのメールをキャッチする専用のメールボックスを作成する。

3. 特定のドメインについては、DomainType を "InternalRelay" に設定します。 後で Catch All を削除する場合は、必ずドメインを [権限あり] に戻してください。

4. メールフローのトランスポート ルールの作成方法は次のとおりです:

    - 送信者が "組織外" のユーザーの場合
    - メッセージを Catchall@domain.com にリダイレクトする
    - ただし受信者が allusers@domain.com のメンバーである場合を除く (配布グループはすべてのメンバーを含む)
    - 新しいメールボックスが動的配布グループに追加されたことを確認する
