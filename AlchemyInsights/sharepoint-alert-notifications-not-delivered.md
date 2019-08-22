---
title: SharePoint 通知通知が配信されない
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f389785fcd1029ae5a47e07c723874f9f214109d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504468"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint 通知通知が配信されない

通知が表示される場合があるので、メールの迷惑メールフォルダーを確認してください。

すべての**通知が配信されていない**か、特定のファイルまたはライブラリからの**個々の通知**が配信されていないかを確認します。

- **個別の通知が配信**されない: 特定のファイルまたはライブラリからの個々の警告が配信されない場合は、削除して再作成します。 通知を再作成するには、「 [SharePoint alerts を管理、表示、または削除](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)する」を参照してください。
- **すべての通知が配信**されない: 複数のファイルまたはライブラリからのすべての通知が配信されない場合は、[サービス正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)にアクセスして、SharePoint または Exchange で発生している可能性があるすべてのアドバイザリ/インシデントをチェックします。 この問題は、SharePoint の通知機能または Exchange を経由した電子メールの遅延が原因である可能性があります。 また、他の電子メールが配信されているかどうかを確認することも重要であり、そうでない場合は、Exchange の遅延が原因であると考えられます。

警告の FAQ:

- 配布グループに通知を送信することはできません。セキュリティと O365 グループのみがサポートされています。
- 通知電子メールテンプレートをカスタマイズすることはできません。これらのことを実現するには、Microsoft FLOW または SharePoint Designer ワークフローを使用する必要があります。

詳細情報:

- **通知のセットアップ**: 通知の設定の詳細については、「 [SharePoint でファイルまたはフォルダーが変更されたときに通知を受け取る通知を作成する](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)」を参照してください。
- **アラートのトラブルシューティング**: 通知のトラブルシューティングの詳細については、「[ユーザーが SharePoint Online](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)の通知を受信しない」を参照してください。
- **Advanced O365 コンプライアンスアラートポリシー**: これらの通知の設定の詳細については、「[コンプライアンス警告ポリシー](https://docs.microsoft.com/office365/securitycompliance/alert-policies)」を参照してください。
- **SharePoint および OneDrive 監査ログ**: これらのイベントを取得する方法の詳細については、「 [Search the Audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。
- **Advanced Threat Protection によって送信されるアラート**: 「 [SharePoint および OneDrive の ATP](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)」を参照してください。
- **データ損失防止ポリシーによって送信されるアラート**: 「 [DLP ポリシーの電子メール通知](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)」を参照してください。

## <a name="related-topics"></a>関連項目

SharePoint Online で Microsoft Flow を試す場合

- [フローを作成する](https://support.office.com/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint およびフロー](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
