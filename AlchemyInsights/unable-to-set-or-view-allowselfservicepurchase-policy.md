---
title: AllowSelfServicePurchase policy を設定または表示できません
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/16/2020
ms.locfileid: "42094398"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase policy を設定または表示できません

AllowSelfServicePurchase policy を設定または表示しようとすると、次のエラーメッセージが表示されます。

*HandleError: PolicyId ' AllowSelfServicePurchase '、ErrorMessage-基になる接続が閉じられました。送信で予期しないエラーが発生しました。*

これは、以前のバージョンのトランスポート層セキュリティ (TLS) が原因である可能性があります。 MSCommerce サービスを接続するには、TLS 1.2 以上を使用する必要があります。  

TLS プロトコルを有効または有効にするには、次の手順を実行してください。1.2、verify、および retry。
 1. PowerShell コマンドプロンプト (PS C::\)次のコマンドを入力して、TLS プロトコルをバージョン1.2 に設定します。

    \[Net.tcp Pointmanager]:: SecurityProtocol = \[Net.tcp protocol type]:: Tls12

2. 次のコマンドを使用して、使用されている TLS プロトコルを確認します。

    \[Net.tcp: ServicePointManager]:: SecurityProtocol 

3. 必要に応じて、Get または Update コマンドを再試行します。

