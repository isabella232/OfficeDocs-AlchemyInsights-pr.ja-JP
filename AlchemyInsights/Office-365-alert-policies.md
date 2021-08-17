---
title: 1385-Office-365-アラート-ポリシー
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 681f7609f32b004ddfa7bfbeff179757e7063657
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312692"
---
# <a name="alert-policies"></a>アラート ポリシー

Microsoft 365 には、Microsoft 365 Enterprise または Microsoft 365 US Government E1/G1、E3/G3、E5/G5 サブスクリプションを持つ組織に対してアラートをトリガーする [既定のアラート ポリシー](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)が含まれます。そのため、管理者は Office365Alerts@microsoft.com から送信された "低重要度アラート: *アラート ポリシーの名前*" などの件名でのアラート メール通知を受信する場合があります。アラート通知は、ユーザーによる以下のような一般的なアクティビティに対してアラートがトリガーされたときに送信されます。

- メールを転送する受信トレイのルールを作成する。
- アクセス許可をメールボックスに割り当てる。
- SharePoint ファイル共有で、多数のファイルを共有または削除します。
- 電子情報開示検索を実行し、検索結果をエクスポートする。

アラートを確認して対応するには、次の操作を実行します。

1. 次のいずれかの手順を実行します。
   - <https://compliance.microsoft.com> の Microsoft 365 コンプライアンス センターで、**[アラート]** に移動します。 または、**[アラート]** ページに直接移動するには、<https://compliance.microsoft.com/compliancealerts> を使用します。
   - <https://security.microsoft.com> の Microsoft 365 Defender ポータルで、**[インシデントとアラート]** \> **[アラート]** の順に移動します。 または、**[アラート]** ページに直接移動するには、<https://security.microsoft.com/alerts> を使用します。
2. アラートをクリックして、アラートに関する情報を含むポップアップ ページを表示させます。

アラートに対して、[不審な受信トレイのルールの削除](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)などの操作を実行することができます。または、単にアラートのポップアップ ページで **[解決]** をクリックして、アラートを閉じることもできます。

アラート ポリシーの構成と管理の詳細については、[こちらの記事](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)を参照してください。

**重要**: Microsoft からのアラートのメール通知では、次の操作を要求することは決してありません。

- パスワードを入力する
- アカウントのセキュリティについての詳細を確認する
- 自分自身を再認証する

これらの種類の要求を含むメール メッセージを受信した場合、それは Microsoft から送信されたものではないため、フィッシング詐欺と見なす必要があります。 これらの種類の要求を含むメッセージを受信した場合は、[そのメッセージを Microsoft に報告してください](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)。
