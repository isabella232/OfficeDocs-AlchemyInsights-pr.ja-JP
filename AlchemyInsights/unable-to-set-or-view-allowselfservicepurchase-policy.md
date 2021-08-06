---
title: AllowSelfServicePurchase ポリシーを設定または表示できません
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
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020197"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>AllowSelfServicePurchase ポリシーを設定または表示できません

AllowSelfServicePurchase ポリシーを設定または表示しようとすると、次のエラー メッセージが表示されます。

*HandleError: PolicyId 'AllowSelfServicePurchase' で製品ポリシーを取得できませんでした、ErrorMessage - 基になる接続が閉じられました: 送信で予期しないエラーが発生しました。*

これは、トランスポート層セキュリティ (TLS) の古いバージョンが原因である可能性があります。 MSCommerce サービスに接続するには、TLS 1.2 以降を使用する必要があります。  

次の手順を試して、TLS プロトコルを 1.2 に有効化/設定し、確認して、再試行します。
 1. PowerShell コマンドプロンプトで (PS C:\) 次のコマンドを入力して、TLS プロトコルをバージョン 1.2 に設定します。

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 次のコマンドを使用して、使用中の TLS プロトコルを確認します。

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 必要に応じて、Get または Update コマンドを再試行します。

