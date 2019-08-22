---
title: 1385-Office-365-アラート-ポリシー
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 46a029f262fa05edffa6f681c7205e289fe448c5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496344"
---
# <a name="office-365-alert-policies"></a>Office 365 アラート ポリシー

Office 365 セキュリティ/コンプライアンス センターには、Office 365 Enterprise または Office 365 US Government の E1/G1、G3/E3、E5/G5 のサブスクリプションを利用している組織に対してアラートをトリガーする[既定のアラート ポリシー](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies)が用意されています。そのため、管理者は、Office365Alerts@microsoft.com によって送信されたアラートのメール通知を、"重大度が低いアラート:*アラート ポリシー名*" といった件名で受信することがあります。一般的なアクティビティに対しアラートがトリガーされると、アラート通知が送信されます。たとえば、ユーザーが次のような操作を行った場合です。

- メールを転送する受信トレイのルールを作成する。
- アクセス許可をメールボックスに割り当てる。
- SharePoint ファイル共有で、多数のファイルを共有または削除する。
- 電子情報開示検索を実行し、検索結果をエクスポートする。

アラートを確認して対応するには、次の操作を実行します。

1. [セキュリティ/コンプライアンス センター](https://protection.office.com)に移動して、サインインします。
2. **[アラート] > [アラートの表示]** の順にクリックします。
3. アラートをクリックして、アラートに関する情報を含むポップアップ ページを表示させます。

アラートに対して、[不審な受信トレイのルールの削除](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account)などの操作を実行することができます。または、単にアラートのポップアップ ページで **[解決]** をクリックして、アラートを閉じることもできます。

アラート ポリシーの構成と管理の詳細については、[こちらの記事](https://docs.microsoft.com/office365/securitycompliance/alert-policies)を参照してください。

**重要**: Microsoft からのアラートのメール通知では、次の操作を要求することは決してありません。

- パスワードを入力する。
- アカウントのセキュリティについての詳細を確認する。
- 自分自身を再認証する。

このようなメール メッセージを受信した場合、Microsoft から送信されたものではありませんので、フィッシング詐欺を疑ってください。そうしたメールを受け取ったら、[Microsoft に報告してください](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop)。