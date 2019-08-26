---
title: SharePoint のアラート通知が配信されない
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504468"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint のアラート通知が配信されない

アラートはメールの [迷惑メール] フォルダーに移動される場合があるため、このフォルダーを確認してください。

**すべてのアラートが配信されない**のか、特定のファイルまたはライブラリからの**個別のアラートが配信されない**のかを特定します。

- **個別のアラートが配信されない場合**: 特定のファイルやライブラリからの個別のアラートが配信されない場合は、アラートを削除してから再作成してみてください。 詳細については、「[SharePoint アラートの管理、表示、または削除](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)」を参照してください。
- **すべてのアラートが配信されない場合**: 複数のファイルやライブラリからのすべてのアラートが配信されない場合は、[[サービス正常性](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)] ダッシュボードにアクセスして、SharePoint または Exchange でインシデントやアドバイザリが発生していないかどうかを確認します。 問題の原因は、SharePoint のアラート機能によるもの、または Exchange 経由のメールの遅延によるものである可能性があります。 また、その他のメールが配信されているかどうかを確認することも重要です。配信されていない場合は、問題の原因が Exchange の遅延である可能性が高くなります。

アラートに関する FAQ:

- 配布グループにアラートを送信することはできません。サポートされているのはセキュリティ グループと O365 グループのみです。
- アラート メール テンプレートをカスタマイズすることはできません。カスタマイズを行うには、Microsoft FLOW または SharePoint Designer ワークフローを使用する必要があります。

詳細情報:

- **アラートの設定**: アラートの設定の詳細については、「[SharePoint でファイルやフォルダーが変更されたときに知らせてくれる通知を作成する](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)」を参照してください。
- **アラートのトラブルシューティング**: アラートのトラブルシューティングの詳細については、「[ユーザーが SharePoint Online アラート通知を受信していない](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)」を参照してください。
- **高度な O365 コンプライアンス アラート ポリシー**: この種類のアラートの設定の詳細については、「[コンプライアンス アラート ポリシー](https://docs.microsoft.com/office365/securitycompliance/alert-policies)」を参照してください。
- **SharePoint および OneDrive 監査ログ**: これらのイベントを取得する方法の詳細については、「[監査ログを検索する](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。
- **Advanced Threat Protection によって送信されるアラート**: 「[ATP for SharePoint and OneDrive (SharePoint および OneDrive 用の ATP)](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)」を参照してください。
- **データ損失防止ポリシーによって送信されるアラート**: 「[Email notifications for DLP policies (DLP ポリシーのメール通知)](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)」を参照してください。

## <a name="related-topics"></a>関連項目

SharePoint Online で Microsoft Flow を試す方法。

- [フローを作成する](https://support.office.com/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint and Flow (SharePoint と Flow)](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
