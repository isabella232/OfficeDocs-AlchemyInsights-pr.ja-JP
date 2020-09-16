---
title: SharePoint のアラート通知が配信されない
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751248"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint のアラート通知が配信されない

アラートはメールの [迷惑メール] フォルダーに移動される場合があるため、このフォルダーを確認してください。

**すべてのアラートが配信されない**のか、特定のファイルまたはライブラリからの**個別のアラートが配信されない**のかを特定します。

- **個別のアラートが配信されない場合**: 特定のファイルやライブラリからの個別のアラートが配信されない場合は、アラートを削除してから再作成してみてください。 詳細については、「[SharePoint アラートの管理、表示、または削除](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)」を参照してください。
- **すべてのアラートが配信されない場合**: 複数のファイルやライブラリからのすべてのアラートが配信されない場合は、[[サービス正常性](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)] ダッシュボードにアクセスして、SharePoint または Exchange でインシデントやアドバイザリが発生していないかどうかを確認します。 問題の原因は、SharePoint のアラート機能によるもの、または Exchange 経由のメールの遅延によるものである可能性があります。 また、その他のメールが配信されているかどうかを確認することも重要です。配信されていない場合は、問題の原因が Exchange の遅延である可能性が高くなります。

アラートに関する FAQ:

- 配布グループにアラートを送信することはできません。サポートされているのはセキュリティ グループと O365 グループのみです。
- アラート メール テンプレートをカスタマイズすることはできません。カスタマイズを行うには、Microsoft FLOW または SharePoint Designer ワークフローを使用する必要があります。

## <a name="related-topics"></a>関連項目

SharePoint Online で Microsoft Flow を試す方法。

- [フローを作成する](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint and Flow (SharePoint と Flow)](https://flow.microsoft.com//blog/sharepoint-and-flow/)
