---
title: 電子メールのキャッチをすべて作成する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2020
ms.locfileid: "42307116"
---
# <a name="create-an-email-catch-all"></a>電子メールのキャッチをすべて作成する

キャッチを使用しないことをお勧めします。 送信者にバウンスを提供することをお勧めします。メッセージが処理を実行できるように、そのメッセージをアドレス指定として配信できなかったことを知らせることができます。 また、監視対象のメールボックスを制限して、以前有効なメールアドレスのみをキャッチすることもできます。 

すべてのキャッチメールボックスは、適切なスパムを受信し、ほぼ監視されていない場合は最終的にはいっぱいになることがあります。 (受信制限があります。) 

続行する場合は、次の手順を実行します。

1. "すべての受信者の種類" を含む動的配布グループを作成 & ます。

2. メールをキャッチする専用のメールボックスを作成します。たとえば、catchall@domain.com のようにします。

3. 特定のドメインについて、DomainType を "InternalRelay" に設定します。 後でキャッチを削除した場合は、ドメインを [権限あり] に戻してください。

4. メールフロートランスポートルールを次のように作成します。

    - 送信者が組織外の場合
    - メッセージを Catchall@domain.com にリダイレクトします。
    - 受信者が allusers@domain.com のメンバーである場合を除きます (配布グループにはすべてのメンバーが含まれています)。
    - 新しいメールボックスが動的配布グループに追加されたことを確認する
