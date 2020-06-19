---
title: 1385-Office-365-アラート-ポリシー
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 05c58bded5ba45aef8ae3bc1d33491e6e0365c18
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502432"
---
# <a name="alert-policies"></a>アラート ポリシー

The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription. Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*". Alert notifications are sent when alerts are triggered for common activities, such as when users:

- メールを転送する受信トレイのルールを作成する。
- アクセス許可をメールボックスに割り当てる。
- SharePoint ファイル共有で、多数のファイルを共有または削除します。
- 電子情報開示検索を実行し、検索結果をエクスポートする。

アラートを確認して対応するには、次の操作を実行します。

1. [セキュリティ/コンプライアンス センター](https://protection.office.com)に移動して、サインインします。
2. [**アラート**] >  [**アラートの表示**] の順にクリックします。
3. アラートをクリックして、アラートに関する情報を含むポップアップ ページを表示させます。

You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account). Or you can simply close the alert by clicking **Resolve** on the alert flyout page.

アラート ポリシーの構成と管理の詳細については、[こちらの記事](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)を参照してください。

**重要**: Microsoft からのアラートのメール通知では、次の操作を要求することは決してありません。

- パスワードを入力する
- アカウントのセキュリティについての詳細を確認する
- 自分自身を再認証する

If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam. If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).