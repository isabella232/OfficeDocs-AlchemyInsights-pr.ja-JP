---
title: Apple MDM プッシュ証明書が設定されていません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931547"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM プッシュ証明書が設定されていません

Apple MDM プッシュ証明書 (Apple Push Notification Service (APNS) 証明書とも呼ばれます) が、お客様のサブスクリプションに構成されていません。 Apple MDM プッシュ証明書が構成されていないと、iOS デバイスや Mac OS デバイスの登録および管理は行えません。 Intune に証明書を追加すると、ユーザーはポータル サイト アプリをインストールして iOS デバイスを登録することができるようになります。

1. **「同意します。」** を選び データを Apple に送信するためのアクセス許可を Microsoft に付与します。

2. Apple MDM プッシュ証明書の作成に必要な Intune 証明書署名要求を **CSR にダウンロードする** を選択します。 ファイルは、Apple Push Certificates ポータルから信頼関係の証明書を要求するのに使用します。

3. **MDM プッシュ証明書を作成する** を選択して、Apple Push Certificates ポータルに移動します。 会社の Apple ID でサインインし、**証明書を作成する** を選択します。 **ファイルを選ぶ** を選択し、証明書の署名要求ファイルに移動し、**アップロード** を選択します。 確認ページで、**ダウンロード** を選択して証明書 (.pem) ファイルをダウンロードし、ファイルをローカルに保存します。
 
**注**: 証明書は、作成に使用された Apple ID に関連付けられています。 ベスト プラクティスとして、管理タスクに会社の Apple ID を使用して、メールボックスを複数のユーザーまたは配布リストを使用して監視するようにしてください。 個人用の Apple ID は使用しません。 同じ Apple ID を使用して、12 か月ごとに Apple プッシュ証明書を更新します。
 
4. Apple MDM プッシュ証明書の作成に使用する Apple ID を入力します。 証明書を更新する必要がある場合のリマインダーとして、この ID を記録します。

5. 証明書 (.pem) ファイルに移動し、**開く** を選択して、**アップロード** を選択します。 プッシュ証明書を使用して、Intune で Apple デバイスを登録および管理できます。