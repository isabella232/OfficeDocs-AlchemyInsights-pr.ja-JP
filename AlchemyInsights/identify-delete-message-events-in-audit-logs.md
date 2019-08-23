---
title: 監査ログの削除メッセージイベントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539214"
---
# <a name="audit-logs-for-deleted-email-messages"></a>削除された電子メールメッセージの監査ログ

2019年1月以降、Microsoft は既定でメールボックス監査ログをオンにしています。 または、特定のユーザーのメッセージイベントの削除を確認するには、監査の削除アクションを手動で有効にする必要があります。 メールボックス監査ログが組織または特定のユーザーに対して既に有効になっている場合は、次の手順を実行します。

1. [Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインする

2. [**検索と調査**] をクリックして、[**監査ログの検索**] を選択します。

3. [**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。 調査するユーザーのユーザー名 (アイテムを削除したユーザー) を指定します。 [**アクティビティ**] フィールドで、[削除済み**アイテムフォルダーからメッセージ**を削除し、削除済み**アイテムフォルダーにメッセージを移動**しました] を選択します。

4. **[検索]** をクリックします。

結果から、監査レコードを選択します。 詳細ポップアップで、[**詳細情報**] をクリックします。 削除されたアイテムに関する追加情報 (たとえば、アイテムが削除されたときの件名やアイテムの場所) は、 **AffectedItems**フィールドに表示されます。 **Clientinfostring**プロパティは、outlook、web 上の outlook (旧称 Outlook web App)、またはその他のデバイスで削除が行われた場合に表示されます。

詳細については、「[メールボックスのメール転送をセットアップするユーザーの特定](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)」を参照してください。

**注**: 監査ログ機能を使用して、削除されたアイテムを取得することはできません。 削除済みメッセージを Outlook on the web で取得するには、「 [Outlook Web App で削除済みアイテムを回復](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)する」を参照してください。
